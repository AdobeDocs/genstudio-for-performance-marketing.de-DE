---
title: Journey Optimizer für GenStudio
description: Installieren und konfigurieren Sie die App Journey Optimizer for GenStudio Adobe Exchange , damit Ihr Unternehmen Adobe Journey Optimizer-Vorlagen in GenStudio for Performance Marketing verwenden kann.
feature: Extensibility
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Journey Optimizer für GenStudio

Organisationen, die [!DNL Adobe Journey Optimizer] (AJO) und [!DNL GenStudio for Performance Marketing] in derselben [!DNL IMS] verwenden, können die App **Journey Optimizer for GenStudio** von [!DNL Adobe Exchange] installieren. Nachdem ein Systemadministrator die App genehmigt und die Bereitstellung abgeschlossen hat, können Autorinnen und Autoren beim Erstellen von E-Mail-Erlebnissen in GenStudio neben Vorlagen, die direkt in [!DNL Content] hochgeladen wurden, AJO-Inhaltsvorlagen auswählen.

Dieses Thema richtet sich an **Administratoren und Entwickler** die die App installieren, OAuth-Anmeldeinformationen in der [!DNL Adobe Developer Console] erstellen und Berechtigungen für technische Konten in [!DNL Adobe Experience Platform] zuordnen. Informationen zur Funktionsweise der Vorlagensyntax für AJO und Marketo mit GenStudio finden Sie unter [Vorlagen aus AJO und Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Voraussetzungen

* AJO muss in der Organisation bereitgestellt werden, in der Sie die Erweiterung bereitstellen.
* Benutzende, die Vorlagen in AJO erstellen, benötigen die Berechtigung **Erstellen und Bearbeiten** von Inhaltsvorlagen in Journey Optimizer, wie sie in Ihrem Unternehmen definiert sind.
* E-Mail-Vorlagen in AJO müssen Platzhalter für Felder (Handlebars) enthalten, in denen generierte Inhalte angezeigt werden sollen. Eine Vorlage kann ohne diese Felder ausgewählt werden, aber **Erlebnisgenerierung schlägt fehl** wenn die von [!DNL GenStudio for Performance Marketing] erwarteten Platzhalter fehlen. Siehe [Anpassen einer ](/help/user-guide/templates/customize-template.md) und [Erkannte Feldnamen](/help/user-guide/templates/customize-template.md#recognized-field-names).

## Installieren der App über Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483287?learn=on)

1. Öffnen Sie [Adobe Exchange](https://exchange.adobe.com) und wechseln Sie zu **[!UICONTROL CX Enterprise]**.
1. Öffnen Sie die Liste [Journey Optimizer for GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio).
   ![Journey Optimizer for GenStudio-Auflistung in Adobe Exchange, einschließlich Anforderungen und kostenloser Installation](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. Wählen Sie **[!UICONTROL Kostenlos]** aus, um die App für Ihre Organisation anzufordern.
1. Nachdem Ihr Unternehmen **die Anfrage geprüft und**, fahren Sie mit dem [Erstellen von OAuth-Anmeldeinformationen in Adobe Developer Console](#create-oauth-credentials-in-adobe-developer-console) und [Bereitstellen des Programms aus Exchange](#deploy-the-application-from-exchange) fort.

## Erstellen von OAuth-Anmeldeinformationen in Adobe Developer Console

Erstellen Sie **Projekt** in der [Adobe Developer Console](https://developer.adobe.com/console/) das OAuth-Anmeldeinformationen für die Journey Optimizer-API bereitstellt. Sie benötigen Werte wie **Client-ID**, **Client-Geheimnis**, **Organisations-ID** und **Umfang** beim Konfigurieren der App in Exchange.

1. Melden Sie sich bei Adobe Developer Console an und erstellen Sie ein **neues Projekt**.
1. Fügen Sie die **Adobe Journey Optimizer (AJO)-** zum Projekt hinzu, indem Sie auf **[!UICONTROL API hinzufügen]** klicken und **[!UICONTROL Adobe Journey Optimizer]** aus der Liste der **[!DNL CX Enterprise]**-Produkt-APIs auswählen.
1. Generieren Sie Anmeldeinformationen im Projektarbeitsbereich und kopieren Sie **Client-ID**, **Client-Geheimnis**, **Organisations-ID**, **Scope** und alle anderen Werte, nach denen Ihr Bereitstellungsfluss fragt. Bewahren Sie sie für den nächsten Abschnitt sicher auf.

>[!NOTE]
>
>Verwenden Sie bei der Installation über Exchange die **OAuth-Client-ID**, wenn sowohl eine OAuth-Client-ID als auch eine ID des technischen Kontos angezeigt wird.

## Anwendung von Exchange bereitstellen

### Öffnen Sie die App in Verwalten und fügen Sie eine Umgebung hinzu

1. Kehren Sie zu [Adobe Exchange ](https://exchange.adobe.com).
1. Wählen Sie **[!UICONTROL Verwalten]** und öffnen Sie **[!UICONTROL App Builder-]** (oder den Pfad Ihres Unternehmens zu verwalteten Apps).
1. Wählen Sie **Journey Optimizer für GenStudio aus** bestätigen Sie, dass die App **genehmigt** ist.
1. Wählen **[!UICONTROL unter &quot;]**&quot; eine vorhandene Umgebung aus dem Dropdown **Umgebungen:** oder wählen Sie **[!UICONTROL Umgebung hinzufügen]**, um eine Umgebung zu erstellen.
   ![Anwendungsdetails mit dem Status Genehmigt und Umgebung hinzufügen](/help/extensibility/ajo-config-002.png){width="50%"}
1. Wählen Sie in der ausgewählten Umgebung **[!UICONTROL Konfiguration]** aus.
1. Suchen Sie auf der **[!UICONTROL Konfiguration]** nach **[!UICONTROL AJO-Anmeldeinformationen]**.
   ![Konfiguration mit AJO-Anmeldeinformationen vor der Bereitstellung (Entwurf)](/help/extensibility/ajo-config-004.png){width="80%"}
1. Geben Sie die Anmeldeinformationen aus dem Developer Console-Projekt ein, dem die Journey Optimizer-API hinzugefügt wurde (z. B. **[!UICONTROL AJO Client ID]**, **[!UICONTROL AJO Client Secret]** und **[!UICONTROL AJO Token Endpoint]** und alle anderen erforderlichen Felder).
1. Geben Sie den **Sandbox-Namen in Kleinbuchstaben** ein (z. B. `prod`).
1. Klicken Sie **[!UICONTROL Bereitstellen]**. Nach Abschluss der Bereitstellung wird der Status als „bereitgestellt“ angezeigt. Der Schaltflächentext ändert sich in „Bereitstellung **[!UICONTROL &quot;]**.
   ![Bereitgestellte Anwendung mit „Bereitstellung aufheben“ in der Ansicht &quot;App Builder-Anwendungen“](/help/extensibility/ajo-config-005.png){width="80%"}

Nach der Bereitstellung enthält die Adobe Developer Console ein neues automatisch generiertes Projekt mit dem Namen **Journey Optimizer für GenStudio &lt;your_environment_name>** mit AJO- und Adobe Runtime-APIs. Dieses Projekt ist schreibgeschützt und kann nicht bearbeitet oder gelöscht werden.
![Schreibgeschütztes, automatisch generiertes Developer Console-Projekt nach der Bereitstellung](/help/extensibility/ajo-auto-project.png){width="100%"}

### Konfiguration aktualisieren

Um Konfigurationsvariablen für eine Umgebung zu ändern, **[!UICONTROL Sie „Bereitstellung aufheben]** aktualisieren Sie zunächst die Werte und dann erneut **[!UICONTROL Bereitstellen]**, damit die Änderungen wirksam werden.

Sie können **mehrere Umgebungen** in Exchange erstellen (z. B. eine pro Sandbox). Jede Bereitstellung kann als separates Erlebnis in GenStudio angezeigt werden, wenn Ihr Unternehmen mehrere Sandboxes verwendet.

## Berechtigungen für das technische Konto zuordnen

Benutzende können die AJO-Erweiterung in GenStudio ohne vollständigen [!DNL Adobe Experience Platform] sehen. Für API-Aufrufe (z. B. zum Laden von Vorlagen) müssen dem technischen Konto, das mit den OAuth-Anmeldeinformationen verknüpft ist, Journey Optimizer-Berechtigungen unter **[!DNL Adobe Experience Platform]** > **[!UICONTROL Berechtigungen]** gewährt werden. Die genauen Rollennamen und Berechtigungssätze hängen von Ihrer Organisation ab.

Zeigen Sie die Erweiterung unter **[!UICONTROL Journey Administrator]** in AJO **[!UICONTROL Berechtigungen]** > **[!UICONTROL Rollen]** an und fügen Sie die **API-** aus dem Developer Console-Projekt hinzu. Dabei handelt es sich um dieselben Anmeldeinformationen, die Sie bei der Bereitstellung von Exchange verwendet haben.

![API-Anmeldeinformationen, die der Rolle AJO-Architekt in Adobe Experience Platform-Berechtigungen zugewiesen sind](/help/extensibility/ajo-map-permissions.png){width="80%"}

**Siehe auch** (Journey Optimizer-Zugriffssteuerung):

* [Zugangssteuerung](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Berechtigungen in Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Erste Schritte für Systemadministratoren](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/quick-start/administrator)

## Zugriff auf AJO-Vorlagen in GenStudio

Nach der Bereitstellung und der Berechtigungszuordnung:
1. Öffnen Sie **[!UICONTROL Erstellen]** in GenStudio for Performance Marketing und starten Sie ein **E-Mail** Erlebnis.
1. Öffnen Sie **[!UICONTROL Vorlage auswählen]** die Registerkarte **[!UICONTROL AJO-Vorlage]** neben **[!UICONTROL Hochgeladene Vorlagen]**, um Vorlagen aus Journey Optimizer zu durchsuchen.

![Vorlage mit AJO-Vorlagenregisterkarte und Vorlagenkatalog auswählen](/help/extensibility/ajo-template-tab.png){width="80%"}

## Fehlerbehebung

### Die Registerkarte AJO-Vorlagen wird nicht angezeigt

* Bestätigen Sie, dass die in Exchange **[!UICONTROL Konfiguration]** eingegebenen Werte korrekt sind, einschließlich **Client-ID**, **Client-Geheimnis**, **Umfang** und **Sandbox**.
* Stellen Sie sicher **dass der (Sandbox-Name in Kleinbuchstaben** vorliegt (z. B. `prod`).
* Verwenden Sie bei der Installation von Exchange die **Client-ID** wie unter [Erstellen von OAuth-Anmeldeinformationen](#create-oauth-credentials-in-adobe-developer-console) beschrieben.

### Die Registerkarte AJO-Vorlagen wird angezeigt, es werden jedoch keine Vorlagen angezeigt

* Laden Sie die Seite neu oder öffnen Sie die Registerkarte **[!UICONTROL AJO]** erneut.
* Überprüfen Sie im **[!UICONTROL &quot;]**&quot; die **`get-templates`**. Wenn &quot;**403 Forbidden** zurückgegeben wird, wird das technische Konto keiner Rolle oder Gruppe mit den erforderlichen Journey Optimizer-Berechtigungen zugewiesen. Aktualisieren Sie Zuordnungen in [!DNL Adobe Experience Platform] **[!UICONTROL Berechtigungen]** und in AJO **[!UICONTROL Berechtigungen]** je nach Bedarf Ihres Unternehmens.
