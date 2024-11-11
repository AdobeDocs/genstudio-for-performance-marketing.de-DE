---
title: Attributkategorien
description: Erfahren Sie mehr über die in GenStudio for Performance Marketing verwendeten Attributkategorien.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
source-git-commit: 3b5fc55595f766db0327b6aefb0e29c3896e00c0
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 1%

---

# Attributkategorien

Eine Attributkategorie ist eine Classification-Gruppe, die verwandte Attribute organisiert, die ein gemeinsames Merkmal aufweisen. Diese Kategorien helfen bei der Optimierung der Erkennung, Identifizierung und des Verständnisses bestimmter Attribute, indem sie einen größeren Kontext bieten und deren Anwendung und Verwendung erleichtern.

GenStudio for Performance Marketing nutzt Adobe-API- und maschinelle Lernfunktionen, um Bilder, Videos und Texte zu untersuchen und [!UICONTROL Asset] auf der Grundlage des Vertrauensgrads anzuwenden. _Konfidenz_ bezieht sich auf die Wahrscheinlichkeit, mit der die KI einer Vorhersage oder Klassifizierung zuweist. Im Kontext des maschinellen Lernens ist es eine Art Scoring, das misst, wie &quot;sicher&quot;die KI ist, dass die Classification korrekt ist. Je höher die Konfidenzauswertung, desto größer die Gewissheit. Beispielsweise kann die KI bei der Analyse eines Bildes mehrere Funktionen identifizieren und jedem einen Wert zuweisen, der angibt, wie sicher die Funktion ist. Die Attributliste eines Assets ist nicht vollständig. Assets mit einer Vielzahl von Funktionen kann auf einen Vertrauensschwellenwert beschränkt werden, wie z. B. die drei am weitesten verbreiteten Merkmale.

## Bildfunktionen

Bildfunktionen stellen eindeutige und informative Elemente oder Muster innerhalb eines Bildes dar, die für die Analyse mit [!DNL Insights] verwendet werden. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing AI erkannten Bildfunktionskategorien aufgeführt.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategorie | Beschreibung | Beispiel |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Kamerawinkel | Position und Winkel der Kamera in Bezug auf das Thema. |                                                                                                                                                                                |
| Fachweite | Die Entfernung zwischen der Kamera und dem Betreff eines Bildes. | `close up`, `mid shot`, `long shot` |
| Kameraeinstellung | Die Konfiguration der Steuerelemente der Kamera, um das Bild zu erzeugen. |                                                                                                                                                                                |
| Farbe und Ton | Wertet die in Bildelementen verwendeten Farben aus. Identifiziert eine bis drei Farben aus einem Satz von 40 vorab bestimmten Farben in den folgenden Bildebenen:<br>**[!UICONTROL Vordergrundfarben ]**- Elemente in der Vorderseite des Bildes<br>**[!UICONTROL Hintergrundfarben]** - Elemente in der Hinterschicht eines Bildes<p>**[!UICONTROL Farbtemperatur]** beschreibt die allgemeine Wärme oder Farbtiefe der Farben im Bild.<br>Ton- oder Temperaturwerte: `warm`, `cool`, `neutral` | ![Farben und coole Töne](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Bildstil | Die visuelle Behandlung eines Bildes. |                                                                                                                                                                                |
| Beleuchtungsbedingung | Die Lichtart in einem Bild. |                                                                                                                                                                                |
| Objekte | Identifiziert ein oder mehrere Elemente, Entitäten und Elemente, aus denen das Bild besteht. | ![Sonnenblumen, Ebene, Blumenobjekt](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Ausrichtung | Die Position des Bildes im Verhältnis zum Seitenverhältnis. | `landscape`, `portrait`, `square` |
| Personen | Wenn mindestens eine Person vorhanden ist, können ein oder mehrere Attribute die Person(en) im Bild beschreiben. | ![Frau, die tanzt](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Fotografiergenres | Ermittelt den Betreff und die Technik, die zum Erfassen eines Bildes verwendet werden, z. B. `abstract` oder `landscape` (nicht identisch mit der Ausrichtung im Querformat). |           |
| Szenen | Ermittelt die in einem Bild dargestellte Einstellung oder Umgebung. |                                             |
| Tags | Ermittelt Objekte, Elemente und andere Bildmerkmale, die nicht unter eine bestimmte Classification fallen. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Videofunktionen

Bildfunktionen stellen eindeutige und informative Elemente, Töne oder Muster innerhalb eines Videos zur Analyse mit [!DNL Insights] dar. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing AI erkannten Videofunktionskategorien aufgeführt.

| Kategorie | Beschreibung | Beispiel |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Audio-Genre | Wenn Musik vorhanden ist, kann das Video eine Klassifizierung des Musikstils erhalten, z. B. `electronic` oder `classical`. |          |
| Kategorie &quot;Audio-Genre&quot; | Wenn Musik vorhanden ist, kann das Video eine umfassende Klassifizierung des Musikgenres erhalten, z. B. `acoustic` oder `traditional`. |          |
| Audio-Stimmung | Beschreibt die allgemeine Atmosphäre oder den Ton des Audios, z. B. `relaxing` oder `energetic`. |          |
| Audiotypen | Wenn Audio vorhanden ist, kann das Video ein Tag für einen oder mehrere Audiotypen erhalten, z. B. `music` oder `speech`. |          |
| Objekte | Identifiziert ein oder mehrere Elemente, Entitäten und Elemente, die im Video angezeigt werden. | ![Objekte im Video](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Ausrichtung | Die Position des Videos im Verhältnis zum Seitenverhältnis des Rahmens. | `landscape`, `portrait`, `square` |
| Personen | Wenn mindestens eine Person vorhanden ist, kann eines oder mehrere Attribute die Person(en) im Video beschreiben. |        |
| Szenen | Die im Video dargestellte Einstellung oder Umgebung. |        |
| Stile | Ermittelt visuelle Behandlungen, die auf Elemente im Video angewendet werden, z. B. `matte` oder `neon`. |        |
| Tags | Ermittelt Objekte, Elemente und andere Videomerkmale, die nicht unter eine bestimmte Classification fallen. |        |

## Textfunktionen

Zu den Textfunktionen gehören Zählungen für bestimmte Textelemente wie Wörter, Sätze, Emojis und Klassifizierungen für Semantik, Emotion und Ton, die für die Analyse mit [!DNL Insights] verwendet werden. Text kann auch eine Lesbarkeit erhalten. Bald.

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
