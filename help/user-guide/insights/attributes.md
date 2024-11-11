---
title: Übersicht über Attribute
description: Erfahren Sie, wie Sie die Leistung bestimmter Attribute in Adobe GenStudio for Performance Marketing bewerten.
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: d6ea1a34a8679ae958fb184e40ad0673abbab0a4
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Übersicht über Attribute

Die Ansicht [!DNL Insights] _[!UICONTROL Attribute]_ zeigt eine Liste der Attribute, die in Anzeigenkampagnen für das ausgewählte Kanalkonto verwendet werden.

Die Tabelle _[!UICONTROL Attribute]_ ist nach dem Namen [!UICONTROL Attribut] geordnet. Mit der Schaltfläche **[!UICONTROL Bilder]** und der Schaltfläche **[!UICONTROL Video]** können Sie zwischen den Listentypen umschalten. Klicken Sie auf das Einstellungssymbol (Zahnrad) rechts neben der Tabelle, um die sichtbaren Spalten umzuschalten.

Das Filtersymbol (Trichter) über der linken Seite der Tabelle öffnet das Menü **[!UICONTROL Filter]** , in dem Sie aus den Optionen [!UICONTROL Konto] und [!UICONTROL Attributkategorie] auswählen können, um die Attribute in der Tabelle zu filtern. Das folgende Beispiel zeigt eine Liste von Attributen in der Kategorie `Lighting Condition` .

![Filter und Tabelle der Attribute](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Attributdetails

Attribute helfen bei der Identifizierung von Assets anhand ihrer inhärenten Details wie Farbe, Zusammensetzung, visuelle Elemente und andere Eigenschaften.

In der Detailansicht des Attributs können Sie sehen, welche Erlebnisse das ausgewählte Attribut verwenden. Zu den Details gehören die Gesamt-Attributleistung und eine Aufschlüsselung der Leistungsmetriken für die einzelnen Erlebnisse.

![Attribute Performance metrics](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing erkennt bestimmte Funktionen und wendet das entsprechende Attribut auf ein Asset oder Erlebnis als Tag an. Unter [Kategorien](#categories) finden Sie Beispiele für diese Tags. Um alle mit einem Erlebnis verknüpften Attribute anzuzeigen, klicken Sie auf das Einstellungssymbol (Zahnrad) rechts neben der Tabelle, um die Spalte **[!UICONTROL Attribute]** auszuwählen.

## Kategorien

GenStudio for Performance Marketing erkennt bestimmte Funktionen von Bildern, Videos und Text und wendet ein Feature-Tag auf das Asset an. Eine _Kategorie_ ist eine Reihe von Funktionen, die ein bestimmtes Merkmal teilen. Beispielsweise hat die Kategorie _Bildausrichtung_ den Wert `landscape`, `portrait` oder `square`.

Sie können keine Tags bearbeiten, die erkannt und automatisch angewendet werden.

Detaillierte Listen der Bild-, Video- und Textfunktionen finden Sie unter [Attributkategorien](/help/user-guide/insights/attribute-category.md) .

## Attributleistung

Insights-Metriken können Ihnen dabei helfen, herauszufinden, welche Attribute zu mehr Kundeninteraktion beitragen.

Die folgende Tabelle enthält Definitionen und Einblicke für wichtige digitale Marketingmetriken in der Tabellenansicht [!UICONTROL Attribute]. Jede Metrik enthält eine kurze Definition, da sie sich auf ein Asset bezieht, wie die Metrik berechnet wird, und einen oder mehrere Einblicke, um deren Bedeutung und Auswirkung auf eine Anzeigenkampagne zu verstehen.

| Metrik | Definition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribut]** | Der Attributname. | Sortieren Sie die Tabelle, indem Sie für eine der Schlüsselmetriken auf die Spaltenüberschrift klicken. |
| **[!UICONTROL Kategorie]** | Die [Kategorie](#categories) , die die inhärente Qualität eines Attributs darstellt. |  |
| **[!UICONTROL Anzahl der Bilder]** | Anzahl der Bilder mit diesem Attribut. |  |
| **[!UICONTROL Anzahl der Videos]** | Anzahl der Videos mit diesem Attribut. |  |
| **[!UICONTROL Impressionen]** | Ein Zähler, der jedes Laden eines Bildes oder Videos mit diesem Attribut im Kanal zählt, unabhängig von Interaktion oder Anzeige. | Eine hohe Impressionsanzahl kann auf eine breite Sichtbarkeit hinweisen. Für echte Leistungseinblicke sollten Sie jedoch andere Interaktionsmetriken berücksichtigen. |
| **[!UICONTROL Klicks]** | Anzahl der Interaktionen von Benutzern mit einem Bild oder Video mit diesem Attribut. | Eine hohe Klickanzahl weist auf starkes Interesse und Interaktion mit dem Inhalt hin, die effektiv sein können und die richtige Zielgruppe erreichen. |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Prozentsatz (%) der Impressionen, die zu Klicks auf Bilder oder Videos mit diesem Attribut führten <br>**Berechnung**: `clicks` dividiert durch `impressions` | Eine hohe Clickthrough-Rate weist darauf hin, dass der Inhalt für die Zielgruppe in Messaging und Design hochgradig relevant und motivierend ist und effektiv auf die Interessen der Zielgruppe ausgerichtet ist. |
| **[!UICONTROL CPM ]**<br>_Kosten pro Tausend_ | Kosten für jede tausend Anzeigenimpressionen eines Bildes oder Videos mit diesem Attribut.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch Reichweite, dann multipliziert mit 1000 | Ein niedriger Wert kann auf eine kostengünstige Sichtbarkeit hinweisen, insbesondere bei Kombination mit einer hohen Clickthrough-Rate. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Durchschnittliche Kosten, die für die Erzielung einer bestimmten Kundenaktion ausgegeben werden, z. B. ein Kauf oder ein Abonnement.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen | Hilft bei der Identifizierung von Attributen, die zu wertvollen Kundenaktionen führen. |
| **[!UICONTROL CPC ]**<br>_Kosten pro Klick_ | Durchschnittliche Kosten für jeden Klick auf Bilder oder Videos mit diesem Attribut.<br>**Berechnung**: Gesamtbetrag `spent` dividiert durch `clicks` | Niedrigere Durchschnittskosten können auf kosteneffiziente Anzeigenausgaben hinweisen, insbesondere im Vergleich zu einem Anstieg der Konversionen. |
| **[!UICONTROL Spend]** | Der aus dem Budget ausgegebene Betrag in Bezug auf Attribute über einen bestimmten Zeitraum. | Ein hoher Ausgabenbetrag in kurzer Zeit kann auf eine rasche Nutzung hindeuten, was zu einer frühzeitigen Erschöpfung der Ressourcen führen könnte. Verfolgen Sie den Ausgabenbetrag im Vergleich zu den wichtigsten Leistungsmetriken, um die Gesamtrendite zu überwachen. |
