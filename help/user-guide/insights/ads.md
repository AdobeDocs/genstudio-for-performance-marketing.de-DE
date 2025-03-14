---
title: Übersicht über Anzeigen und Anzeigenplatzierung
description: Hier erhalten Sie einen Überblick über Kundeninteraktion, Budget und Ausgaben für Anzeigen- und Anzeigenplatzierungs-Performance in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 9c4df8d5b9e45d0c26bee8db9085e3ad21b02742
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Übersicht über Anzeigen und Anzeigenplatzierung

Die Ansicht [!DNL Insights] _[!UICONTROL Anzeigen]_ zeigt eine Liste der Anzeigen für das verbundene Kanal-Werbekonto an. Eine _Anzeige_ ist ein Werbeelement, das visuelle und interaktive Inhalte enthält, die im Rahmen einer Marketing-Kampagne an eine bestimmte Zielgruppe verteilt werden sollen. Bei Facebook sind die Anzeigen Meta-Anzeigenamen.

{{connect-insights}}

Die _[!UICONTROL Anzeigen]_-Tabelle ist nach &quot;[!UICONTROL -Namen“ ]. Klicken Sie auf das Symbol Einstellungen (Zahnrad) oberhalb der rechten Seite der Tabelle, um zwischen den sichtbaren Spalten umzuschalten. Mit dem Filtersymbol (Trichter) oberhalb der linken Seite der Tabelle wird das Menü **[!UICONTROL Filter]** geöffnet, in dem Sie aus mehreren Listen auswählen können. Wählen Sie **[!UICONTROL Alle löschen]** über der Tabelle aus, um alle Filter zu entfernen.

![Anzeigenfilter und -tabelle](/help/assets/insights-ads-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Anzeigendetails

Wählen Sie eine Anzeige aus und zeigen Sie die Leistungsmetriken, Textattribute und Platzierungen an, die mit jeder Anzeige verbunden sind. Die _[!UICONTROL Seite „Anzeigendetails]_ enthält Metriken für die `click-through rate`, `cost per action` und `spend`, d. h. wie viel des Budgets für die Anzeige ausgegeben wurde. Da Anzeigen mehrere Platzierungen haben können, z. B. einen Feed oder ein Banner, können Sie für jede Anzeigenplatzierung eine Aufschlüsselung der gleichen Metriken sehen. Verwenden Sie die Pfeile nach links und rechts unter **[!UICONTROL Performance nach Anzeigenplatzierung]**, um durch die Platzierungsmetriken zu navigieren.

![Anzeigendetails mit Metriken und Anzeigenplatzierungen](/help/assets/insights-ad-details.png){zoomable="yes"}

### Textattribute

Unterhalb der Anzeigenvorschau befindet sich eine Liste mit [!UICONTROL Textattributen] die mit der Anzeige verknüpft sind. Wenn Assets und Anzeigen in [!DNL Content] genehmigt und gespeichert werden, generiert GenStudio for Performance Marketing Tags basierend auf ihren inhärenten Funktionen. Weitere [ zu Systemmetadaten finden Sie ](/help/user-guide/content/asset-details.md#system-metadata) „Mediendetails“.

### Platzierungen hinzufügen

Zum Zeitpunkt der Erstellung einer Kampagne mit Meta-Anzeigen haben Sie möglicherweise anhand des Kampagnenziels ausgewählt[ wo Ihre Anzeigen geschaltet ](channels.md#objectives). Anzeigenplatzierungen erweitern die Reichweite der Zielgruppe für Ihre Anzeige.

GenStudio for Performance Marketing unterstützt Anzeigenformate wie Asset-Feeds, Link-Anzeigen und Einzelbilder oder Videos. Im Folgenden finden Sie eine Liste der Anzeigenformate nach Plattform:

| Instagram | Facebook/Meta | Überbringerin | Zielgruppennetzwerk |
| ------------ | ---------------- | ------------ | ---------------- |
| Explore<br>Explore home<br>Explore grid home<br>feed<br>reels<br>profile feed<br>search<br>shop<br>storys | Business Explore<br>Feed<br>In-stream video<br>marketplace<br>reels<br>reels overlay<br>right column<br>search results<br>storys<br>video feeds<br>Anzeigen auf Facebook reels | <br> Storys | Natives Video, Banner und interstitielles <br> |

#### Nicht unterstützte Platzierungen

GenStudio for Performance Marketing unterstützt die folgenden Anzeigenplatzierungen nicht:

- Partizipativ
- Catalog/Advantage+ Katalog
- Instanzerlebnis
- Karussell

## Anzeigenleistung

Mithilfe von Insights-Metriken können Sie bewerten, welche Anzeigen zum Erfolg einer Kampagne beitragen und welche Anzeigenplatzierungen am effektivsten sind.

Die folgende Tabelle enthält Definitionen und Einblicke zu wichtigen digitalen Marketing-Metriken in der [!UICONTROL Anzeigen]-Tabellenansicht. Jede Metrik enthält eine kurze Definition, wie sie sich auf Anzeigenamen bezieht, wie die Metrik berechnet wird, und ein oder mehrere Einblicke, die dabei helfen, ihre Bedeutung und Auswirkung auf eine Anzeige zu verstehen.

| Metrik | Definition | Einblick |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Anzeigename]** | Eine Liste von Anzeigen für das verbundene Kanalkonto. Filtern Sie Anzeigen, indem Sie eine Kampagne auswählen. | Sortieren Sie die Anzeigenliste, indem Sie auf eine der Schlüsselmetriken klicken. |
| **[!UICONTROL Kampagne]** | Eine Kampagne ist ein Satz von Anzeigen, die dazu dienen, ein bestimmtes Ziel zu erreichen. | Wenn Sie die Tabelle Anzeigen nach Kampagne filtern, können sich die Zusammenfassungsmetriken aller Anzeigen für die Kampagne von der Zusammenfassungszeile der Kampagne in der Ansicht [!UICONTROL Kanäle] unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Platzierungen]** | Anzahl der Anzeigen [Platzierungen](#ad-placements), an denen eine Anzeige in der Kampagne erschienen ist. | Platzierungen erhöhen die Reichweite von Zielgruppen.<p>Anzeigen, die keine Platzierungen und keine Medien zeigen, können auf einen [nicht unterstützten Anzeigentyp](#unsupported-placements) hinweisen.</p> |
| **[!UICONTROL Media]** | Die Anzahl der in der Anzeige oder Anzeige verwendeten Assets. | Die Anzahl in der Ads-Tabelle kann sich von der Anzahl in der Ad-Detailansicht unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Impressions]** | Eine Zählung, mit der jedes Mal, wenn die Anzeigenplatzierung oder -anzeige im Kanal geladen wird, unabhängig von Interaktion oder Anzeige. | Eine hohe Impressionsanzahl kann auf eine breite Sichtbarkeit hinweisen, aber berücksichtigen Sie dies im Zusammenhang mit anderen Interaktionsmetriken, um echte Leistungseinblicke zu erhalten. |
| **[!UICONTROL Klicks]** | Die Häufigkeit, mit der Benutzende in einer Anzeigenplatzierung mit einem anklickbaren Element interagieren, z. B. mit einem Link oder einer Aktionsaufruf-Schaltfläche. | Eine hohe Klickanzahl zeigt ein starkes Interesse an den Inhalten und deren Interaktion mit ihnen an, was effektiv sein und die richtige Zielgruppe erreichen kann. |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Prozentsatz (%) der Impressionen, die innerhalb einer Kampagne zu Klicks auf die Anzeige geführt haben.<br>**Berechnung**: `clicks` geteilt durch `impressions` | Eine hohe Klickrate bedeutet, dass die Inhalte für die Zielgruppe in den Bereichen Messaging und Design hochrelevant und motivierend sind und auf die Interessen der Zielgruppe ausgerichtet sind. |
| **[!UICONTROL CPM ]**<br>_Kosten pro Tausend_ | Kosten pro tausend Anzeigen-Impressionen.<br>**Berechnung**: Gesamtbetrag `spent` durch REACH geteilt und dann mit 1000 multipliziert | Ein niedriger Wert kann auf eine kostengünstige Sichtbarkeit hinweisen, insbesondere in Verbindung mit einer hohen Clickthrough-Rate. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Durchschnittliche Kosten, die für eine bestimmte Kundenaktion ausgegeben werden, z. B. für einen Kauf oder ein Abonnement.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen | Verwenden Sie , um die Ausgaben für Anzeigen zu überwachen, die zu wertvollen Kundenaktionen führen. |
| **[!UICONTROL CPC ]**<br>_Cost per click_ | Durchschnittliche Kosten, die mit jedem Klick in einer Anzeigenplatzierung verbunden sind.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks` | Niedrigere Durchschnittskosten können auf kosteneffiziente Werbeausgaben hindeuten, insbesondere im Vergleich zu einem Anstieg der Konversionen. |
| **[!UICONTROL Ausgaben]** | Der Betrag, der über einen bestimmten Zeitraum aus dem Kampagnenbudget für die Platzierung dieser Anzeige ausgegeben wurde. | Ein hoher Ausgabenbetrag innerhalb eines kurzen Zeitraums kann auf eine schnelle Nutzung hindeuten, was zu einem frühzeitigen Abbau der Ressourcen führen könnte. Verfolgen Sie die Ausgaben anhand wichtiger Leistungsmetriken, um die Gesamtrendite zu überwachen. |

## Platzierungsleistung

Auf der _[!UICONTROL Anzeigendetailseite]_ spiegeln die drei wichtigsten Metriken die Gesamtleistung der ausgewählten Anzeige wider. Im Abschnitt _Performance nach Platzierung_ werden jedoch die detaillierten Metriken für jede Anzeigenplatzierung angezeigt. Navigieren Sie mit den Rechts- und Linkspfeilen durch die verschiedenen Anzeigenplatzierungen.

Die folgende Tabelle enthält Definitionen für Leistungsmetriken zur Anzeigenplatzierung:

| Metrik | Definition | Einblick |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Der Prozentsatz (%) der Impressionen für eine einzelne Anzeigenplatzierung, die zu Klicks geführt hat.<p>**Berechnung**:`clicks` geteilt durch `impressions`<p>Diese Metrik hilft bei der Bestimmung der Effektivität der Anzeigenplatzierung, um die Zielgruppe anzusprechen. | Ein hoher CTR zeigt an, dass die Anzeigenplatzierung für die Zielgruppe relevant und überzeugend ist, was zu mehr Interaktionen führt. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Die durchschnittlichen Kosten, die für eine einzelne Anzeigenplatzierung aufgewendet werden, um eine gewünschte Kundenaktion zu erzielen, z. B. einen Kauf oder ein Abonnement.<p>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen<p>Diese Metrik hilft bei der Bewertung der Kosteneffizienz der Anzeigenplatzierung bei der Förderung wertvoller Aktionen. | Ein niedrigerer CPA legt nahe, dass die Anzeigenplatzierung Zielgruppeninteraktionen mit geringeren Kosten in gewünschte Aktionen umwandelt. |
| **[!UICONTROL CPC ]**<br>_Cost per click_ | Die durchschnittlichen Kosten, die mit jedem Klick in einer einzelnen Anzeigenplatzierung verbunden sind.<p>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks`<p>Diese Metrik hilft bei der Bewertung der Kosteneffizienz der Anzeigenplatzierung bei der Generierung von Klicks. | Ein niedrigerer CPC zeigt an, dass die Anzeigenplatzierung Klicks zu niedrigeren Kosten generiert, was für die Maximierung des ROI von Vorteil sein kann. |
| **[!UICONTROL Ausgaben]** | Der Betrag, der für eine einzelne Anzeigenplatzierung ausgegeben wird und einen Bruchteil der Gesamtsumme darstellt, die für die gesamte Anzeige ausgegeben wird. Diese Metrik hilft, die Budgetzuweisung und die Ausgabeneffizienz für jede Anzeigenplatzierung zu verfolgen. | Die Überwachung der Ausgaben kann dazu beitragen, sicherzustellen, dass Ressourcen auf verschiedenen Platzierungen effektiv verwendet werden. |
