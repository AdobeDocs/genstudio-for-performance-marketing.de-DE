---
title: Workfront Proof-Integration mit Überprüfung und Genehmigung
description: Integration von Workfront Proof mit Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
exl-id: 149db773-4787-4cfb-b29e-c49f13abf39a
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Integration von Workfront Proof mit GenStudio for Performance Marketing

Die Integration mit Workfront Proof verbessert den Überprüfungs- und Genehmigungs-Lebenszyklus von GenStudio for Performance Marketing mit erweiterten Funktionen, einschließlich Genehmigungsvorlagen, mehrstufigen Workflows und der Möglichkeit, Korrekturabzugsversionen [ vergleichen](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Diese strukturierte Versionierung gewährleistet Transparenz, Verantwortlichkeit und optimierte Zusammenarbeit während des gesamten Lebenszyklus der Inhaltsüberprüfung.

>[!BEGINSHADEBOX]

**Voraussetzungen**:

Installieren Sie die Erweiterung [Adobe Workfront Web Viewer](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proofs [!DNL Proofing Viewer] ist ein umfangreicher Arbeitsbereich zum Anzeigen, Kommentieren und Vergleichen von Korrekturabzügen. Von [!DNL Proofing Viewer] aus haben Sie folgende Möglichkeiten

* Vergleichen verschiedener Versionen des Inhalts
* Hinzufügen von Kommentaren und Zeichnungsmarkierungen zu einem Korrekturabzug
* Korrekturabzug genehmigen

[!DNL Proofing Viewer] wird geladen, wenn Sie auf die Korrekturabzugs-URL in der E-Mail mit der Genehmigungsanfrage oder in der produktinternen Benachrichtigung klicken. Die [!DNL Proofing Viewer] Ansicht _Meine neue Genehmigung_ wird geöffnet. In dieser Ansicht können Sie Inhalte überprüfen und Kommentare mithilfe der wichtigsten [!DNL Proofing Viewer]-Tools eingeben.

Um [!DNL Proofing Viewer] zu beenden, klicken Sie auf **[!UICONTROL Zurück zu GenStudio]**.

## Genstudio für Performance Marketing und Workfront Proof: Funktionsvergleich

In der folgenden Tabelle werden die standardmäßigen Überprüfungs- und Genehmigungsfunktionen von GenStudio for Performance Marketing mit den erweiterten Funktionen verglichen, die über die Workfront Proof-Integration verfügbar sind.

| Funktion        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Lebenszyklus von Entwürfen/Korrekturabzügen**        | Der Entwurfsinhalt läuft mit der Veröffentlichung ab. | Mehrstufige, rollenbasierte Genehmigungsketten mit zeitgestempelten, persistenten Protokollen.<br> Alle Versionen werden auf unbestimmte Zeit beibehalten. |
| **Kommentare**                | Kommentare sind mit einer Entwurfs-ID verknüpft und werden nach der Veröffentlichung verworfen.                                           | Persistente Kommentare und Anmerkungen werden zur Prüfung und Compliance beibehalten.     |
| **Versionen**           | Entwürfe werden als eindeutige Instanzen behandelt.<br>Kein Seitenvergleich.                                      | Vollständige Versionskontrolle mit Side-by-Side- und Overlay-Vergleichstools.        |
| **Projektmanagement** | Grundlegende Kampagnenverwaltung. | Umfassendes Kampagnen-Lifecycle-Management, einschließlich Anpassung, Vorlagen, Reporting und detaillierter Audits. |

### Lizenzen und Benutzerrollen

Lizenzen identifizieren die Gruppe von Benutzerberechtigungen innerhalb eines Produkts. Workfront Proof bietet mehr Lizenztypen oder Benutzerrollen als GenStudio for Performance Marketing. [Übersicht über Korrekturabzugsrollen](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) führt Benutzerrollen ein, die mit dem Workfront Proof-Workflow für Überprüfung und Genehmigung verknüpft sind.

| GenStudio for Performance Marketing-Lizenz       | Workfront-Lizenz                 | Beschreibung                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Workfront-Administrator/Hauptbenutzer | Vollständiger Zugriff auf GenStudio Performance Marketing-Funktionen wie Marken-, Rollen- und Produktverwaltung. Verwaltet Workflows und Einstellungen Erstellt Validierungsvorlagen. |
| Inhaltsersteller und -editor (Power-User-Lizenz)   | Korrekturabzug-Ersteller (Standardlizenz)  | Erzeugt Inhaltsentwürfe und sendet sie. Lädt in der Korrekturabzugsansicht Assets hoch und initiiert Korrekturabzüge. Erfordert eine Workfront Proof-Lizenz.                              |
| Prüfende Person/genehmigende Person (Mitwirkende-Lizenz)        | Prüfer/genehmigende Person                 | Nimmt an mehrstufigen Reviews teil, fügt Kommentare hinzu und genehmigt oder lehnt Inhalte ab.                                                                             |

Adobe-Systemadministratoren verwalten die Benutzerbereitstellung und Berechtigungen für beide Produkte in der Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof bietet [zusätzliche Benutzerrollen](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Nicht alle Rollen sind innerhalb von Performance Marketing sichtbar. Das System berücksichtigt jedoch alle Rollen, die in einer Workfront Proof-Vorlage festgelegt sind.

### Entwürfe und Testsendungen

Workfront [!DNL Proofing Viewer] erweitert den grundlegenden Überprüfungs- und Genehmigungsprozess von GenStudio for Performance Marketing um strukturiertere Überprüfungs- und Genehmigungsfunktionen. Die in dieser Integration überprüften Testsendungen sind auf die Formate beschränkt, die von GenStudio for Performance Marketing unterstützt werden.

### Versionskontrolle

GenStudio for Performance Marketing unterstützt keine Genehmigungsvorlagen, Workfront Proof jedoch. Die Versionierungsfunktionen des Korrekturabzugs verbessern den Prozess der Inhaltsüberprüfung und -validierung von GenStudio erheblich. Jede Übermittlung im Korrekturabzugs-Workflow wird als separate Version des Inhaltsentwurfs oder -_behandelt_. Korrekturabzüge werden automatisch gespeichert und können nebeneinander mit vorherigen Iterationen verglichen werden. Stakeholder können Änderungen nachverfolgen, präzises Feedback geben und die Ausrichtung während des gesamten Prüfungszyklus beibehalten. Der Korrekturabzug bewahrt einen vollständigen Verlauf aller Kommentare, Entscheidungen und Versionen und unterstützt somit Auditbereitschafts- und Compliance-Anforderungen. Jede Version unterstützt auch mehrstufige, rollenbasierte Genehmigungs-Workflows, wobei jede Aktion - Genehmigung, Ablehnung oder Kommentar - klar protokolliert und mit einem Zeitstempel versehen ist.

### Validierungsvorlagen

Workfront Proof-Genehmigungsvorlagen bieten vorformatierte Schritte, die den Workflow für die Korrekturabzugsgenehmigung optimieren können. Zu diesen Vorlagen gehören ausgewählte Prüfer und genehmigende Personen, Rollen für Korrekturabzüge und Fristen, wodurch Konsistenz und Effizienz gewährleistet sind. Ersteller von Inhalten, die eine Überprüfung starten, können aus einem Satz vordefinierter Vorlagen für einphasige und mehrphasige Genehmigungs-Workflows auswählen.

In jedem Schritt der Workflow-Vorlage werden zugewiesene Validierungsverantwortliche identifiziert. Alle Statusaktualisierungen und Kommentare aus dem Workfront Proof-Workflow sind im Proofing Viewer sichtbar, was die Transparenz und Zusammenarbeit verbessert.

Genehmigungsvorlagen unterstützen mehrstufige Genehmigungen, die die Koordinierung von Überprüfungen von verschiedenen Gruppen von Stakeholdern unterstützen.

### Kommentare

Reviewer können direkt auf bestimmte Bereiche des Testversands klicken, um präzise, kontextuelle Kommentare zu hinterlassen. Alle Kommentare erhalten einen Zeitstempel und werden als Teil des Versionsverlaufs des Korrekturabzugs gespeichert. Der Kommentarverlauf ist in GenStudio for Performance Marketing nicht verfügbar.

Sie können [zwei Versionen eines Korrekturabzugs vergleichen](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) um Prüfungskommentare und -inhalte auszuwerten.

## Benachrichtigungen und Erinnerungen

Prüfende und genehmigende Personen erhalten E-Mail-Benachrichtigungen, wenn ein neuer Korrekturabzug zur Überprüfung verfügbar ist oder wenn sich der Status einer laufenden Überprüfung geändert hat.
[Korrekturabzugsbenachrichtigungen und -](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders): enthalten einen personalisierten Link zum Korrekturabzug, Details zum Korrekturabzug und seinem Fortschritt während des Genehmigungsprozesses sowie Versionsinformationen.
