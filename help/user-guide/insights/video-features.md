---
title: Videofunktionen
description: Erfahren Sie mehr über die Videofunktion der in GenStudio for Performance Marketing verwendeten Attributkategorien.
feature: Insights, Attributes, Generative AI
source-git-commit: f8b22221f4fee0e1430740e670f580926ac33862
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 1%

---

# Videofunktionen

Videofunktionen stellen bestimmte und informative Elemente, Töne oder Muster innerhalb eines Videos zur Analyse mit [!DNL Insights] dar. Diese Funktionen helfen bei der Kategorisierung und beim Verständnis der Videoinhalte und ermöglichen genauere und detailliertere Einblicke. Durch die Identifizierung verschiedener Attribute wie Audio-Stimmung, Musikgenre und Objekte kann die KI eine umfassende Analyse des Videos bereitstellen und so zu einer besseren Entscheidungsfindung und Strategieformulierung beitragen.

## Audio-Erkennung

Die Audioerkennung in GenStudio for Performance Marketing umfasst die Analyse der Audiospur eines Videos, um verschiedene Attribute zu identifizieren. Dieser Erkennungsprozess bestimmt die allgemeine Stimmung des Audios, indem er die vorhandenen Audiotypen identifiziert, bestimmte Genres oder Musikkategorien taggt und Schlüsselwörter aus der Sprache extrahiert. Durch das Verständnis dieser Audioelemente kann die KI tiefere Einblicke in den Inhalt und Kontext des Videos bieten und so den gesamten Analyse- und Kategorisierungsprozess verbessern.

## Videofunktionen suchen

**So zeigen Sie eine Vorschau eines Videos an und hören ein Beispiel des Audioinhalts**:

1. Wählen Sie _[!DNL Insights]_die Ansicht **[!UICONTROL Attribute]**aus.

1. Ändern Sie die Tabellenansicht, indem Sie **[!UICONTROL Video]** auswählen.

1. Wählen Sie eine Funktion aus der Liste **[!UICONTROL Attributkategorie]** aus. Wählen Sie für ein Audiobeispiel **Musikgenre**.

1. Wählen Sie ein Attribut für eine detaillierte Ansicht von Videos aus, die diese Kategorie teilen.

   Beispielsweise kann die Kategorie `Music genre` als Attribut `electronic` haben.

1. Auf _Seite „Attributdetails_ werden alle Videos mit diesem Attribut aufgelistet. Halten Sie den Mauszeiger über ein beliebiges Video in der Liste, um eine Videovorschau zu starten.

1. Schalten Sie die Schaltfläche **Stummschaltung aufheben** (in der linken unteren Ecke einer Videovorschau) um und hören Sie sich das Audio der Videovorschau an.

In der folgenden Tabelle sind die Videofunktionskategorien aufgeführt, die von der GenStudio for Performance Marketing-KI erkannt werden. Die Liste der erkannten Attribute für ein Asset ist nicht vollständig. Assets, die einen umfangreichen Funktionssatz enthalten, kann auf die drei dominantesten Funktionen beschränkt sein, die von der KI identifiziert werden.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategorie | Beschreibung | Beispiel |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Audiomodus | Bestimmt den emotionalen Gesamtton oder die Atmosphäre der Audiospur, z. B. `calm`, `upbeat` oder `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Audiotypen | Taggt das Video mit einem oder mehreren vorhandenen Audiotypen, z. B. `music` oder `speech`. | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Kategorien | Klassifiziert das Video in eine oder mehrere Kategorien. | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| Musikkategorie | Grobe Klassifizierung des Musikgenres, wenn Musik im Video vorhanden ist. Dies hilft bei der Identifizierung des allgemeinen Musiktyps, wie `contemporary` oder `traditional`. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Musikgenre | Spezifische Klassifizierung des Musikstils, wenn Musik im Video vorhanden ist, die eine detailliertere Identifizierung der Musik ermöglicht, z. B. `electronic` oder `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Objekte | Identifiziert ein oder mehrere Elemente, Entitäten und Elemente, die im Video angezeigt werden. | Werte sind zu zahlreich, aber einige Beispiele sind: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Ausrichtung | Die Ausrichtung des Videos in Bezug auf seine Breite und Höhe. Ermittelt, ob er breiter ist als er hoch ist (Querformat), größer als er breit ist (Hochformat) oder gleich in Breite und Höhe (Quadrat). | `landscape`, `portrait`, `square` |
| Personen | Wenn mindestens eine Person vorhanden ist, können ein oder mehrere Attribute die Person(en) beschreiben, die im Video vorhanden sind. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Szenen | Identifiziert die Einstellung oder Umgebung innerhalb eines Videos und gibt den Kontext an, wo das Video erstellt wurde, oder den Typ des gezeigten Standorts. | Werte sind zu zahlreich, aber einige Beispiele sind: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge` |
| Stile | Erkennt visuelle Behandlungen, die auf Videoelemente angewendet werden, z. B. die in After Effects oder Lightroom verwendeten. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Tags | Erkennt andere Videoeigenschaften, die nicht unter eine bestimmte Klassifizierung fallen. Tags bieten zusätzlichen Kontext und Metadaten zum Video. | Zu viele Werte, aber einige Beispiele sind: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing` |
