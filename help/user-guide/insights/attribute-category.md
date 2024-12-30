---
title: Attributkategorien
description: Erfahren Sie mehr über die in GenStudio for Performance Marketing verwendeten Attributkategorien.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
last-substantial-update: 2024-11-11T00:00:00Z
exl-id: c3b51ef2-56ac-4dd8-98b7-79185b5998d0
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 2%

---

# Attributkategorien

Eine Attributkategorie ist eine Klassifizierungsgruppe, die verwandte Attribute organisiert, die ein gemeinsames Merkmal aufweisen. Diese Kategorien helfen, die Erkennung, Identifizierung und das Verständnis bestimmter Attribute zu optimieren, indem sie einen größeren Kontext bieten und ihre Anwendung und Verwendung erleichtern.

GenStudio for Performance Marketing verwendet KI-Funktionen von Adobe und maschinelles Lernen, um Bilder, Videos und Texte zu untersuchen und [!UICONTROL Asset-Attribute] basierend auf einer Korrektheitswahrscheinlichkeit anzuwenden. Die Attributliste eines Assets ist nicht vollständig. Assets, die einen umfangreichen Funktionssatz enthalten, kann auf die drei dominantesten Funktionen beschränkt sein, die von der KI identifiziert werden.

## Bildfunktionen

Bildfunktionen stellen bestimmte und informative Elemente oder Muster innerhalb eines Bildes dar, die für die Analyse mit [!DNL Insights] verwendet werden. In der folgenden Tabelle sind die Bildfunktionskategorien aufgeführt, die von der GenStudio for Performance Marketing-KI erkannt werden.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategorie | Beschreibung | Beispiel |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Kamerawinkel | Die Position und der Winkel der Kamera relativ zum Motiv. |                                                                                                                                                                                |
| Entfernung des Objekts | Der Abstand zwischen der Kamera und dem Motiv eines Bildes. | `close up`, `mid shot`, `long shot` |
| Kameraeinstellung | Die Konfiguration der Kamerasteuerung zur Erzeugung des Bildes. |                                                                                                                                                                                |
| Farbe und Ton | Wertet die in Bildelementen verwendeten Farben aus. Identifiziert ein bis drei Farben aus einem Satz von 40 vordefinierten Farben in den folgenden Bildebenen:<br>**[!UICONTROL Vordergrundfarben ]**-Elemente in der Vorderschicht des Bildes<br>**[!UICONTROL Hintergrundfarben]**-Elemente in der Hinterschicht eines Bildes<p>**[!UICONTROL Farbtemperatur]** beschreibt die allgemeine Wärme oder Kälte von Farben im Bild.<br>Ton- oder Temperaturwerte: `warm`, `cool`, `neutral` | ![Farben und kühle Töne](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Bildstil | Die visuelle Behandlung eines Bildes. |                                                                                                                                                                                |
| Beleuchtungsbedingung | Die Art des Lichts in einem Bild. |                                                                                                                                                                                |
| Objekte | Identifiziert ein oder mehrere Elemente, Entitäten und Elemente, aus denen das Bild besteht. | ![Sonnenblume, Ebene, Blumenobjekt](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Ausrichtung | Die Position des Bildes relativ zum Seitenverhältnis. | `landscape`, `portrait`, `square` |
| Personen | Wenn mindestens eine Person vorhanden ist, können ein oder mehrere Attribute die Person(en) im Bild beschreiben. | ![Frau Person tanzt](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Genres der Fotografie | Erkennt das Motiv und die Technik, mit der ein Bild erfasst wird, z. B. `abstract` oder `landscape` (nicht identisch mit der Querformat-Ausrichtung). |           |
| Szenen | Erkennt die in einem Bild dargestellte Einstellung oder Umgebung. |                                             |
| Tags | Erkennt Objekte, Elemente und andere Bildmerkmale, die nicht unter eine bestimmte Klassifizierung fallen. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Videofunktionen

Bildfunktionen stellen bestimmte und informative Elemente, Töne oder Muster innerhalb eines Videos zur Analyse mit [!DNL Insights] dar. In der folgenden Tabelle sind die Videofunktionskategorien aufgeführt, die von der GenStudio for Performance Marketing-KI erkannt werden.

| Kategorie | Beschreibung | Beispiel |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Audiogenre | Wenn Musik vorhanden ist, erhält das Video möglicherweise eine Klassifizierung des Musikstils, z. B. `electronic` oder `classical`. |          |
| Genre-Kategorie | Wenn Musik vorhanden ist, erhält das Video möglicherweise eine breite Klassifizierung des Musikgenres, z. B. `acoustic` oder `traditional`. |          |
| Audiomodus | Beschreibt die allgemeine Atmosphäre oder den Ton des Audios, z. B. `relaxing` oder `energetic`. |          |
| Audiotypen | Wenn Audio vorhanden ist, empfängt das Video möglicherweise ein -Tag für einen oder mehrere Audiotypen, z. B. `music` oder `speech`. |          |
| Objekte | Identifiziert ein oder mehrere Elemente, Entitäten und Elemente, die im gesamten Video angezeigt werden. | ![Objekte im Video](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Ausrichtung | Die Position des Videos im Verhältnis zum Seitenverhältnis des Bildes. | `landscape`, `portrait`, `square` |
| Personen | Wenn mindestens eine Person vorhanden ist, können ein oder mehrere Attribute die Person(en) im Video beschreiben. |        |
| Szenen | Die Einstellung oder Umgebung, die im Video dargestellt wird. |        |
| Stile | Erkennt visuelle Behandlungen, die auf Elemente im Video angewendet werden, z. B. `matte` oder `neon`. |        |
| Tags | Erkennt Objekte, Elemente und andere Videoeigenschaften, die nicht unter eine bestimmte Klassifizierung fallen. |        |

## Textfunktionen

Zu den Textfunktionen gehören Zählungen für bestimmte Textelemente wie Wörter, Sätze, Emojis und Klassifizierungen für Semantik, Emotion und Ton, die für die Analyse mit [!DNL Insights] verwendet werden. Text kann auch einen Lesbarkeitswert erhalten. Bald verfügbar.

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
