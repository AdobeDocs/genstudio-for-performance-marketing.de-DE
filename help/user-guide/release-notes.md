---
title: Versionshinweise zu Adobe GenStudio for Performance Marketing
description: Erfahren Sie mehr über die neuesten Funktionen und Verbesserungen von Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substantial-update: 2025-02-13T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 0d55b89d550a8e44e7dd354d809f00699fccf468
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 1%

---

# Versionshinweise zu GenStudio for Performance Marketing

Diese Versionshinweise enthalten die neuesten Aktualisierungen der GenStudio for Performance Marketing-Anwendung.

## 2 025,2,13 {#latest}

### Verbesserungen an der Landingpage für [!DNL Create]

Die [!DNL Create] Landingpage in GenStudio for Performance Marketing enthält Verbesserungen an der Benutzeroberfläche, die das Benutzererlebnis verbessern. Der _Letzte Arbeit_ wird verfeinert und mit der Listenansicht als Standardansicht konfiguriert. Abstände und andere visuelle Verbesserungen optimieren das Erscheinungsbild der [!DNL Create] Arbeitsfläche.

### Insights-Export in CSV

Sie können jetzt die anzeigbare Tabelle aus jeder [!DNL Insights] in eine CSV-Datei herunterladen. Diese Funktion ermöglicht den einfachen Export und die Analyse von Daten aus verschiedenen [!DNL Insights] und erleichtert so die Datenanalyse und Berichterstellung.

## Frühere Versionshinweise

+++Hinweise aus 2025.1.16

### Integration mit Adobe Workfront Proof

[!BADGE Beta]{type=Informative tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."}

Das Beta-Programm zur Integration von GenStudio for Performance Marketing und Adobe Workfront-Korrekturabzügen wird diesen Monat gestartet. Workfront Proof erhöht den Lebenszyklus der Inhaltserstellung und -aktivierung mit Genehmigungsvorlagen, mehrstufigen Workflows und Anmerkungen. GenStudio for Performance Marketing-Benutzende mit Workfront Proof-Berechtigungen können die erweiterten Funktionen des Korrekturabzugs in GenStudio for Performance Marketing verwenden, um GenStudio-generierte Inhalte zu überprüfen und zu kommentieren.

Beta-Programme bieten eine Möglichkeit, die Produktentwicklung zu gestalten und die allgemeine Verfügbarkeit zu bestimmen.

### Neue Aktionsaufrufe generieren

Sie können jetzt beim Verwalten von Varianten neue Ausdrücke für Aktionsaufrufe (CTA) generieren. Verwenden Sie die neuen Optionen _Umformulieren_ und _Link hinzufügen_, um neue Phrasen zu generieren und den CTA-Link zu bearbeiten. Ihre Vorlage muss ordnungsgemäß eingerichtet sein, damit diese neuen CTA-Funktionen funktionieren. Befolgen Sie die Richtlinien unter _Anpassen einer Vorlage_: [Aktionsaufrufe](/help/user-guide/content/customize-template.md#calls-to-action). Richtlinien zum Verwalten von CTAs in Varianten finden Sie unter [Revise Call to Action](/help/user-guide/create/manage-variants.md#revise-call-to-action). <!-- GS-6676 -->

### Fehlerbehebungen und Verbesserungen

* Die Zeichenzahl wird jetzt in allen erzeugten und manuellen Feldern von Display-Anzeigen angezeigt. Siehe _Zeichenanzahl_ in [Meta-](/help/user-guide/create/meta-experiences.md#character-counts)<!-- GS-7732 -->

* _Mitwirkende_ können jetzt Assets anzeigen, diese Assets jedoch nicht erstellen, bearbeiten oder löschen. Zuvor wurden Kollaborateurberechtigungen nicht wie erwartet in erzwungen[!DNL Create]. <!-- GS-7614 -->

* Inhaltseditoren können jetzt Asset-, Erlebnis- und Vorlagenmetadaten bearbeiten. <!-- GS-4905 -->

* Benutzerdefinierte Bildgrößen in Meta-Anzeigenvorlagen werden jetzt unterstützt. <!-- GS-7512 -->

* Die Auswahl von Rollen, Marken und Produkten wird jetzt während der Vorlagenerstellung vorgeladen. <!-- GS-8069 -->

* Der Link für E-Mail-Aktionsaufrufe ist kein erforderliches Feld mehr. <!-- GS-8103 -->

* Das Dropdown-Menü der [!DNL Brand] funktioniert jetzt für Vorlagen wie erwartet. Zuvor wurde der Selektor für einige Vorlagen nicht erfolgreich geladen. <!-- GS-8908 -->

* Bearbeiter können jetzt maximal vier Bilder für E-Mails mit einem Pod und Meta-Anzeigen auswählen. <!-- GS-2631 -->

* Der Jahreswert des Felds `Created by` eines genehmigten Erlebnisses bleibt nun wie erwartet konsistent, nachdem die Metadaten des Erlebnisses bearbeitet wurden. <!-- GS-8344 -->

* Inhaltseditoren können jetzt erfolgreich eine Vorlage aus [!DNL Create] auswählen. Zuvor gab die Anwendung einen Konsolenfehler aus, wenn ein Editor eine Vorlage auswählte.  <!-- GS-8798 -->

* Probleme mit Vorgängen zum Ändern der Größe und Neugenerieren für Meta-Anzeigen wurden behoben. <!-- GS-8900 -->

* Die Schaltfläche **[!UICONTROL Zurück]** gibt Benutzerinnen und Benutzer jetzt erwartungsgemäß entweder zur vorherigen Seite oder zur [!DNL Create] Landingpage zurück. <!-- GS-8622 -->

+++

+++Anmerkungen vom 12.12.2024

### Neue Funktionen

Bearbeiter können jetzt die folgenden Metadaten-bezogenen Aufgaben ausführen:

* Asset-, Erlebnis- und Vorlagenmetadaten bearbeiten. Siehe [Asset-Details](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* Zeigen Sie die generierten Tags eines Assets in der Ansicht _Details_ jedes Erlebnisses an, das das Asset verwendet. Siehe _Erzeugte Tags_ in [Asset-](/help/user-guide/content/asset-details.md#generated-tags)<!-- GS-3705 -->

Editoren können jetzt benutzerdefinierte Werte für diese Aspekte der generierten Varianten angeben:

* Breite und Höhe für Webbanner in Anzeigen-Vorlagen. Diese Werte werden jetzt als Vorlagenmetadaten gespeichert. <!-- GS-6735 -->

* Abmessungen der Bilder in Anzeigen-Erlebnissen während des Bild-Uploads.<!-- GS-7166 -->

* Siehe kanalspezifische Richtlinien in den [Best Practices für Vorlagen](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

Zu den Exportoptionen gehören jetzt:

* Exportieren Sie Display-Anzeigen und Meta-Anzeigen als HTML, JPEG oder PNG. Siehe [Erstellen eines Anzeigen-Erlebnisses](/help/user-guide/create/create-display-ad.md) und [Erstellen eines Meta-Anzeigen-](/help/user-guide/create/create-meta-ad.md)<!-- GS-7093 6655 5152-->

Zusätzliche neue Funktionen bieten Editoren folgende Möglichkeiten:

* Verwenden Sie die Schaltfläche **[!UICONTROL Aktualisieren]** in der Ansicht [!DNL Content]-Vorlage _Asset-_), um die ausgewählte Vorlage zu aktualisieren. <!-- GS-7102 -->

* Abschnitte von Anzeige- und E-Mail-Varianten neu generieren. Siehe [Erstellen eines Anzeigen-Erlebnisses](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) und [Erstellen eines E-Mail-Erlebnisses](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Duplizieren Sie bestehende Marken. Siehe [Marken verwalten](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

### Fehlerbehebungen und Verbesserungen

* Anzeigentitel werden jetzt erwartungsgemäß in [!DNL Content] gespeichert. <!-- GS-7239 -->

* Die Eingabeaufforderung wird nicht mehr geschlossen, wenn ein Editor außerhalb des Dropdown-Menüs der Schublade klickt. <!-- GS-7275 -->

* Das Dropdown-Menü [!DNL Create] [!DNL Persona]/[!DNL Product] wird jetzt wie erwartet geladen, wenn ein Fehler im URL-Service für Miniaturansichten auftritt. <!-- GS-7277 -->

* Anzeigen, die Elemente enthalten, die Fragmente überlagern, können jetzt bearbeitet werden. <!-- GS-7186 -->

* Die Canvas **[!UICONTROL Marke]**-Schaltfläche ist jetzt deaktiviert, wenn keine Markenbewertungen für ein Erlebnis generiert werden. <!-- GS-6429 -->

* Auf der Arbeitsfläche werden Erlebnisse in der Größe jetzt in konsistenter Reihenfolge angezeigt. <!-- GS-7123 -->

* Beim manuellen Zuschneiden werden jetzt bei der Bearbeitung von Display-Anzeigen Bildabmessungen und nicht Vorlagenabmessungen verwendet. Zuvor, wenn ein Bild kleiner war als die in der Anzeige und Vorlage angegebenen Abmessungen, verwendete der Begrenzungsrahmen Vorlagendimensionen, nicht Bilddimensionen. <!-- GS-7315 -->

* Bearbeiter können jetzt beim Erstellen einer Display-Anzeige bis zu vier Bilder auswählen. <!-- GS-7189 -->

* Die Entwürfe für Anzeigen und Meta-Anzeigen werden jetzt wie erwartet geladen, wenn die Größe in einem anderen Browser geändert wird. <!-- GS-7204 -->

* Nicht verwendete Vorlagenfelder werden im generierten Inhalt nicht mehr angezeigt.  <!-- GS-5670 -->

* Editoren können jetzt auf Links klicken, um sie wie erwartet in generierten Varianten zu bearbeiten. <!-- GS-7423 -->

* [!DNL Create] respektiert jetzt korrekt die Berechtigungen der Mitwirkenden. <!-- GS-7614 -->

* Die Schaltfläche **[!UICONTROL Größe ändern]** der Arbeitsfläche ist jetzt deaktiviert, nachdem alle Größenänderungsoptionen ausgewählt und gerendert wurden. <!-- GS-5940 -->

* Reviewer mit Lesezugriff können jetzt bei Reviews Varianten ein- und auszoomen. <!-- GS-7371 -->

* Der Tastaturfokus wurde nur zu ausführbaren Schaltflächen in der Ansicht [!DNL Create]Letzte _&quot;_. <!-- GS-4060 -->

* Die **Speichervorgang läuft** Meldung, die während der Speichervorgänge für E-Mail-Fragmente angezeigt wird, wird jetzt nur noch während des Speichervorgangs angezeigt. Zuvor wurde diese Nachricht auf der Arbeitsfläche unbegrenzt angezeigt. <!-- GS-6964 -->

* Editoren sehen jetzt eine Fehlermeldung wie erwartet, wenn ein Entwurf im Bereich [!DNL Create]Letzte Arbeit _nicht geladen_.  <!-- GS-8081 -->

* Auf der Arbeitsfläche werden jetzt in der Größe angepasste Meta-Anzeigen und Anzeigen in der richtigen Reihenfolge angezeigt.  <!-- GS-7375 -->

* Editoren können jetzt per Einzelklick in Felder in E-Mails klicken und Anzeigen anzeigen. <!-- GS-6297 -->

* Die Funktion zum Bearbeiten von Fragmenten für E-Mail- und Meta-Anzeigen wird jetzt wie erwartet durch einen einzigen Klick ausgelöst. <!-- GS-8081 -->

* Verbesserte Leistung der Schaltfläche [!DNL Create]**[!UICONTROL Zurück]**. <!-- GS-6767 -->

+++

+++Anmerkungen aus dem 14.11.2024

### Neue Funktionen

Es wurde Unterstützung für die Anzeige statischer Inhalte hinzugefügt, die auf externen Domains gehostet werden. GenStudio for Performance Marketing validiert die in der Vorlage definierte Inhaltsquelle und bettet eine Kopie ein, um die Vorlagenvorschau zu erstellen. Siehe [Statischer Inhalt](/help/user-guide/content/customize-template.md#static-content). <!-- GS-6107 -->

### Fehlerbehebungen und Verbesserungen

* Wenn die Größe in einem anderen Browser als dem, der zum Generieren des anfänglichen Inhalts verwendet wird, geändert wird, werden Entwürfe jetzt erwartungsgemäß geladen. <!-- GS-7204 -->

* Alle Zeichen werden nun in exportierten HTML korrekt dargestellt. <!-- GS-7246 -->

* Die Schaltflächen im Popup [!DNL Content] _Erlebnisse_ **[!UICONTROL Export]** sind in bestimmten Sprachen nicht mehr abgeschnitten. <!-- GS-6873 -->

* Display-Anzeigen, die mit Vorlagen erstellt wurden, die eine Größe von 50 x 50 haben, werden jetzt in der erwarteten Bildgröße exportiert. Zuvor wurden PNG-Dateien doppelt so stark exportiert wie erwartet. <!-- GS-7192 -->

* Vorlagenfehler, die beim Ändern der Größe von Display-Anzeigen aufgetreten sind, werden jetzt behoben. <!-- GS-7322 -->

### Lokalisierung

Diese Version umfasst Verbesserungen bei der Lokalisierung in der gesamten Benutzeroberfläche, einschließlich:

* Alle Zeichenfolgen im [!DNL Content]-Popup _Asset hochladen_ sind jetzt korrekt lokalisiert. <!-- GS-6872 6770 -->
* Alle QuickInfos im [!DNL Content] _Assets_ Ansichtsfeld **[!UICONTROL Suche]** sind lokalisiert. <!-- GS-6879 -->
* Beim Ersetzen eines vorhandenen Bildes in einer E-Mail-Variante auf der [!DNL Create]-Arbeitsfläche ist die Ansicht _Aus Inhalt auswählen_ jetzt lokalisiert. <!-- GS-6906 -->

+++

+++Anmerkungen vom 11.2024.07

### Fehlerbehebungen und Verbesserungen

* Das _„Speichern in Bearbeitung_ wird nicht mehr angezeigt, wenn ein Benutzer auf **[!UICONTROL Neues Bild hochladen]** klickt und dann den Vorgang abbricht, bevor der Upload abgeschlossen ist. <!-- GS-6780 -->

* Erlebnistitel werden jetzt bei der Regenerierung des Erlebnisses korrekt erstellt. <!-- GS-7006 -->

* Probleme mit flackernden Bildlaufleisten beim Laden von Entwürfen wurden behoben. <!-- GS-5587 -->

* Der `View documentation` Link im Popup-Fenster [!DNL Content]_Genehmigte Vorlage hinzufügen_ funktioniert jetzt erwartungsgemäß. <!-- GS-6881 -->

* Das Löschen eines Bildes aus der Eingabeaufforderungsschublade während eines Größenänderungsvorgangs führt nicht mehr zu einem Fehler. <!-- GS-7115 7009 -->

* Die Auswahl **[!UICONTROL Löschen]** aus dem [!DNL Create] Aktionsmenü (…) funktioniert jetzt erwartungsgemäß. <!-- GS-6871 -->

* Benutzer können jetzt alle interaktiven Meta- und Vorlagenelemente allein über die Tastatur steuern. <!-- GS-4066 -->

* Es wurde eine Extraktion von Bildabmessungen aus Vorlagenbildfeldern hinzugefügt, um Anzeigenvorlagen anzuzeigen. Anfragen zum smarten Zuschneiden werden jetzt für die tatsächliche Dimension des Bildes und nicht für die gesamte Vorlage gesendet. <!-- GS-6926 -->

* Lokalisierte `Zoom to fit to screen` in generierten E-Mail- und Meta-Anzeigen. <!-- GS-5063 -->

* Die [!DNL Create]-Eingabeaufforderungsschublade wird jetzt erwartungsgemäß geschlossen, wenn ein Benutzer wegklickt. <!-- GS-5254 -->

* Der Export von Meta-Anzeigen enthält jetzt wie erwartet die ausgewählte Beschriftung für Aktionsaufrufe. <!-- GS-6504 -->

* Die Markenbewertung wird jetzt aktualisiert und wie erwartet für neu generierte Erlebnisse beibehalten. <!-- GS-6535 -->

* Der HTML-Export von Meta-Anzeigen und Display-Anzeigen enthält nicht mehr Wrapper-`div` und `chrome`. <!-- GS-7116 -->

* Probleme mit dem Rendering von E-Mail-Entwürfen während der Veröffentlichung wurden jetzt behoben. <!-- GS-6394 -->

* Die Schaltfläche **[!UICONTROL Marke]** der Arbeitsfläche ist jetzt deaktiviert, wenn kein Markenwert generiert wird. <!-- GS-6429 -->

* Der Umschalter Facebook/Instagram in der Aktionsleiste der Arbeitsfläche aktualisiert jetzt das Erlebnis-Rendering wie erwartet, wenn die Einstellung Arbeitsfläche `ReadOnly` aktiviert ist. <!-- GS-7039 -->

#### Bildregenerierung

* Das Ändern der Größe mehrerer Meta- und Varianten funktioniert jetzt erwartungsgemäß. Zuvor zeigte die Arbeitsfläche keine regenerierten Varianten an, blieb aber leer. <!-- GS-7010 -->

* Die Fragmentregenerierung funktioniert jetzt für Erlebnisse in der Größe wie erwartet. <!-- GS-6836 -->

* Das erneute Generieren von Meta- und -Bildern nach der Größenanpassung führt nicht mehr zu einem Fehler. Zuvor wurden durch das Ändern der Bildgröße vor der Regenerierung die Kanalmetadaten von `meta` in `facebook` geändert. <!-- GS-7042 -->

+++

+++Anmerkungen aus dem 31.10.2024

### Neue Funktionen

* Der **[!DNL Content]** Suchfilter unterstützt jetzt die Suche nach Farb-Tag. <!-- GS-5501 -->

* Auf der **[!DNL Create]**-Arbeitsfläche wird jetzt die Zeichenanzahl für E-Mail-Fragmente angezeigt. <!-- GS-5819 -->

### Fehlerbehebungen und Verbesserungen

* Fehlende Beschriftungen für Bildschirmlesehilfen wurden zu mobilen und Desktop-`view` hinzugefügt. <!-- GS-5624 4729 -->

* Die Betreffzeile der **[!DNL Create]** Canvas-E-Mail und die Textbereiche der Pre-Header sind jetzt dynamisch in der Höhe. <!-- GS-6258 -->

* Layout-Probleme mit E-Mail-Rahmen wurden behoben. <!-- GS-6631 -->

* Der Tastaturfokus funktioniert jetzt mit der Schaltfläche **[!DNL Content]****[!UICONTROL Löschen]** wie erwartet. Zuvor konnten Benutzer nicht über die Tastatur auf diese Schaltfläche zugreifen.  <!-- GS-4065 -->

+++

+++Hinweise aus 2024.10.14 Allgemeine Verfügbarkeit

Mit dieser Version wird Adobe GenStudio for Performance Marketing eingeführt, eine generative KI-basierte Anwendung, die die Planung, Entwicklung und Analyse von Marketing-Kampagnen beschleunigt. GenStudio for Performance Marketing ermöglicht es Marketing-Teams, markeninterne, kanalübergreifende Inhalte für Anzeigen, E-Mails und Kampagnen zu erstellen und gleichzeitig Echtzeiteinblicke zu erhalten, um die Content-Performance zu optimieren.

### Funktionen

Zu den wichtigsten Produktfunktionen gehören:

**[!DNL Create]** stellt die Arbeitsfläche vor, die ein strukturiertes Eingabeerlebnis bietet, mit dem Inhaltseditoren schnell Inhalte und Varianten generieren können. Systemmanager schulen das Produkt entsprechend den Richtlinien für Unternehmensmarken. [!DNL Create] stellt sicher, dass alle mit KI generierten Inhalte mit Ihren Markenrichtlinien - Branding, Kundenrollen und Produktbeschreibungen - übereinstimmen, und optimiert die Erstellung wirkungsvoller, markenkonsistenter Marketing-Inhalte.

**[!DNL Content]** speichert kuratierte, markenkonforme genehmigte Assets und Erlebnisse. GenStudio for Performance Marketing-Anwender können genehmigte Assets einfach finden, bearbeiten, wiederverwenden und freigeben, sodass für jede Kampagne weniger Inhalte von Grund auf neu erstellt werden müssen.

**[!DNL Reviews and Approvals]** wird ein Framework eingerichtet, mit dem Stakeholder generierte Varianten überprüfen und genehmigen können, bevor sie in **[!DNL Content]** oder exportiert werden.

**[!DNL Campaigns]** organisiert und verwaltet Marketing-Kampagnen und sorgt für eine optimierte Ausführung und Nachverfolgung. Mitarbeiter können Kampagnen visualisieren, planen und verfolgen, um mehrere Initiativen effektiv zu verwalten und eine zeitnahe Bereitstellung sicherzustellen.

**[!DNL Insights]** bietet eine Echtzeit-Bewertung der Content-Performance und hilft Marketing-Experten, ihre Strategien zu optimieren und datengestützte Entscheidungen zu treffen.

GenStudio for Performance Marketing lässt sich mit anderen Adobe Experience Cloud-Produkten wie Adobe Express und Adobe AEM Assets integrieren.

+++
