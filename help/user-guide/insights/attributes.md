---
title: Attributübersicht
description: Erfahren Sie, wie Sie die Leistung bestimmter Attribute in Adobe GenStudio for Performance Marketing bewerten.
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Attributübersicht

Die [!DNL Insights] Ansicht _[!UICONTROL Attribute]_ zeigt eine Liste der Attribute an, die in Anzeigenkampagnen für das ausgewählte Kanalkonto verwendet werden.

{{connect-insights}}

Die _[!UICONTROL Attribute]_ ist unter Verwendung des Namens [!UICONTROL Attribut] organisiert. Sie können mithilfe der Schaltfläche (Bilder **[!UICONTROL und der Schaltfläche (Video]** zwischen **[!UICONTROL Listentypen]**. Klicken Sie auf das Symbol Einstellungen (Zahnrad) oberhalb der rechten Seite der Tabelle, um zwischen den sichtbaren Spalten umzuschalten.

Das Filtersymbol (Trichter) oberhalb der linken Seite der Tabelle öffnet das Menü **[!UICONTROL Filter]**, in dem Sie aus den Kategorien [!UICONTROL Konto] und [!UICONTROL Attribut] auswählen können, um die Attribute in der Tabelle zu filtern. Das folgende Beispiel zeigt eine Liste von Attributen in der Kategorie `Lighting Condition`. Klicken Sie **Zurücksetzen**, um alle Filterauswahlen zu löschen.

![Attributfilter und -tabelle](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Attributdetails

Attribute helfen dabei, Assets anhand ihrer inhärenten Details wie Farbe, Komposition, visuelle Elemente und andere Eigenschaften zu identifizieren.

In der Attributdetailansicht können Sie sehen, welche Erlebnisse das ausgewählte Attribut verwenden. Zu den Details gehören die Gesamtleistung der Attribute und eine Aufschlüsselung der Leistungsmetriken für die einzelnen Erlebnisse.

![Attributleistungsmetriken](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing erkennt bestimmte Funktionen und wendet das entsprechende Attribut als Tag auf ein Asset oder ein Erlebnis an. Unter [Kategorien](#categories) finden Sie Beispiele für diese Tags. Um alle mit einem Erlebnis verknüpften Attribute anzuzeigen, klicken Sie auf das Symbol Einstellungen (Zahnrad) oben rechts in der Tabelle, um die Spalte **[!UICONTROL Attribute]** auszuwählen.

## Kategorien

Eine Attributkategorie ist eine Klassifizierungsgruppe, die verwandte Attribute organisiert, die ein gemeinsames Merkmal aufweisen. Diese Kategorien helfen, die Erkennung, Identifizierung und das Verständnis bestimmter Attribute zu optimieren, indem sie einen größeren Kontext bieten und ihre Anwendung und Verwendung erleichtern.

GenStudio for Performance Marketing nutzt die KI- und maschinellen Lernfunktionen von Adobe zum Untersuchen [Bilder](image-features.md), [Videos](video-features.md) und zum Anwenden von [!UICONTROL Asset-Attributen] auf der Grundlage einer Korrektheitswahrscheinlichkeit.

Die Liste der erkannten Attribute für ein Asset ist nicht vollständig. Assets, die einen umfangreichen Funktionssatz enthalten, kann auf die drei dominantesten Funktionen beschränkt sein, die von der KI identifiziert werden. Die folgende Abbildung enthält beispielsweise mehrere erkannte Bildattribute, einschließlich mehrerer Objekte, Vordergrund- und Hintergrundfarben.

![Bild-Asset-Attribute](/help/assets/category/asset-attributes.png "Bild von Toucan enthält mehrere erkannte Attribute"){width="300" zoomable="yes"}

>[!INFO]
>
>Sie können Tags, die erkannt und automatisch angewendet werden, nicht bearbeiten.

## Attributleistung

Insights-Metriken können Ihnen dabei helfen zu bewerten, welche Attribute zu mehr Kundeninteraktion inspirieren.

Die folgende Tabelle enthält Definitionen und Einblicke zu wichtigen digitalen Marketing-Metriken in der [!UICONTROL Attribute]-Tabellenansicht. Jede Metrik enthält eine kurze Definition, wie sie sich auf ein Asset bezieht, wie die Metrik berechnet wird und ein oder mehrere Einblicke, die dabei helfen, ihre Bedeutung und Auswirkung auf eine Anzeigenkampagne zu verstehen.

| Metrik | Definition | Einblick |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribut]** | Der Attributname. | Sortieren Sie die Tabelle, indem Sie auf die Spaltenüberschrift für eine der Schlüsselmetriken klicken. |
| **[!UICONTROL Kategorie]** | Die [Kategorie](#categories) die die inhärente Qualität eines Attributs darstellt. |  |
| **[!UICONTROL Anzahl der Bilder]** | Die Anzahl der Bilder mit diesem Attribut. | Die Anzahl in der Tabelle Attribute kann sich von der Anzahl in der Ansicht Attributdetails unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Anzahl der Videos]** | Die Anzahl der Videos mit diesem Attribut. | Die Anzahl in der Tabelle Attribute kann sich von der Anzahl in der Ansicht Attributdetails unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Impressions]** | Eine Zählung, mit der jedes Mal, wenn ein Bild oder Videos mit diesem Attribut im Kanal geladen wird, unabhängig von Interaktion oder Anzeige. | Eine hohe Impressionsanzahl kann auf eine breite Sichtbarkeit hinweisen, aber berücksichtigen Sie dies im Zusammenhang mit anderen Interaktionsmetriken, um echte Leistungseinblicke zu erhalten. |
| **[!UICONTROL Klicks]** | Die Häufigkeit, mit der Benutzende mit einem Bild oder Video mit diesem Attribut interagieren. | Eine hohe Klickanzahl zeigt ein starkes Interesse an den Inhalten und deren Interaktion mit ihnen an, was effektiv sein und die richtige Zielgruppe erreichen kann. |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Prozentsatz (%) der Impressionen, die zu Klicks auf Bilder oder Videos mit diesem Attribut geführt haben.<br>**Berechnung**: `clicks` geteilt durch `impressions` | Eine hohe Klickrate bedeutet, dass die Inhalte für die Zielgruppe in den Bereichen Messaging und Design hochrelevant und motivierend sind und auf die Interessen der Zielgruppe ausgerichtet sind. |
| **[!UICONTROL CPM ]**<br>_Kosten pro Tausend_ | Kosten für alle eintausend Anzeigen-Impressionen eines Bildes oder Videos mit diesem Attribut.<br>**Berechnung**: Gesamtbetrag `spent` durch REACH geteilt und dann mit 1000 multipliziert | Ein niedriger Wert kann auf eine kostengünstige Sichtbarkeit hinweisen, insbesondere in Verbindung mit einer hohen Clickthrough-Rate. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Durchschnittliche Kosten, die für eine bestimmte Kundenaktion ausgegeben werden, z. B. für einen Kauf oder ein Abonnement.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen | Hilft bei der Identifizierung von Attributen, die zu wertvollen Kundenaktionen führen. |
| **[!UICONTROL CPC ]**<br>_Cost per click_ | Durchschnittliche Kosten für jedes Klickereignis auf Bilder oder Videos mit diesem Attribut.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks` | Niedrigere Durchschnittskosten können auf kosteneffiziente Werbeausgaben hindeuten, insbesondere im Vergleich zu einem Anstieg der Konversionen. |
| **[!UICONTROL Ausgaben]** | Der aus dem Budget ausgegebene Betrag, da er sich auf Attribute über einen bestimmten Zeitraum bezieht. | Ein hoher Ausgabenbetrag innerhalb eines kurzen Zeitraums kann auf eine schnelle Nutzung hindeuten, was zu einem frühzeitigen Abbau der Ressourcen führen könnte. Verfolgen Sie die Ausgaben anhand wichtiger Leistungsmetriken, um die Gesamtrendite zu überwachen. |
