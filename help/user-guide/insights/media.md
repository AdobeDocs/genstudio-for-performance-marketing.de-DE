---
title: Medienübersicht
description: Erfahren Sie, wie Sie die Medienleistung in Adobe GenStudio for Performance Marketing bewerten.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: facc38b8afe8104e27a89ac3d9ec40d1209229a9
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Medienübersicht

Die [!DNL Insights] Ansicht _[!UICONTROL Medien]_ zeigt eine Liste der Medien, die in Anzeigen- und Anzeigenkampagnen für das ausgewählte Konto verwendet werden. _Media_ stellt ein Bild, Video, Text oder andere kreative Inhalte dar, die für die Verwendung in Ihren Marketing-Initiativen genehmigt wurden.

{{connect-insights}}

Die _[!UICONTROL Media]_-Tabelle ist nach **[!UICONTROL Medien-ID]** organisiert. Sie können zwischen den Ansichten wechseln, indem Sie das Symbol Liste anzeigen (Tabelle) und das Symbol Galerieansicht (Raster) verwenden. Klicken Sie auf das Symbol Einstellungen (Zahnrad) oberhalb der rechten Seite der Tabelle, um zwischen den sichtbaren Spalten umzuschalten.

![Medienfilter und -tabelle](/help/assets/insights-media-filter.png){zoomable="yes"}

Die _[!UICONTROL Media]_-Galerieansicht zeigt eine Collage aus Medienvorschauen und eine Metrik, wie z. B. die Clickthrough-Rate. Klicken Sie auf das Symbol Einstellungen (Zahnrad) oben rechts in der Galerie, um **[!UICONTROL Karteneinstellungen]** zu öffnen und eine der drei sichtbaren Metriken umzuschalten:

- CPA (Kosten pro Aktion)
- CTR (Clickthrough-Rate)
- CPC (Kosten pro Klick)
- Ausgaben

{{filter-table}}

## Mediendetails

In der Ansicht _Mediendetails_ können Sie sehen, welche Anzeigen die ausgewählten Medien verwenden. Zu den Details gehören die Gesamtleistung der Medien, Anzeigen, die die Medien verwenden, benutzerdefinierte Attribute und mit den Medien verknüpfte KI-erkannte Funktionen.

![Mediendetails](/help/assets/insights-media-details.png){zoomable="yes"}

### Medienattribute

{{$include /help/_includes/generated-attributes.md}}

## Medienleistung

Insights-Metriken können Ihnen dabei helfen zu bewerten, welche Medien zum Erfolg einer Kampagne beitragen und welche Medienattribute am effektivsten sind.

Die folgende Tabelle enthält Definitionen und Einblicke zu wichtigen Digital-Marketing-Metriken in der [!UICONTROL Media]-Tabellenansicht. Jede Metrik enthält eine kurze Definition, wie sie sich auf Medien bezieht, wie die Metrik berechnet wird und ein oder mehrere Einblicke, die dabei helfen, ihre Bedeutung und Auswirkung zu verstehen.

| Metrik | Definition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Medien-ID]** | Der mit einem Bild, Video, Text oder anderen kreativen Inhalten verknüpfte Name. | Sortieren Sie die Tabelle, indem Sie auf die Spaltenüberschrift für eine der Schlüsselmetriken klicken. |
| **[!UICONTROL Impressions]** | Eine Zählung, die anzeigt, wie oft die Medien im Kanal geladen werden, unabhängig von Interaktion oder Anzeige. | Eine hohe Impressionsanzahl kann auf eine breite Sichtbarkeit hinweisen, aber für eine echte Leistung von insight sollten Sie sie im Zusammenhang mit anderen Interaktionsmetriken berücksichtigen. |
| **[!UICONTROL Klicks]** | Die Häufigkeit, mit der Benutzende auf Medien mit einem anklickbaren Element interagieren, z. B. mit einem Link. | Eine hohe Klickanzahl zeigt ein starkes Interesse an den Inhalten und deren Interaktion mit ihnen an, was effektiv sein und die richtige Zielgruppe erreichen kann. |
| **[!UICONTROL CTR &#x200B;]**<br>_Clickthrough-Rate_ | Prozentsatz (%) der Impressionen, die zu Medienklicks innerhalb einer Anzeige geführt haben.<br>**Berechnung**: `clicks` geteilt durch `impressions` | Eine hohe Klickrate bedeutet, dass die Medien für die Zielgruppe äußerst relevant und interessant sind. Es deutet darauf hin, dass die Botschaften und das Design das Interesse der Zielgruppe effektiv wecken und sie zum Handeln auffordern. Darüber hinaus kann eine hohe CTR bedeuten, dass die Medien zielgerichtet sind und bei der gewünschten Zielgruppe Anklang finden, was zu einer besseren Gesamtleistung der Kampagne führt. |
| **[!UICONTROL CPM &#x200B;]**<br>_Kosten pro Tausend_ | Die durchschnittlichen Kosten für jeden tausend Medienimpressionen.<br>**Berechnung**: Gesamtbetrag `spent` durch die Anzahl der Impressionen geteilt und dann mit 1000 multipliziert | Ein niedriger CPM-Wert kann auf eine kostengünstige Medienleistung hinweisen, insbesondere in Verbindung mit einer hohen Clickthrough-Rate. |
| **[!UICONTROL CPA &#x200B;]**<br>_Kosten pro Aktion_ | Durchschnittliche Kosten, die für eine bestimmte Kundenaktion ausgegeben werden, z. B. für einen Kauf oder ein Abonnement.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch die Anzahl der abgeschlossenen Kundenaktionen | Hilft bei der Identifizierung von Medien, die zu wertvollen Kundenaktionen führen. |
| **[!UICONTROL CPC &#x200B;]**<br>_Cost per click_ | Durchschnittliche Kosten für jeden Klick auf das Medium.<br>**Berechnung**: Gesamtbetrag `spent` geteilt durch `clicks` | Niedrigere Durchschnittskosten können auf kosteneffiziente Werbeausgaben hindeuten, insbesondere im Vergleich zu einem Anstieg der Konversionen. |
| **[!UICONTROL Ausgaben]** | Der aus dem Budget ausgegebene Betrag, da er sich auf einzelne Medien über einen bestimmten Zeitraum bezieht. | Ein hoher Ausgabenbetrag innerhalb eines kurzen Zeitraums kann auf eine schnelle Nutzung hindeuten, was zu einem frühzeitigen Abbau der Ressourcen führen könnte. Verfolgen Sie die Ausgaben anhand wichtiger Leistungsmetriken, um die Gesamtrendite zu überwachen. |
| **[!UICONTROL Wird in diesen Anzeigen verwendet]** | Die Anzahl der Anzeigen, die diese Medien verwenden. | |
| **Attribute** | Liste der in diesem Medium vorhandenen inhärenten Funktionen. | Attribute helfen dabei, kreative Elemente zu identifizieren, die Ihre Zielgruppe am meisten ansprechen. |
