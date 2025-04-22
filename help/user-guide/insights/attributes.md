---
title: Attributübersicht
description: Erfahren Sie, wie Sie die Leistung bestimmter Attribute in Adobe GenStudio for Performance Marketing bewerten.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: a7241193b38a45dbd927269d65c1edac05cab002
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Attributübersicht

Die [!DNL Insights] Ansicht _[!UICONTROL Attribute]_ zeigt eine Liste der Attribute an, die in Anzeigenkampagnen für das ausgewählte Kanalkonto verwendet werden.

{{connect-insights}}

Die _[!UICONTROL Attribute]_ ist unter Verwendung des Namens [!UICONTROL Attribut] organisiert. Sie können mithilfe der Schaltfläche (Bilder **[!UICONTROL und der Schaltfläche (Video]** zwischen **[!UICONTROL Listentypen]**. Klicken Sie auf das Symbol Einstellungen (Zahnrad) oberhalb der rechten Seite der Tabelle, um zwischen den sichtbaren Spalten umzuschalten.

Mit dem Filtersymbol (Trichter) oberhalb der linken Seite der Tabelle wird das Menü **[!UICONTROL Filter]** geöffnet, in dem Sie aus mehreren Listen auswählen können. Wählen Sie **[!UICONTROL Alle löschen]** über der Tabelle aus, um alle Filter zu entfernen.

![Attributfilter und -tabelle](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Attributdetails

Attribute helfen dabei, [Anzeigen](ads.md#ad-details) und [Medien](media.md#media-details) anhand ihrer inhärenten Details wie Farbe, Komposition, visuelle Elemente und andere Eigenschaften zu identifizieren.

In der Attributdetailansicht können Sie sehen, welche Anzeigen das ausgewählte Attribut verwenden. Zu den Details gehören die Gesamtleistung der Attribute und eine Aufschlüsselung der Leistungsmetriken für jede Anzeige.

![Attributleistungsmetriken](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing erkennt bestimmte Funktionen und wendet das entsprechende Attribut auf Medieninhalte oder Anzeigen als Tag an. Beispiele für [ Tags finden ](#categories) unter „Kategorien“. Um alle mit einer Anzeige verknüpften Attribute anzuzeigen, klicken Sie auf das Symbol „Einstellungen“ (Zahnrad) oben rechts in der Tabelle, um die Spalte **[!UICONTROL Attribute]** auszuwählen.

## Kategorien

Ein Attribut _Kategorie_ ist eine Klassifizierungsgruppe, die verwandte Attribute organisiert, die ein gemeinsames Merkmal aufweisen. Diese Kategorien helfen, die Erkennung, Identifizierung und das Verständnis bestimmter Attribute zu optimieren, indem sie einen größeren Kontext bieten und ihre Anwendung und Verwendung erleichtern.

GenStudio for Performance Marketing nutzt die KI- und maschinellen Lernfunktionen von Adobe zum Untersuchen [Bilder](image-features.md), [Videos](video-features.md) und [Text](text-features.md) und zum Anwenden von Attributen auf Anzeigen und Medien basierend auf der Wahrscheinlichkeit der Korrektheit.

Die Liste der erkannten Attribute für Anzeigen und Medieninhalte ist nicht vollständig. Inhalte, die einen umfangreichen Satz von Funktionen enthalten, können auf die drei dominantesten Funktionen beschränkt sein, die von der KI identifiziert werden. Die folgende Abbildung enthält beispielsweise mehrere erkannte Bildattribute, einschließlich mehrerer Objekte, Vordergrund- und Hintergrundfarben:

![image attributes](/help/assets/category/asset-attributes.png "Image of Toucan enthält mehrere erkannte Attribute"){width="300" zoomable="yes"}

>[!INFO]
>
>Sie können Tags, die erkannt und automatisch angewendet werden, nicht bearbeiten.

## Attributleistung

Insights-Metriken können Ihnen dabei helfen zu bewerten, welche Attribute zu mehr Kundeninteraktion inspirieren.

Die folgende Tabelle enthält Definitionen und Einblicke zu wichtigen digitalen Marketing-Metriken in der [!UICONTROL Attribute]-Tabellenansicht. Jede Metrik enthält eine kurze Definition, wie sie sich auf Attribute bezieht, wie die Metrik berechnet wird, und ein oder mehrere Einblicke, die dabei helfen, ihre Bedeutung und Auswirkung auf eine Anzeigenkampagne zu verstehen.

| Metrik | Definition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribut]** | Der Attributname. | Sortieren Sie die Tabelle, indem Sie auf die Spaltenüberschrift für eine der Schlüsselmetriken klicken. |
| **[!UICONTROL Kategorie]** | Die [Kategorie](#categories) die die inhärente Qualität eines Attributs darstellt. |  |
| **[!UICONTROL Anzahl der Bilder]** | Die Anzahl der Bilder mit diesem Attribut. | Die Anzahl in der Tabelle Attribute kann sich von der Anzahl in der Ansicht Attributdetails unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Anzahl der Videos]** | Die Anzahl der Videos mit diesem Attribut. | Die Anzahl in der Tabelle Attribute kann sich von der Anzahl in der Ansicht Attributdetails unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Impressions]** | Eine Zählung, mit der jedes Mal, wenn ein Bild oder Videos mit diesem Attribut im Kanal geladen wird, unabhängig von Interaktion oder Anzeige. | Eine hohe Impressionsanzahl kann auf eine breite Sichtbarkeit hinweisen, aber für eine echte Leistung von insight sollten Sie sie im Zusammenhang mit anderen Interaktionsmetriken berücksichtigen. |
| **[!UICONTROL Klicks]** | Die Häufigkeit, mit der Benutzende mit einem Bild oder Video mit diesem Attribut interagieren. | Eine hohe Klickanzahl zeigt ein starkes Interesse an den Inhalten und deren Interaktion mit ihnen an, was effektiv sein und die richtige Zielgruppe erreichen kann. |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Prozentsatz (%) der Impressionen, die zu Klicks auf Bilder oder Videos mit diesem Attribut geführt haben.<br>**Berechnung**: `clicks` geteilt durch `impressions` | Eine hohe Klickrate bedeutet, dass die Inhalte für die Zielgruppe in den Bereichen Messaging und Design hochrelevant und motivierend sind und auf die Interessen der Zielgruppe ausgerichtet sind. |
| **[!UICONTROL CPM ]**<br>_Kosten pro Tausend_ | Kosten für alle eintausend Anzeigen-Impressionen eines Bildes oder Videos mit diesem Attribut.<br>**Berechnung**: Gesamtbetrag `spent` durch REACH geteilt und dann mit 1000 multipliziert | Ein niedriger Wert kann auf eine kostengünstige Sichtbarkeit hinweisen, insbesondere in Verbindung mit einer hohen Clickthrough-Rate. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Durchschnittliche Kosten, die für eine bestimmte Kundenaktion ausgegeben werden, z. B. für einen Kauf oder ein Abonnement.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen | Hilft bei der Identifizierung von Attributen, die zu wertvollen Kundenaktionen führen. |
| **[!UICONTROL CPC ]**<br>_Cost per click_ | Durchschnittliche Kosten für jedes Klickereignis auf Bilder oder Videos mit diesem Attribut.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks` | Niedrigere Durchschnittskosten können auf kosteneffiziente Werbeausgaben hindeuten, insbesondere im Vergleich zu einem Anstieg der Konversionen. |
| **[!UICONTROL Ausgaben]** | Der aus dem Budget ausgegebene Betrag, da er sich auf Attribute über einen bestimmten Zeitraum bezieht. | Ein hoher Ausgabenbetrag innerhalb eines kurzen Zeitraums kann auf eine schnelle Nutzung hindeuten, was zu einem frühzeitigen Abbau der Ressourcen führen könnte. Verfolgen Sie die Ausgaben anhand wichtiger Leistungsmetriken, um die Gesamtrendite zu überwachen. |
