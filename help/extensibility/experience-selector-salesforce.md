---
title: Experience Selector-MFE in Salesforce
description: Erfahren Sie, wie Sie den Experience Selector-MFE in Salesforce Lightning bereitstellen und konfigurieren, einschließlich CSP, Adobe-Authentifizierung, Apex-E-Mail-Vorlagen und Validierung.
feature: Extensibility, Extensions, Experiences
source-git-commit: 4cac970f46ab08bcec2f23fd882c552af088c4ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Experience Selector-MFE in Salesforce

In diesem Abschnitt wird erläutert, wie Kunden und Implementierer das [!DNL GenStudio for Performance Marketing] Experience Selector Micro Frontend (MFE) in einer Salesforce-Organisation bereitstellen und ausführen können. Es behandelt Administratorschritte (kein Code), Entwicklerschritte (Bereitstellen und Konfigurieren) und sicherheitsbezogene Einstellungen wie die Content Security Policy (CSP).

Allgemeine Optionen zur MFE-Integration, Konfigurationseigenschaften und Framework-Beispiele finden Sie unter [GenStudio Experience Selector-MFE](experience-selector.md).

## Funktionsweise dieser Integration

>[!VIDEO](https://video.tv.adobe.com/v/3491088?captions=ger&learn=on)

Die Lightning-Web-Komponente (LWC) lädt `sfgsmfe` Adobe Experience Selector-UMD-Bundle und rendert es in einem `<dialog>`, damit Benutzer ein Erlebnis aus [!DNL GenStudio for Performance Marketing] auswählen können.

Die Integration kann auch:

* **Vorschau und Decodierung:** Zeigt die ausgewählte Payload als JSON, decodierten HTML und eine bereinigte HTML-Vorschau im LWC an.
* **E-Mail-Vorlagen (optional):** Ein **[!UICONTROL E-Mail-Vorlage erstellen]**-Fluss in Salesforce kann Apex (`EmailTemplateController.createEmailTemplate`) aufrufen, um einen `EmailTemplate`-Datensatz (HTML, Betreff und Ordner) einzufügen.
* **Laufzeitladen:** Das GenStudio-Skript wird von der in Adobe gehosteten URL auf `experience.adobe.com` geladen, nicht von einer statischen Salesforce-Ressource in der typischen Implementierung.

## Voraussetzungen

* **Salesforce-Organisation:** Eine Sandbox- oder Produktions-Organisation, in der Sie Metadaten bereitstellen und &quot;**[!UICONTROL App Builder&quot;]** können.
* **Salesforce-CLI:** Die Salesforce-CLI (`sf`) wird installiert und authentifiziert, z. B.:

  ```bash
  sf org login web --alias <your-org-alias>
  ```

* **Berechtigungen:** Benutzer, die E-Mail-Vorlagen erstellen, benötigen Zugriff auf den E-Mail-Zielvorlagenordner und Rechte zum Erstellen von Vorlagen entsprechend Ihren Organisationsrichtlinien. Apex wird `with sharing` ausgeführt.
* **Adobe/GenStudio:** Ihre Adobe IMS-Organisations-ID und SUSI-`clientId` müssen mit Ihrer Adobe-Konfiguration übereinstimmen (siehe &quot;[&#x200B; konfigurieren](#configure-integration-values-developer--implementation)).
* **Browser/CSP:** Salesforce muss das Laden von Skripten aus `https://experience.adobe.com` zulassen (siehe [Konfigurieren einer Inhaltssicherheitsrichtlinie und einer Adobe-URL](#configure-content-security-policy-and-adobe-url)).

## Bereitstellen des Pakets (Entwickler)

Die Integration folgt einem Salesforce DX-Stil-Layout. Der standardmäßige Paketordner wird normalerweise in Ihrem Salesforce DX-Projekt `force-app`.

1. Stellen Sie im Stammverzeichnis Ihres Projekts die Quelle für die Zielorganisation bereit:

   ```bash
   sf project deploy start --source-dir force-app --target-org <your-org-alias>
   ```

2. Vergewissern Sie sich, dass die Bereitstellung fehlerfrei abgeschlossen wird.

Typische Metadaten in Ihrem Projekt umfassen:

* Ein LWC-Bundle mit dem Namen `sfgsmfe` (HTML, JavaScript, CSS und Meta XML), das die Selektor-Benutzeroberfläche und das Laden von Skripten hostet.
* Eine Apex-Klasse (z. B. `EmailTemplateController`), die E-Mail-Vorlagen erstellt, wenn Sie diesen optionalen Fluss verwenden.

Ihr Projekt kann auch statische Ressourcen definieren. Wenn der LWC-Lader die Adobe CDN-URL für die `standalone.js` verwendet, sind diese Ressourcen für diesen Ladepfad nicht erforderlich, es sei denn, Sie ändern die Implementierung.

## Hinzufügen der Komponente zu einer Lightning-Seite (Admin)

Die `sfgsmfe` Komponente wird bereitgestellt für:

* Lightning-App-Seiten
* Startseiten
* Datensatzseiten
* Registerkarten (indem die Komponente auf einer Lightning-Seite platziert wird, die über eine benutzerdefinierte Registerkarte geöffnet wird)

So fügen Sie die Komponente hinzu:

1. Öffnen Sie **[!UICONTROL Setup]** &quot;**[!UICONTROL Manager]**.
1. Erstellen Sie eine **[!UICONTROL Neue Lightning-App]** (oder öffnen Sie eine vorhandene App, die Sie erweitern möchten).
   ![Das neue Lightning-App-Modal](./mfe-new-lighting-app.png){width="80%" zoomable="yes"}
1. Öffnen Sie die App und wählen Sie **[!UICONTROL Bearbeiten]** aus.
   ![Das Modal „Lightning-App bearbeiten“](./mfe-lightning-edit.png){width="80%" zoomable="yes"}
1. Erstellen Sie **[!UICONTROL Neue Seite]** (oder bearbeiten Sie eine vorhandene Lightning-Seite).
   ![Das Modal „Neue Seite“](./mfe-lightning-new-page.png){width="60%" zoomable="yes"}
1. Ziehen Sie **[!UICONTROL Lightning App Builder]** die Komponente **sfgsmfe** auf das Layout.
1. **[!UICONTROL Speichern]**, **[!UICONTROL Aktivieren]** und weisen Sie die Seite der richtigen Lightning-App, den richtigen Profilen und der richtigen App-Sichtbarkeit zu, damit die gewünschten Benutzer sie öffnen können.

## Konfigurieren der Inhaltssicherheitsrichtlinie und der Adobe-URL

Der LWC injiziert ein `<script>`-Tag, dessen `src` auf das UMD-Bundle von Adobe verweist, z. B.:

`https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js`

Sie müssen Salesforce so konfigurieren, dass dieser Ursprung für das Laden von Skripten gemäß den Sicherheitseinstellungen von CSP und Lightning Ihrer Organisation zulässig ist.

Wenn das Skript nicht geladen werden kann:

1. Öffnen Sie die Browser-Entwickler-Tools.
1. Überprüfen Sie die **[!UICONTROL Konsole]** und **[!UICONTROL Netzwerk]** auf blockierte Anfragen oder CSP-Verstöße.
1. Fügen Sie **[!UICONTROL CSP Trusted Sites]** (und alle zugehörigen Einstellungen für Ihre Salesforce-Version) für `https://experience.adobe.com` hinzu oder passen Sie sie entsprechend der aktuellen Salesforce-Dokumentation für Lightning an.

## Integrationswerte konfigurieren (Entwickler/Implementierung)

In der LWC-JavaScript sind für `sfgsmfe` mehrere Werte festgelegt. Kunden ersetzen diese in der Regel pro Umgebung.

| Wert | Beschreibung |
| --- | --- |
| `folderId` | Salesforce-Ordner-ID (`00l...`) für E-Mail-Vorlagen, in denen neue Vorlagen erstellt werden. Erforderlich für Apex; der Ordner muss vorhanden und für den ausgeführten Benutzer zugänglich sein. |
| `imsOrg` | Kennung der Adobe IMS-Organisation an `GenStudioExperienceSelector.renderExperienceSelectorWithSUSI` übergeben. |
| `susiConfig.clientId` | Adobe SUSI-Client-ID für die Registrierung der Experience Selector-App. |
| GenStudio `script.src` | URL des UMD-`standalone.js`; aktualisieren, wenn Adobe einen neuen Pfad veröffentlicht. |

Bei der Erstellung einer E-Mail-Vorlage werden GenStudio-Felder der Vorlage zugeordnet (z. B. Betreff aus `experienceFields`). Passen Sie Zuordnungen im LWC an, wenn Ihr Inhaltsmodell unterschiedlich ist.

Weitere Informationen zu `renderExperienceSelectorWithSUSI` und verwandten Optionen finden Sie [Konfigurationseigenschaften](experience-selector.md#configuration-properties) im MFE-Thema zur Erlebnisauswahl.

## Apex: EmailTemplateController

`EmailTemplateController.createEmailTemplate` typisch:

* Validiert den Vorlagennamen, die Ordner-ID und die nicht leere HTML.
* Erstellt eine `EmailTemplate` mit `TemplateType = 'custom'`-, `HtmlValue`-, `Subject`-, `Body`- und Ordnerzuweisung.
* Überträgt Fehler an das LWC bis `AuraHandledException`.

Tipps für den Betrieb:

* Beachten Sie die Eindeutigkeit und Benennungsregeln von DeveloperName in der Organisation.
* Bestätigen Sie die Ordner-ID und stellen Sie sicher, dass der Benutzer `EmailTemplate` Datensätze in diesem Ordner erstellen kann.
* Verwenden Sie Salesforce-Debug-Protokolle, wenn DML den genauen Fehler nicht erfassen kann.

## Validierungs-Checkliste

Diese Liste nach Bereitstellung und Konfiguration verwenden:

* [ ] Bereitstellung wird fehlerfrei abgeschlossen.
* [ ] Benutzer können die Lightning-Seite öffnen, die `sfgsmfe` enthält.
* [ ] Die Komponente zeigt keinen Ladefehler an. Die Registerkarte Netzwerk gibt HTTP 200 für `standalone.js` zurück.
* [ ] **[!UICONTROL GenStudio-Erlebnis auswählen]** wird die Auswahl geöffnet und Auswahlrückrufe werden ausgeführt.
* [ ] **[!UICONTROL E-Mail-]** erstellen) ist erfolgreich, wenn Sie diesen Fluss verwenden, und die Vorlage wird unter dem konfigurierten Ordner in &quot;**[!UICONTROL &quot;]**.

## Siehe auch

* [GenStudio Experience Selector-MFE](experience-selector.md)
