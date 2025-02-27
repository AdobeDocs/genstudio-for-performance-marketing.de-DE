---
title: Übersicht über Erlebnisse
description: Hier erhalten Sie einen Überblick über Kundeninteraktion, Budget und Ausgaben für Erlebnisse und Anzeigenplatzierungs-Performance in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 0%

---

# Übersicht über Erlebnisse

Die [!DNL Insights] Ansicht _[!UICONTROL Erlebnisse]_ zeigt eine Liste der Erlebnisse für das verbundene Kanal-Werbekonto an. Bei Facebook sind die Erlebnisse Meta-Anzeigenamen.

{{connect-insights}}

Die _[!UICONTROL Erlebnisse]_ ist nach „Anzeigenamen. Klicken Sie auf das Symbol Einstellungen (Zahnrad) oberhalb der rechten Seite der Tabelle, um zwischen den sichtbaren Spalten umzuschalten. Das Filtersymbol (Trichter) oberhalb der linken Seite der Tabelle öffnet das Menü **[!UICONTROL Filter]**, in dem Sie aus den Listen [!UICONTROL Konto] und [!UICONTROL Kampagne] auswählen können, um die Anzeigenamen in der Tabelle zu filtern. Klicken Sie **Zurücksetzen**, um alle Filterauswahlen zu löschen.

![Erlebnisfilter und -tabelle](/help/assets/insights-experiences-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Erlebnisdetails

Ein _Erlebnis_ ist ein Werbeelement, das visuelle und interaktive Inhalte enthält, die im Rahmen einer Marketing-Kampagne an eine bestimmte Zielgruppe verteilt werden sollen.

Wählen Sie ein Erlebnis aus und zeigen Sie die Leistungsmetriken, Textattribute und Platzierungen an, die mit jeder Anzeige verknüpft sind. In der Detailansicht können Sie die Metriken eines Erlebnisses basierend auf seinen Platzierungs- und Marketing-Maßnahmen innerhalb eines bestimmten Datumsbereichs analysieren.

Die Detailansicht enthält eine Metrik mit den `click-through rate`, `cost per action` und `spend` der gesamten Anzeige, d. h. wie viel vom Budget für die Anzeige verwendet wurde. Da Anzeigen mehrere Platzierungen haben können, z. B. einen Feed oder ein Banner, können Sie für jede Anzeigenplatzierung eine Aufschlüsselung der gleichen Metriken sehen. Verwenden Sie die Pfeile nach links und rechts unter **[!UICONTROL Performance nach Anzeigenplatzierung]**, um durch die Platzierungsmetriken zu navigieren.

![Anzeigendetails mit Metriken und Anzeigenplatzierungen](/help/assets/insights-experience-details.png){zoomable="yes"}

### Textattribute

Unter der Erlebnisvorschau befindet sich eine Liste mit [!UICONTROL Textattributen] die mit der Anzeige verknüpft sind. Wenn Assets und Erlebnisse in [!DNL Content] genehmigt und gespeichert werden, generiert GenStudio for Performance Marketing Tags basierend auf ihren inhärenten Funktionen. Weitere [ zu Systemmetadaten finden Sie ](/help/user-guide/content/asset-details.md#system-metadata) „Asset-Details“.

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

## Erlebnisleistung

Mit Insights-Metriken können Sie bewerten, welche Erlebnisse zum Erfolg einer Kampagne beitragen und welche Anzeigenplatzierungen am effektivsten sind.

Die folgende Tabelle enthält Definitionen und Einblicke zu wichtigen Digital-Marketing-Metriken in der [!UICONTROL Erlebnisse]-Tabellenansicht. Jede Metrik enthält eine kurze Definition, wie sie sich auf Anzeigennamen bezieht, wie die Metrik berechnet wird, und ein oder mehrere Einblicke, die dabei helfen, ihre Bedeutung und Auswirkungen auf ein Erlebnis zu verstehen.

| Metrik | Definition | Einblick |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Erlebnisname]** | Eine Liste von Erlebnissen für das verbundene Kanalkonto. Filtern Sie Anzeigen, indem Sie eine Kampagne auswählen. | Sortieren Sie die Liste der Erlebnisse, indem Sie auf eine der Schlüsselmetriken klicken. |
| **[!UICONTROL Kampagne]** | Eine Kampagne ist eine Reihe von Erlebnissen, mit denen ein bestimmtes Ziel erreicht werden soll. | Wenn Sie die Tabelle Erlebnisse nach Kampagne filtern, können sich die Zusammenfassungsmetriken aller Erlebnisse für die Kampagne von der Zusammenfassungszeile der Kampagne in der Ansicht [!UICONTROL Kanäle] unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Platzierungen]** | Anzahl der Anzeigen [Platzierungen](#ad-placements) Standorte, an denen ein Erlebnis in der Kampagne erschienen ist. | Platzierungen erhöhen die Reichweite von Zielgruppen.<p>Anzeigen, die keine Platzierungen und keine Assets aufweisen, können auf einen [nicht unterstützten Anzeigetyp“ ](#unsupported-placements).</p> |
| **[!UICONTROL Assets]** | Die Anzahl der in der Anzeige oder dem Erlebnis verwendeten Assets. | Die Anzahl in der Tabelle Erlebnisse kann sich von der Anzahl in der Ansicht Erlebnisdetails unterscheiden. Diese Diskrepanz kann auftreten, wenn die Kanalquelle (z. B. Meta und GenStudio) geringfügig unterschiedliche Zusammenfassungsberechnungen verwendet. |
| **[!UICONTROL Impressions]** | Eine Zählung, mit der jedes Mal, wenn die Anzeigenplatzierung oder das Erlebnis im Kanal geladen wird, unabhängig von Interaktion oder Anzeige. | Eine hohe Impressionsanzahl kann auf eine breite Sichtbarkeit hinweisen, aber berücksichtigen Sie dies im Zusammenhang mit anderen Interaktionsmetriken, um echte Leistungseinblicke zu erhalten. |
| **[!UICONTROL Klicks]** | Die Häufigkeit, mit der Benutzende in einer Erlebnisplatzierung mit einem anklickbaren Element interagieren, z. B. mit einem Link oder einer Aktionsaufruf-Schaltfläche. | Eine hohe Klickanzahl zeigt ein starkes Interesse an den Inhalten und deren Interaktion mit ihnen an, was effektiv sein und die richtige Zielgruppe erreichen kann. |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Prozentsatz (%) der Impressionen, die zu Klicks auf die Erlebnisplatzierung innerhalb einer Kampagne geführt haben.<br>**Berechnung**: `clicks` geteilt durch `impressions` | Eine hohe Klickrate bedeutet, dass die Inhalte für die Zielgruppe in den Bereichen Messaging und Design hochrelevant und motivierend sind und auf die Interessen der Zielgruppe ausgerichtet sind. |
| **[!UICONTROL CPM ]**<br>_Kosten pro Tausend_ | Kosten pro 1.000 Anzeigen-Impressions für die Platzierung des Erlebnisses.<br>**Berechnung**: Gesamtbetrag `spent` durch REACH geteilt und dann mit 1000 multipliziert | Ein niedriger Wert kann auf eine kostengünstige Sichtbarkeit hinweisen, insbesondere in Verbindung mit einer hohen Clickthrough-Rate. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Durchschnittliche Kosten, die für eine bestimmte Kundenaktion ausgegeben werden, z. B. für einen Kauf oder ein Abonnement.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen | Verwenden Sie , um die Ausgaben für Erlebnisse zu überwachen, die zu wertvollen Kundenaktionen führen. |
| **[!UICONTROL CPC ]**<br>_Cost per click_ | Durchschnittliche Kosten, die mit jedem Klick in einer Erlebnisplatzierung verbunden sind.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks` | Niedrigere Durchschnittskosten können auf kosteneffiziente Werbeausgaben hindeuten, insbesondere im Vergleich zu einem Anstieg der Konversionen. |
| **[!UICONTROL Ausgaben]** | Der Betrag, der über einen bestimmten Zeitraum aus dem Kampagnenbudget ausgegeben wurde, um dieses Anzeigen-Erlebnis zu platzieren. | Ein hoher Ausgabenbetrag innerhalb eines kurzen Zeitraums kann auf eine schnelle Nutzung hindeuten, was zu einem frühzeitigen Abbau der Ressourcen führen könnte. Verfolgen Sie die Ausgaben anhand wichtiger Leistungsmetriken, um die Gesamtrendite zu überwachen. |

## Platzierungsleistung

In _Ansicht_ Erlebnisdetails“ spiegeln die drei wichtigsten Metriken die Gesamtleistung des ausgewählten Erlebnisses wider. Im Abschnitt _Performance nach Platzierung_ werden jedoch die detaillierten Metriken für jede Anzeigenplatzierung angezeigt. Navigieren Sie mit den Rechts- und Linkspfeilen durch die verschiedenen Anzeigenplatzierungen.

Die folgende Tabelle enthält Definitionen für Leistungsmetriken zur Anzeigenplatzierung:

| Metrik | Definition | Einblick |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR ]**<br>_Clickthrough-Rate_ | Der Prozentsatz (%) der Impressionen für eine einzelne Anzeigenplatzierung, die zu Klicks geführt hat.<p>**Berechnung**:`clicks` geteilt durch `impressions`<p>Diese Metrik hilft bei der Bestimmung der Effektivität der Anzeigenplatzierung, um die Zielgruppe anzusprechen. | Ein hoher CTR zeigt an, dass die Anzeigenplatzierung für die Zielgruppe relevant und überzeugend ist, was zu mehr Interaktionen führt. |
| **[!UICONTROL CPA ]**<br>_Kosten pro Aktion_ | Die durchschnittlichen Kosten, die für eine einzelne Anzeigenplatzierung aufgewendet werden, um eine gewünschte Kundenaktion zu erzielen, z. B. einen Kauf oder ein Abonnement.<p>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen<p>Diese Metrik hilft bei der Bewertung der Kosteneffizienz der Anzeigenplatzierung bei der Förderung wertvoller Aktionen. | Ein niedrigerer CPA legt nahe, dass die Anzeigenplatzierung Zielgruppeninteraktionen mit geringeren Kosten in gewünschte Aktionen umwandelt. |
| **[!UICONTROL CPC ]**<br>_Cost per click_ | Die durchschnittlichen Kosten, die mit jedem Klick in einer einzelnen Anzeigenplatzierung verbunden sind.<p>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks`<p>Diese Metrik hilft bei der Bewertung der Kosteneffizienz der Anzeigenplatzierung bei der Generierung von Klicks. | Ein niedrigerer CPC zeigt an, dass die Anzeigenplatzierung Klicks zu niedrigeren Kosten generiert, was für die Maximierung des ROI von Vorteil sein kann. |
| **[!UICONTROL Ausgaben]** | Der Betrag, der für eine einzelne Anzeigenplatzierung ausgegeben wird und einen Bruchteil der Gesamtsumme darstellt, die für das gesamte Erlebnis ausgegeben wird. Diese Metrik hilft, die Budgetzuweisung und die Ausgabeneffizienz für jede Anzeigenplatzierung zu verfolgen. | Die Überwachung der Ausgaben kann dazu beitragen, sicherzustellen, dass Ressourcen auf verschiedenen Platzierungen effektiv verwendet werden. |
