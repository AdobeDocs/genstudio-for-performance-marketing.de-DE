---
title: Versionshinweise zu Adobe GenStudio for Performance Marketing
description: Erfahren Sie mehr über die neuesten Funktionen und Verbesserungen von Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substantial-update: 2024-11-14T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 2%

---

# Versionshinweise zu GenStudio for Performance Marketing

Diese Versionsinformationen enthalten die neuesten Aktualisierungen der GenStudio for Performance Marketing-Anwendung.

## 2024.11.14 {#latest}

### Neue Funktionen

Unterstützung für Rich-Media-Vorlagen hinzugefügt, sodass Kunden Assets wiederverwenden können, die bereits über ihre eigenen verwalteten Inhaltskanäle veröffentlicht wurden. <!-- GS-6107 -->

### Fehlerbehebungen und Verbesserungen

* Wenn die Größe in einem anderen Browser als dem zum Generieren des anfänglichen Inhalts verwendeten geändert wird, werden Entwürfe jetzt erwartungsgemäß geladen. <!-- GS-7204 -->

* Alle Zeichen werden jetzt in exportierter HTML korrekt dargestellt. <!-- GS-7246 -->

* Die Schaltflächen im Popup [!DNL Content] _Erlebnisse_ **[!UICONTROL Exportieren]** sind in bestimmten Sprachen nicht mehr abgeschnitten. <!-- GS-6873 -->

* Display-Anzeigen, die mit Vorlagen mit einer Größe von 50 x 50 erstellt wurden, werden jetzt in die erwartete Bildgröße exportiert. Zuvor wurden PNG-Dateien mit doppelt so großen Dimensionen exportiert. <!-- GS-7192 -->

* Vorlagenfehler, die beim Ändern der Größe von Display-Anzeigen aufgetreten sind, wurden jetzt behoben. <!-- GS-7322 -->

### Lokalisierung

Diese Version enthält Verbesserungen der Lokalisierung in der gesamten Benutzeroberfläche, einschließlich:

* Alle Zeichenfolgen im Popup [!DNL Content] _Asset hochladen_ sind jetzt korrekt lokalisiert. <!-- GS-6872 6770 -->
* Alle QuickInfos im Feld [!DNL Content] _Assets_ view **[!UICONTROL Search]** sind lokalisiert. <!-- GS-6879 -->
* Wenn ein vorhandenes Bild in einer E-Mail-Variante auf der Arbeitsfläche [!DNL Create] ersetzt wird, ist die Ansicht _Aus Inhalt auswählen_ jetzt lokalisiert. <!-- GS-6906 -->

## Frühere Versionshinweise

+++ Anmerkungen aus dem Jahr 2024.11.07

### Fehlerbehebungen und Verbesserungen

* Der Spinner _In Bearbeitung speichern_ wird nicht mehr angezeigt, wenn ein Benutzer auf **[!UICONTROL Neues Bild hochladen]** klickt und den Vorgang dann abbricht, bevor der Upload abgeschlossen ist. <!-- GS-6780 -->

* Erlebnistitel werden jetzt bei der Erlebnisregenerierung korrekt erstellt. <!-- GS-7006 -->

* Probleme mit flackernden Bildlaufleisten beim Laden von Entwürfen wurden behoben. <!-- GS-5587 -->

* Der Link `View documentation` im Popup [!DNL Content] _Genehmigte Vorlage hinzufügen_ funktioniert jetzt erwartungsgemäß. <!-- GS-6881 -->

* Das Löschen eines Bildes aus der Eingabeaufforderung während eines Größenvorgangs führt nicht mehr zu einem Fehler. <!-- GS-7115 7009 -->

* Die Auswahl von **[!UICONTROL Löschen]** aus dem Aktionsmenü (...) von [!DNL Create] funktioniert jetzt erwartungsgemäß. <!-- GS-6871 -->

* Benutzer können jetzt alle interaktiven Elemente der Meta-Anzeigenvorlage über die Tastatur steuern. <!-- GS-4066 -->

* Die Extraktion von Bilddimensionen aus Vorlagenbildfeldern wurde zu Anzeigenvorlagen hinzugefügt. Anforderungen für smartes Zuschneiden werden jetzt für die tatsächliche Dimension des Bildes und nicht für die gesamte Vorlage gesendet. <!-- GS-6926 -->

* Die Zeichenfolge `Zoom to fit to screen` wurde in generierten E-Mail- und Metaanzeigen lokalisiert. <!-- GS-5063 -->

* Die Eingabeaufforderung [!DNL Create] wird jetzt wie erwartet geschlossen, wenn ein Benutzer auf &quot;Entfernen&quot;klickt. <!-- GS-5254 -->

* Der Export von Meta-Anzeigen enthält jetzt die ausgewählte Aktionsaufruf-Beschriftung wie erwartet. <!-- GS-6504 -->

* Die Markenbewertung wird jetzt aktualisiert und für neu generierte Erlebnisse erwartungsgemäß beibehalten. <!-- GS-6535 -->

* Der HTML-Export von Meta-Anzeigen und Display-Anzeigen umfasst keine Wrapper-Elemente `div` und `chrome` mehr. <!-- GS-7116 -->

* Probleme mit dem Rendering von E-Mail-Entwürfen während der Veröffentlichung wurden jetzt behoben. <!-- GS-6394 -->

* Die Schaltfläche &quot;Arbeitsfläche **[!UICONTROL Marke]**&quot;ist jetzt deaktiviert, wenn kein Markenwert generiert wird. <!-- GS-6429 -->

* Mit dem Umschalter Facebook/Instagram in der Aktionsleiste Arbeitsfläche werden Erlebnisrenderungen jetzt wie erwartet aktualisiert, wenn die Einstellung `ReadOnly` Arbeitsfläche aktiviert ist. <!-- GS-7039 -->

#### Bildregeneration

* Die Größenanpassung mehrerer Meta-Anzeigenvarianten funktioniert jetzt erwartungsgemäß. Zuvor wurden auf der Arbeitsfläche keine regenerierten Varianten angezeigt, aber leer geblieben. <!-- GS-7010 -->

* Die Neuerstellung von Fragmenten funktioniert jetzt bei in der Größe angepassten Erlebnissen erwartungsgemäß. <!-- GS-6836 -->

* Das Regenerieren von Meta-Anzeigenbildern nach der Größenanpassung führt nicht mehr zu einem Fehler. Zuvor wurden durch die Größenanpassung von Bildern vor der Neuerstellung die Kanalmetadaten von `meta` in `facebook` <!-- GS-7042 --> geändert.

+++

+++ Anmerkungen aus dem Jahr 2024.10.31

### Neue Funktionen

* Der Suchfilter **[!DNL Content]** unterstützt jetzt die Suche nach dem Farbtag. <!-- GS-5501 -->

* Die Arbeitsfläche **[!DNL Create]** zeigt jetzt die Zeichenanzahl für E-Mail-Fragmente an. <!-- GS-5819 -->

### Fehlerbehebungen und Verbesserungen

* Zu den Elementen für Mobilgeräte und Desktop wurden fehlende Bildschirmlesehilfen-Beschriftungen hinzugefügt: `view` <!-- GS-5624 4729 -->

* Die Bereiche für die E-Mail-Betreffzeile **[!DNL Create]** und den Text vor der Kopfzeile sind jetzt dynamisch in der Höhe. <!-- GS-6258 -->

* Layout-Probleme mit E-Mail-Rahmen wurden behoben. <!-- GS-6631 -->

* Der Tastaturfokus funktioniert jetzt wie erwartet auf der Schaltfläche **[!DNL Content]** **[!UICONTROL Löschen]** . Zuvor konnte diese Schaltfläche nicht über die Tastatur erreicht oder bedient werden.  <!-- GS-4065 -->

## Allgemeine Verfügbarkeit 2024.10.14 - Version

Mit dieser Version wird Adobe GenStudio for Performance Marketing eingeführt, eine generative KI-basierte Anwendung, die die Planung, Entwicklung und Analyse von Marketingkampagnen beschleunigt. GenStudio for Performance Marketing ermöglicht es Marketingteams, markenübergreifende Inhalte für Anzeigen, E-Mails und Kampagnen mit mehreren Kanälen zu erstellen und gleichzeitig Echtzeiteinblicke zur Optimierung der Inhaltsleistung bereitzustellen.

### Funktionen

Zu den wichtigsten Produktfunktionen gehören:

**[!DNL Create]** führt die Arbeitsfläche ein, die ein strukturiertes Aufforderungserlebnis bietet, mit dem Inhaltseditoren schnell Inhalte und Varianten generieren können. Systemmanager schulen das Produkt nach Richtlinien für Unternehmensmarken. [!DNL Create] stellt sicher, dass alle von KI generierten Inhalte mit Ihren Markenrichtlinien übereinstimmen - Branding, Kundenrollen und Produktbeschreibungen - und optimiert die Produktion von wirkungsvollen, markenkonsistenten Marketinginhalten.

**[!DNL Content]** speichert kuratierte, markenkonforme genehmigte Assets und Erlebnisse. GenStudio for Performance Marketing-Benutzer können problemlos genehmigte Assets finden, bearbeiten, wiederverwenden und freigeben, sodass Inhalte für jede Kampagne nicht von Grund auf neu erstellt werden müssen.

**[!DNL Reviews and Approvals]** legt ein Framework für Stakeholder fest, um generierte Varianten zu überprüfen und zu genehmigen, bevor sie in **[!DNL Content]** gespeichert oder exportiert werden.

**[!DNL Campaigns]** organisiert und verwaltet Marketing-Kampagnen und sorgt so für eine optimierte Ausführung und Verfolgung. Mitwirkende können Kampagnen visualisieren, planen und verfolgen, um mehrere Initiativen effektiv zu verwalten und eine zeitnahe Bereitstellung zu gewährleisten.

**[!DNL Insights]** bietet eine Echtzeitbewertung der Inhaltsleistung, die Marketing-Experten dabei unterstützt, ihre Strategien zu optimieren und datenbasierte Entscheidungen zu treffen.

GenStudio for Performance Marketing kann mit anderen Adobe Experience Cloud-Produkten integriert werden, einschließlich Adobe Expreß und Adobe AEM Assets.

+++
