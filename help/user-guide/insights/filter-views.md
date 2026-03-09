---
title: Filtern von Insights-Ansichten
description: Erfahren Sie, wie Sie die erweiterten Filterfunktionen mit Einblicken verwenden.
level: Intermediate
feature: Reporting and Insights
exl-id: fbc53c2a-388c-4b51-94e2-626cd1e18e63
TQID: https://experienceleague.adobe.com/67TI5R4hy9levkPkdXdQVCgLZl43YEq1oXV8kEEWWOs
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 855
ht-degree: 0%

---

# Filter für Insights-Ansichten

Das [!DNL Insights]-Dashboard bietet einen umfassenden Satz von Filtern für eine effiziente Datenexploration. Bei der Analyse von Kanälen, Anzeigen, Medien oder bestimmten Attributen können Sie mit den Filteroptionen Ihre Ansicht anpassen und Ihren Workflow optimieren. Verwenden Sie Keyword-Filter für eine präzise Zielgruppenbestimmung oder untersuchen Sie vordefinierte Listen, um Ihre Suche zu verfeinern und sich auf die Daten zu konzentrieren, die am wichtigsten sind.

## Grundlagen zum Filtern

Jede Ansicht in [!DNL Insights] bietet eine Liste von Filteroptionen. Der Umschalter Filter (funnel) auf der linken Seite öffnet das Menü **[!UICONTROL Filter]**. Unabhängig davon, ob Sie die Tabelle oder die Galerie anzeigen, werden angewendete Filter in der Liste **[!UICONTROL Filtern nach]** oberhalb der Tabelle oder der Galerie angezeigt. Standardmäßig werden ein Kanal und ein Konto ausgewählt.

![Filtern nach](/help/assets/insights-filter-by.png "Filtern nach"){width=600 zoomable="yes"}

Angewendete Filter bleiben über alle Ansichten hinweg erhalten. Wählen Sie **[!UICONTROL Alle löschen]** über der Tabelle oder Galerie aus, um alle ausgewählten Filter zu entfernen.

### Suchfeld

Klicken Sie auf das Suchsymbol (Lupe), um einen Suchbegriff einzugeben, um bestimmte Elemente in der Tabelle oder im Katalog zu finden. Wenn Sie beispielsweise den Begriff `Gear` in die Tabelle [!UICONTROL Anzeigen] eingeben, werden die Ergebnisse so gefiltert, dass nur Anzeigen angezeigt werden, die den im Namen `Gear` Begriff verwenden.

![Suchfeldbeispiel](/help/assets/insights-search.png "Suche nach Anzeigen mit Gear im Namen"){width=600 zoomable="yes"}

### Datumsbereich

Die Datumsbereichsauswahl ist ein leistungsstarkes Tool, um die angezeigten Daten mit Ihren Analysezielen auszurichten. Verwenden Sie die Datumsbereichsauswahl, um den Zeitrahmen für die in der Tabellen- oder Galerieansicht angezeigten Daten anzupassen. Standardmäßig ist der Datumsbereich auf die letzten 30 Tage festgelegt. Um mehr Daten einzubeziehen oder den Fokus auf einen bestimmten Zeitraum zu legen, erweitern Sie den Datumsbereich.

![Datumsbereichsauswahl](/help/assets/insights-date-range.png "Wählen Sie einen Datumsbereich aus"){width=400}

Wenn in der Tabellen- oder Galerieansicht keine Elemente angezeigt werden, kann dies daran liegen, dass der ausgewählte Datumsbereich relevante Daten ausschließt. Erhöhen Sie in solchen Fällen den Datumsbereich, um sicherzustellen, dass die gewünschten Daten enthalten sind.

### Seiten

Einige Tabellen können sich über mehrere Seiten erstrecken, wie unten in der Tabelle auf der rechten Seite dargestellt. Verwenden Sie die vielseitigen Such- und Filteroptionen, um Ihre Ergebnisse zu verfeinern. Um zwischen Seiten zu navigieren, verwenden Sie die Paginierungssteuerelemente rechts (vorwärts) und links (zurück). Stellen Sie sicher, dass Sie Filter korrekt anwenden, um alle relevanten Daten auf allen Seiten einzubeziehen.

### Schieberegler

Einige Filteroptionen beinhalten ein Schieberegler-Steuerelement, mit dem Sie einen Wert innerhalb eines definierten Bereichs auswählen können. Beispielsweise können Sie mit _[!UICONTROL Regler]_&#x200B;**[!UICONTROL Medienanzahl]** Attribute nach der Anzahl der zugehörigen Bilder oder Videos filtern. Ziehen Sie den Schieberegler, um einen Bereich festzulegen, der von mindestens 0 bis maximal 100 reicht.

## Erweiterte Filter

Mit _[!UICONTROL Kampagnen]_ und _[!UICONTROL Anzeigen]_-Filtern können Sie präzise Keywords verwenden, um die Liste zu verfeinern. Keyword-Filter sind besonders nützlich, um Kampagnen oder Anzeigen zu filtern, die eine komplexe Namenskonvention mit mehreren eindeutigen Kennungen verwenden. Ein Kampagnenname kann beispielsweise Folgendes enthalten:

- Spezifischer Regionenname oder Code: `NA`, `EMEA`
- Content-Typ-Akronyme: `EB`, `CHT` oder `DSP`
- Angebotscodes oder Akronyme: `OFFER2023`, `PROMO`

Im Laufe der Zeit kann Ihre Liste von Kampagnen und Anzeigen exponentiell wachsen. Betrachten Sie das folgende Szenario, um den Filter _[!UICONTROL Kampagnen]_ zur Verfeinerung der Tabelle [!UICONTROL Anzeigen] zu verwenden.

**So verfeinern Sie die Tabelle Anzeigen mithilfe des Filters Kampagnen**:

1. Wählen Sie _[!DNL Insights]_&#x200B;die Ansicht **[!UICONTROL Anzeigen]**&#x200B;aus.

   ![Anzeigen-Filter und &#x200B;](/help/assets/insights-ads-filter.png "-Anzeigen-Ansicht mit Filtermenü"){zoomable="yes"}

1. Klicken Sie auf den Umschalter Filter (funnel) oberhalb der linken Seite der Tabelle, um das Menü **[!UICONTROL Filter]** zu öffnen.

1. Überprüfen Sie, ob der richtige `Filter by` Kanal und das richtige Konto ausgewählt sind.

1. Erweitern Sie den Filter **[!UICONTROL Kampagnen]** und klicken Sie auf **[!UICONTROL Auswählen]**.

   ![Kampagnen filtern](/help/assets/insights-filter-campaigns-expand.png "Kampagnenfilter erweitern"){width=200}

1. Geben _[!UICONTROL im Suchfeld]_ Kampagnen auswählen“ Schlüsselwörter durch Kommas getrennt ein.

   Verwenden Sie Keywords, um Ihre Suche mit logischer und präziser Filterung zu verfeinern.

   - Um Kampagnennamen zu finden, die sowohl `adventure`- als auch **-**-`ready` enthalten, geben Sie beide Schlüsselwörter durch ein Komma getrennt ein:

     ![Alle Keywords durchsuchen](/help/assets/insights-select-campaigns-and.png "Nach Kampagnennamen suchen, die beide Keywords enthalten"){width=500}

   - Um Kampagnennamen zu finden, die entweder `adventure`- **ODER**-`ready` enthalten, geben Sie jedes Keyword separat ein:

     ![Entweder Keywords suchen](/help/assets/insights-select-campaigns-or.png "Nach Kampagnennamen suchen, die mindestens ein Keyword enthalten"){width=500}

   - Um erweiterte Suchvorgänge durchzuführen, kombinieren Sie mehrere Keyword-Sätze. Suchen Sie beispielsweise nach Kampagnennamen mit `adventure` und `apparel` **OR** `sun` und `gear`:

     ![Suche mit mehreren Keyword-Sätzen](/help/assets/insights-advanced-or.png "Suche nach Kampagnennamen mit mehreren Keyword-Sätzen"){width=500}

1. Wählen Sie in der angezeigten Suche mindestens eine Kampagne aus und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![Liste der Kampagnen](/help/assets/insights-select-campaigns-list.png "Wählen Sie die einzuschließenden Kampagnen aus")

Ihre ausgewählten Kampagnen werden jetzt in der Liste _[!UICONTROL Filtern nach]_ über der Tabelle oder der Galerie für Werbeanzeigen angezeigt. Sie können sich ausschließlich auf die Anzeigen konzentrieren, die mit den ausgewählten Kampagnen verknüpft sind. In diesem Beispiel bieten die gefilterten Ergebnisse eine zielgerichtetere Ansicht für die Analyse.

![Tabelle gefiltert nach Kampagnen](/help/assets/insights-filter-by-campaigns.png "Tabelle mit Kampagnenfilter"){zoomable="yes"}

Sie können die Tabelle [!UICONTROL Media] auf ähnliche Weise nach Anzeigenamen filtern. Erweitern Sie den Filter **[!UICONTROL Anzeigen]** und klicken Sie auf **[!UICONTROL Auswählen]**. Sie können dann einen ähnlichen Keyword-Filter durchführen, um Ihre Medientabelle oder Galerie-Ansicht zu verfeinern.

## Herunterladen von Tabellenergebnissen

Sie können die gefilterten Ergebnisse aus der Tabellenansicht zur weiteren Analyse oder Freigabe herunterladen. Klicken Sie auf das Symbol Herunterladen (Pfeil nach unten) oben rechts in der Tabelle, um eine CSV-Datei basierend auf der sichtbaren Tabelle herunterzuladen. Der Download beginnt automatisch und platziert die CSV-Datei an Ihrem standardmäßigen Download-Speicherort.

Einige Tabellen können mehrere Seiten aufweisen, die Sie unterhalb der rechten Seite der Tabelle sehen können. Die CSV-Datei enthält Daten aus _allen_ Seiten der Tabelle.
