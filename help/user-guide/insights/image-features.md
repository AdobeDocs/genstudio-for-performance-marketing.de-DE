---
title: Bildfunktionen
description: Erfahren Sie mehr über die Bildfunktion der in GenStudio for Performance Marketing verwendeten Attributkategorien.
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: 0092458ae4f7e5ca5015a5b768ecfd70f8fcd7d8
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Bildfunktionen

Bildfunktionen stellen bestimmte und informative Elemente oder Muster innerhalb eines Bildes dar, die für die Analyse mit [!DNL Insights] verwendet werden. Diese Funktionen helfen bei der Kategorisierung und dem Verständnis des visuellen Inhalts und ermöglichen genauere und detailliertere Einblicke. Durch die Identifizierung verschiedener Attribute wie Stil, Farbe und Objekte kann die KI eine umfassende Analyse des Bildes bereitstellen und so zu einer besseren Entscheidungsfindung und Strategieformulierung beitragen.

## Stilerkennung

Die Bestimmung _Bildstils_ dient als Grundlage für die Identifizierung anderer Bildmerkmale. Die KI kann die entsprechenden Analysetechniken anwenden und relevante Merkmale erkennen, was zu einem umfassenderen Verständnis des Bildes führt. Jeder Stil hat unterschiedliche visuelle Eigenschaften, die beeinflussen, wie das Bild wahrgenommen und analysiert wird.

Wenn der Bildstil als `photograph` identifiziert wird, analysiert die KI zusätzliche Eigenschaften für `camera settings`, `camera proximity` und `Photography genres`. Diese Eigenschaften sind fotografisch spezifisch und bieten tiefere Einblicke in die Zusammensetzung und Qualität des Bildes. Siehe [28 Arten von Fotografien](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) in Adobe _Fotografie lernen_ und erfahren Sie mehr über beliebte Fotografietypen und grundlegende Begriffe.

Wenn der Bildstil als `sketch` oder `digital cartoon` identifiziert wird, kann ein anderer Satz von Merkmalen relevant sein. Dieser hierarchische Ansatz stellt sicher, dass die Analyse kontextuell genau und auf den jeweiligen Bildtyp zugeschnitten ist.

## Bildsuchfunktionen

**So zeigen Sie Bilder in einer bestimmten Attributkategorie**:

1. Wählen Sie _[!DNL Insights]_die Ansicht **[!UICONTROL Attribute]**aus.

1. Ändern Sie die Tabellenansicht, indem Sie **[!UICONTROL Bilder]** auswählen.

1. Wählen Sie eine Bildfunktion aus der Liste **[!UICONTROL Attributkategorie]** aus, z. B. `Scenes`.

1. Wählen Sie ein Attribut für eine detaillierte Ansicht von Bildern aus, die diese Kategorie gemeinsam haben.

   Beispielsweise kann die Kategorie `Scenes` als Attribut `restaurant` haben.

1. Auf _Seite „Attributdetails_ werden alle Bilder mit diesem Attribut aufgelistet.

In der folgenden Tabelle sind die Bildfunktionskategorien aufgeführt, die von der GenStudio for Performance Marketing-KI erkannt werden. Die Liste der erkannten Attribute für Medieninhalte ist nicht vollständig. Medien, die einen umfangreichen Satz von Funktionen enthalten, können auf die drei dominantesten Funktionen beschränkt sein, die von der KI identifiziert werden.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategorie | Beschreibung | Beispiel |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Aufmerksamkeitsverteilung | Der Grad der Aufmerksamkeit des Betrachters, der sich über ein Bild verteilt und angibt, wie viel Fokus verschiedene Bereiche des Bildes erhalten können. Eine höhere Verteilung bedeutet, dass kein einzelner Bereich den Fokus des Betrachters dominiert, während eine niedrigere Verteilung bedeutet, dass ein oder zwei Fokuspunkte die Aufmerksamkeit des Betrachters erfassen. | `high`, `medium`, `low`<p>Beispiel für `low` Verteilung links und `high` Verteilung rechts:<p>![Niedrig- und Hochverteilungs-](/help/assets/category/image-attn-lowhigh.png " in niedriger und hoher Verteilung"){width="200" zoomable="yes"} |
| Kamerawinkel | Die Perspektive, aus der die Kamera das Motiv erfasst, was sich auf die Wahrnehmung und Interpretation des Bildes auswirkt. Wenn der Bildstil `photograph` ist, wird diese Eigenschaft identifiziert. | `Low angle`, `High angle`, `Eye level`, `Neutral angle`, `Bird's eye view`<p>Beispiel für `eye level`:<p>![Augenhöhe](/help/assets/category/image-camera-angle.png "Menschen sitzen unter verschiedenen Winkeln"){width="200" zoomable="yes"} |
| Kameraeinstellung | Spezifische Einstellungen und Konfigurationen der Kamerasteuerung, die das endgültige Erscheinungsbild und die Qualität des Bildes beeinflussen. Wenn der Bildstil `photograph` ist, wird diese Eigenschaft identifiziert. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Double-exposure`, `Macro`, `Normal mode`<p>Beispiel für eine `macro`:<p>![Makro-Nahaufnahme](/help/assets/category/image-subject-distance.png "Makroeinstellung für Nahaufnahme von Blumen und Juwelen-Bienen"){width="200" zoomable="yes"} |
| Farbe und Ton | Die Farben und tonalen Qualitäten innerhalb eines Bildes. Identifiziert bis zu drei Farben aus einem vordefinierten Satz von 40 Farben in verschiedenen Bildebenen:<p>**[!UICONTROL Vordergrundfarben]** - Farben in der Vorderebene des Bildes<br>**[!UICONTROL Hintergrundfarben ]**- Farben in der Hinterebene des Bildes | Werte: `Red`, `Dark Red`, `Bright Green`, `Light Green`, `Blue`, `Dark Blue`, `Royal Blue`, `Black`, `Silver`, `Green`, `Dark Green`, `Mud Green`, `Magenta`, `Light Blue`, `White`, `Off White`, `Gray`, `Dark Gray`, `Cream`, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink` `Dark Pink` `Maroon` `Tan` `Purple` `Lavender` `Turquoise` `Plum` `Gold` `Emerald` `Orange` `Beige` `Lilac` `Olive`, |
| Farbtemperatur | Beschreibt die allgemeine Wärme oder Kühle von Farben im Bild. | Ton- oder Temperaturwerte: `warm`, `cool`, `neutral`<br>![Farben und kühle Töne](/help/assets/category/image-color-temp.png "Farbtemperatur mit kühlem Hintergrund und mehrfarbigen Objekten"){width="200" zoomable="yes"} |
| Dichte des Inhalts | Die Konzentration visueller Elemente und Details innerhalb eines Bildes, die angeben, wie viele Informationen in den visuellen Raum gepackt werden.<p>Im Gegensatz zur Aufmerksamkeitsverteilung, die misst, wie der Viewer-Fokus über verschiedene Bereiche eines Bildes verteilt ist, konzentriert sich die Inhaltsdichte auf die Menge der vorhandenen visuellen Informationen. Eine höhere Inhaltsdichte bedeutet, dass mehr Elemente vorhanden sind. | `high`, `medium`, `low`<p>Beispiel für `low` Dichte links und `high` Dichte rechts:<p>![Ballspiel mit niedriger und hoher Dichte](/help/assets/category/image-attn-lowhigh.png "Unterschied in niedriger und hoher Inhaltsdichte"){width="200" zoomable="yes"} |
| Bildstil | Die visuelle Behandlung eines Bildes, z. B. eines Fotos oder einer Zeichnung. Sobald die KI den Bildstil bestimmt, können andere Eigenschaften identifiziert werden. Wenn es sich bei dem Bild beispielsweise um ein Foto handelt, können Kameraeinstellungen, die Kameranähe und Lichtbedingungen gelten. | `Photograph`, `Photograph with text overlay`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Beispiel für einen `digital cartoon` Bildstil![Cartoon-Bildstil](/help/assets/category/image-style.png "Bildstil-Cartoon einer Katze"){width="200" zoomable="yes"} |
| Beleuchtungsbedingung | Beschreibt die Qualität und die Eigenschaften des Lichts in einem Bild und beeinflusst seine Stimmung, seinen Ton und seine Sichtbarkeit. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Beispiel für `daylighting` Bedingung:<p>![Person und Hund auf dem Gehsteig im Tageslichtzustand](/help/assets/category/image-lighting.png "Tageslichtzustand"){width="200" zoomable="yes"} |
| Objekte | Identifiziert ein oder mehrere Elemente, Entitäten und Elemente, aus denen das Bild besteht. | Werte sind zu zahlreich, aber einige Beispiele sind: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Beispiel für `toucan`- und `bird`:<p>![Vogel, Toucan-Objekt](/help/assets/category/image-objects-bird.png "Grafikdesign des Toucan-Vogel-Objekts"){width="200" zoomable="yes"} |
| Ausrichtung | Die Ausrichtung des Bildes in Bezug auf seine Breite und Höhe. Ermittelt, ob er breiter ist als er hoch ist (Querformat), größer als er breit ist (Hochformat) oder gleich in Breite und Höhe (Quadrat). | `landscape`, `portrait`, `square`<p>Beispiel für eine `square`:<p>![Quadratische ](/help/assets/category/image-orientation-square.png "-Quadratische Blumenskizze"){width="200" zoomable="yes"} |
| Personen | Wenn mindestens eine Person vorhanden ist, können ein oder mehrere Attribute die Person(en) im Bild beschreiben. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Beispiel für Personen `woman` und `person` Kategorien:<p>![Person Frau mit Kamera](/help/assets/category/image-people.png "Person, die eine Kamera verwaltet"){width="200" zoomable="yes"} |
| Genres der Fotografie | Erkennt das Motiv und die Technik, mit der ein Bild erfasst wird, z. B. `abstract` oder `landscape` (nicht identisch mit der Querformat-Ausrichtung). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite`, `Surreal`,,, `Fashion`,,,,, <p>Siehe [Arten von Fotografien](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html). |
| Szenen | Identifiziert die Einstellung oder Umgebung innerhalb eines Bildes und gibt den Kontext an, wo das Bild erfasst wurde, oder den Typ des gezeigten Standorts. | Werte sind zu zahlreich, aber einige Beispiele sind: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Beispiel für `snow`, `sky`, `winter` und `mountain` Szenen, die auf einem Helm dargestellt werden:<p>![Winter-Schneeszene](/help/assets/category/image-scenes.png "Winter-, Schnee-, Himmel- und Bergszenen-Reflexion"){width="200" zoomable="yes"} |
| Entfernung des Objekts | Der Abstand zwischen der Kamera und dem Motiv eines Bildes. | `close up`, `mid shot`, `long shot`<p>Beispiel einer `closeup shot`:<p>![Nahaufnahme](/help/assets/category/image-subject-distance.png "Nahaufnahme Blume und Juwelen Biene"){width="200" zoomable="yes"} |
| Stile | Erkennt visuelle Behandlungen, die auf Bildelemente angewendet werden, z. B. die in Lightroom oder Photoshop verwendeten. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Beispiel für `circular` Stil:<p>![Rundtor in einem Korallenriff](/help/assets/category/image-styles-circular.png "Rundportal in einem Korallenriff"){width="200" zoomable="yes"} |
| Tags | Erkennt andere Bildmerkmale, die nicht unter eine bestimmte Klassifizierung fallen. Tags bieten zusätzlichen Kontext und Metadaten zum Bild. Beispielsweise kann die KI `helmet` und `motorobike` Objekte in einem Bild erkennen und `riding` als Tag einschließen. | Zu viele Werte, aber einige Beispiele sind: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Beispiel für `dancer` und `dancing` Tags:<p>![Tags für Tänzer und ](/help/assets/category/image-tags.png "-tanzende Person"){width="200" zoomable="yes"} |
