---
title: Markenvalidierung in Adobe GenStudio for Performance Marketing
description: Erfahren Sie, wie das integrierte System zur Markenvalidierung in GenStudio for Performance Marketing funktioniert.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: e2acf90ef5fef6af03a756882caf53ab125055c4
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# Markenvalidierung

In GenStudio for Performance Marketing ist die Markenvalidierung eine wesentliche Komponente, die mit den generativen KI-Funktionen und -Richtlinien ([[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) und [[!DNL Personas]](/help/user-guide/guidelines/personas.md)) zusammenarbeitet. Dadurch wird sichergestellt, dass Ihr gesamter Inhalt mit Ihrer Markenidentität, Ihren ADA-Standards und den individuellen Richtlinien zur Kanalplattform übereinstimmt.

GenStudio for Performance Marketing führt Markenvalidierungen und andere Inhaltsprüfungen zu verschiedenen Aspekten durch, darunter:

* Definierte oder standardmäßige [!DNL Brand]
* Platform-Richtlinien
* [Standards des American with Disabilities Act (ADA)](/help/user-guide/guidelines/brand-validation.md#american-with-disabilities-act-ada-validation)
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->


## Zusammenfassung der Inhaltsprüfung

Eine Zusammenfassung der Markenvalidierung und andere Informationen zur Inhaltsprüfung für jedes Element des generierten Inhalts sind über das Symbol _Inhaltsprüfung_ Zusammenfassung für jede Variante auf der Arbeitsfläche zugänglich.

Die _Inhaltsüberprüfung_ Zusammenfassung zeigt Folgendes an:

* Prozentualer Anteil der Konformität mit Ihren [[!DNL Brand]](brands.md), berechnet als Anzahl der [Richtlinien](overview.md) die die Validierung bestanden haben, im Vergleich zur Anzahl der getesteten Richtlinien
* `Pass` oder `Fail` Ergebnisse für die Plattformrichtlinien wie Meta oder LinkedIn
* `Pass` oder `Fail` Ergebnis für ADA-Barrierefreiheitsstandards

![Zusammenfassung der Inhaltsprüfung](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Klicken Sie auf den Prozentsatz, um zu sehen, wie konform die Variante ist. Die Bewertungen werden automatisch aktualisiert, wenn Sie Änderungen an den Varianten oder anderen Inhalten vornehmen. Sie können auf _Probleme anzeigen und beheben_ klicken, um weitere Kompatibilität sicherzustellen.

Siehe [Verbesserung der Markenausrichtung](#improve-brand-alignment).

## Content-Checkpanel

Das _Inhaltsüberprüfung_-Bedienfeld wird auf der rechten Seite der Arbeitsfläche geöffnet, wenn Sie in der rechten Aktionsleiste _oder_ über das [_Inhaltsüberprüfung_ Zusammenfassungssymbol klicken](#content-check-summary). Dieses Bedienfeld bietet detaillierte Informationen zur Markenvalidierung, zu Plattform-Richtlinien und zu Barrierefreiheitsstandards sowie Möglichkeiten zur Verbesserung.

![Content-Checkpanel](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

Das Bedienfeld _Inhaltsüberprüfung_ zeigt Informationen zur Validierung und [Compliance](/help/user-guide/guidelines/overview.md#compliance) für Bilder und Variantenabschnitte an:

* Darstellung der _Inhaltsüberprüfung_ zusammenfassenden Informationen zu [!DNL Brand], Platform-Richtlinien und Barrierefreiheitsstandards
* _Überprüfung erforderlich_ Abschnitt mit der Anzahl fehlgeschlagener Richtlinien und detaillierten Informationen zu jeder Richtlinie, die überarbeitet werden muss
* _Übergeben_ Abschnitt mit der Anzahl der übergebenen Richtlinien und detaillierten Informationen zu den einzelnen Richtlinien

Unter [Verbesserung der Markenausrichtung](#improve-brand-alignment) erfahren Sie, wie Sie die Punktzahlen _Inhaltsprüfung_ des Bedienfelds verbessern können.

### Inhaltstyp

Im Bedienfeld _Inhaltsüberprüfung_ können Sie ein-/ausschalten, welche Richtlinien- und Barrierefreiheitsprüfungen durchgeführt werden. Klicken Sie auf _Symbol_ Content-Typ“ (Ebenensymbol) oben im Bedienfeld, um diese Option zu aktivieren oder zu deaktivieren:

* **[!DNL Brand]** - Führt die mit [!DNL Brand] Richtlinien verbundenen Prüfungen durch
* **Platform-Richtlinien**: Führt die mit der kanalspezifischen Plattform verbundenen Prüfungen durch, z. B. Meta
* **Barrierefreiheit** - Führt die Prüfungen durch, die mit den ADA-Barrierefreiheitsstandards verbunden sind

Um **Inhaltstyp festzulegen** für die Prüfungen, die Sie durchführen möchten, klicken Sie auf , um sie zu deaktivieren, oder auf die verfügbaren Typen und klicken Sie auf **Anwenden**.

## Verbesserung der Markenausrichtung

Um die Effektivität der generierten Inhalte zu maximieren und eine konsistente Markenidentität zu gewährleisten, verwenden Sie die [_Inhaltsüberprüfung_ Zusammenfassung &#x200B;](#content-check-summary) das Bedienfeld [_Inhaltsüberprüfung_](#content-check-panel). Sie können bestimmte Abschnitte manuell ändern, um sie an Ihre [[!DNL Brand] Richtlinien](brands.md), Platform-Richtlinien, Prüfungen und Barrierefreiheitsstandards anzupassen.

**So verbessern Sie die Markenausrichtung für generierte Varianten**:

1. Klicken Sie auf das _Inhaltsüberprüfung_ Bedienfeldsymbol in der rechten Aktionsleiste, um Informationen zu Validierung und Barrierefreiheit anzuzeigen.

   Sie können eine Zusammenfassung der Prüfungen _Überprüfung erforderlich_ und _bestanden_ sehen, um zu sehen, was verbessert werden muss.

   >[!NOTE]
   >
   > Die _Markensprache_ Richtlinie im Bedienfeld _Inhaltsprüfung_ gilt für die gesamte Variante, nicht für einen einzelnen Abschnitt. Die gesamte Inhaltsvariante ist hervorgehoben, um Verbesserungsvorschläge zu erhalten.

1. Klicken Sie hier, um Richtlinien zu korrigieren, die derzeit nicht konform sind.
1. Klicken Sie hier, um alle Prüfungen zu erweitern und zu überprüfen, die in verfügbaren Abschnitten wie _Überschrift_, _Farbe_ und _Markenstimme_ überprüft werden müssen.

   Verwenden Sie die für jede Prüfung angegebenen Begründungen, um Sie bei der Überarbeitung von Bildern und Varianten zu unterstützen.

1. Nachdem Sie die erforderlichen Überarbeitungen vorgenommen haben, klicken Sie auf **[!UICONTROL Punktzahl erneut überprüfen]**, um Ihre Änderungen erneut zu überprüfen und zu validieren, um sicherzustellen, dass sie mit Ihrer Markenidentität, den Plattformrichtlinien und den Barrierefreiheitsstandards übereinstimmen.

   Der Inhaltsprüfungsprozess wird erneut ausgeführt. Wenn die überarbeiteten Elemente die Validierung bestehen, wird unten auf der Arbeitsfläche ein grünes Banner angezeigt, um zu bestätigen, dass die Bewertung aktualisiert wurde. Wenn es nach einer erneuten Prüfung keine Änderung gab, bestätigt das Banner, dass es keine Änderung am Score gab. Der Prozentsatz im Symbol _Inhaltsprüfung_ Zusammenfassung für die überarbeitete Variante zeigt auch Ihren Fortschritt an.

1. Fahren Sie mit der Überarbeitung der Abschnitte fort, um sicherzustellen, dass die gesamte Variante die Validierungs- und Barrierefreiheitsprüfungen besteht. Navigieren Sie durch jede Variante mithilfe der Pfeile neben einer einzelnen Variante auf der Arbeitsfläche.

## Validierung des American with Disabilities Act (ADA)

Diese Barrierefreiheitsprüfungen sind für die Einhaltung des American With Disabilities Act (ADA) enthalten:

[WCAG 1.1.1 Nichttextlicher Inhalt](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html) - Stellt sicher, dass Bilder ein `<alt>` Attribut bereitstellen.
[WCAG 1.4.3 Kontrast (Minimum)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html) - Stellt sicher, dass der generierte Text einen Kontrast von 4,5 % :1 Hintergrund hat.
[WCAG 3.1.3 Ungewöhnliche Wörter](https://www.w3.org/WAI/WCAG21/Understanding/unusual-words.html) - Identifiziert Wörter oder Ausdrücke, die auf ungewöhnliche oder eingeschränkte Weise verwendet werden, einschließlich Idiome und Jargon.
[WCAG 3.1.4 Abkürzungen](https://www.w3.org/WAI/WCAG21/Understanding/abbreviations.html) - Ein Mechanismus zur Identifizierung der erweiterten Form oder Bedeutung von Abkürzungen.
[WCAG 3.1.5 Reading Level](https://www.w3.org/WAI/WCAG21/Understanding/reading-level.html) - Stellt sicher, dass die Inhalte auf einer niedrigeren Sekundarstufe lesbar sind.

