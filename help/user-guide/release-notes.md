---
title: Versionshinweise zu Adobe GenStudio for Performance Marketing
description: Erfahren Sie mehr über die neuesten Funktionen und Verbesserungen von Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
source-git-commit: b502e0a558cbc26c70d813938734a2f6f230dc8e
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 3%

---

# Versionshinweise zu GenStudio for Performance Marketing

Diese Versionsinformationen enthalten die neuesten Aktualisierungen der GenStudio for Performance Marketing-Anwendung.

## 2024.11.07 {#latest}

### Fehlerkorrekturen

* Der Spinner _In Bearbeitung speichern_ wird nicht mehr angezeigt, wenn ein Benutzer auf **[!UICONTROL Neues Bild hochladen]** klickt und den Vorgang dann abbricht, bevor der Upload abgeschlossen ist. <!-- GS-6780 -->

* Erlebnistitel werden jetzt bei der Erlebnisregenerierung korrekt erstellt. <!-- GS-7006 -->

* Probleme mit flackernden Bildlaufleisten beim Laden von Entwürfen wurden behoben. <!-- GS-5587 -->

* Der Link `View documentation` im Popup [!DNL Content] _Genehmigte Vorlage hinzufügen_ funktioniert jetzt erwartungsgemäß. <!-- GS-6881 -->

* Das Löschen eines Bildes aus der Eingabeaufforderung während eines Größenvorgangs führt nicht mehr zu einem Fehler. <!-- GS-7115 7009 -->

* Die Auswahl von **[!UICONTROL Löschen]** aus dem Aktionsmenü (...) von [!DNL Create] funktioniert jetzt erwartungsgemäß. <!-- GS-6871 -->

* Benutzer können jetzt alle interaktiven Elemente der Meta-Anzeigenvorlage über die Tastatur steuern. <!-- GS-4066 -->

* Extraktion von Bilddimensionen aus Vorlagenbildfeldern zur Anzeige von Anzeigenvorlagen hinzugefügt. Anforderungen für smartes Zuschneiden werden jetzt für die tatsächliche Dimension des Bildes und nicht für die gesamte Vorlage gesendet. <!-- GS-6926 -->

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

## 2024.10.31

### Neue Funktionen

* Der Suchfilter **[!DNL Content]** unterstützt jetzt die Suche nach dem Farbtag. <!-- GS-5501 -->

* Die Arbeitsfläche **[!DNL Create]** zeigt jetzt die Zeichenanzahl für E-Mail-Fragmente an. <!-- GS-5819 -->

### Fehlerkorrekturen

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

### Weitere Informationen

Weitere Informationen finden Sie in den folgenden hilfreichen Ressourcen:

* [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [Adobe GenStudio Academy](genstudioacademy.md), Online-Lernplattform für die Nutzung generativer KI-Technologien im Kreativprozess. [Registrieren Sie sich für die GenStudio Academy](http://adobe.ly/genstudioacademyregistration).
