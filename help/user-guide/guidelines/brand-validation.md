---
title: Markenvalidierung in Adobe GenStudio for Performance Marketing
description: Erfahren Sie, wie das integrierte System zur Markenvalidierung in GenStudio for Performance Marketing funktioniert.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 29685c96353703705f3f742e88f3934644bc4282
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Markenvalidierung

In GenStudio for Performance Marketing ist die Markenvalidierung eine wesentliche Komponente, die mit den generativen KI-Funktionen und -Richtlinien ([[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) und [[!DNL Personas]](/help/user-guide/guidelines/personas.md)) zusammenarbeitet. Dadurch wird sichergestellt, dass Ihr gesamter Inhalt mit Ihrer Markenidentität, Ihren ADA-Standards und den individuellen Richtlinien zur Kanalplattform übereinstimmt.

GenStudio for Performance Marketing führt Markenvalidierungen und andere Inhaltsprüfungen zu verschiedenen Aspekten durch, darunter:

* Definierte oder standardmäßige [!DNL Brand]
* Platform-Richtlinien
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->
* Standards des American with Disabilities Act (ADA)

## Zusammenfassung der Inhaltsprüfung

Eine Zusammenfassung der Markenvalidierung und andere Informationen zur Inhaltsprüfung für jede generierte Inhaltsvariante ist über das Symbol _Inhaltsprüfung_ Zusammenfassung für jede Variante auf der Arbeitsfläche zugänglich.

Die _Inhaltsüberprüfung_ Zusammenfassung zeigt Folgendes an:

* Prozentualer Anteil der Konformität mit Ihren [[!DNL Brand]](brands.md), berechnet als Anzahl der [Richtlinien](overview.md) die die Validierung bestanden haben, im Vergleich zur Anzahl der getesteten Richtlinien
* `Pass` oder `Fail` Ergebnisse für die Plattform-Richtlinien wie Meta oder LinkedIn
* `Pass` oder `Fail` Ergebnis für ADA-Barrierefreiheitsstandards

![Zusammenfassung der Inhaltsprüfung](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Klicken Sie auf den Prozentsatz, um zu sehen, wie konform die Variante ist. Die Bewertungen werden automatisch aktualisiert, wenn Sie die Varianten bearbeiten. Sie können auf _Probleme anzeigen und beheben_ klicken, um weitere Kompatibilität sicherzustellen.

Siehe [Verbesserung der Markenausrichtung](#improve-brand-alignment).

## Content-Checkpanel

Das _Inhaltsüberprüfung_-Bedienfeld wird auf der rechten Seite der Arbeitsfläche geöffnet, wenn Sie in der rechten Aktionsleiste _oder_ dem [_Inhaltsüberprüfung_ Zusammenfassungssymbol](#content-check-summary) für eine Variante klicken. Dieses Bedienfeld bietet eine detaillierte Markenvalidierung. Informationen zu Platform-Richtlinien und Barrierefreiheitsstandards sowie Verbesserungsmöglichkeiten für jeden Variantenabschnitt.

![Content-Checkpanel](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

Das _Inhaltsprüfung_-Bedienfeld zeigt Informationen [ Validierung und ](/help/user-guide/guidelines/overview.md#compliance) für jeden Abschnitt der Variante an:

* Darstellung der _Inhaltsüberprüfung_ zusammenfassenden Informationen zu [!DNL Brand], Platform-Richtlinien und Barrierefreiheitsstandards
* _Überprüfung erforderlich_ Abschnitt mit der Anzahl fehlgeschlagener Richtlinien und detaillierten Informationen zu jeder Richtlinie, die überarbeitet werden muss
* _Übergeben_ Abschnitt mit der Anzahl der übergebenen Richtlinien und detaillierten Informationen zu den einzelnen Richtlinien

Unter [Verbesserung der Markenausrichtung](#improve-brand-alignment) erfahren Sie, wie Sie die Punktzahlen _Inhaltsprüfung_ des Bedienfelds verbessern können.

### Inhaltstyp

Im Bedienfeld _Inhaltsüberprüfung_ können Sie ein-/ausschalten, welche Richtlinien- und Barrierefreiheitsprüfungen durchgeführt werden. Klicken Sie auf _Symbol_ Content-Typ“ (Ebenensymbol) oben im Bedienfeld, um diese Option zu aktivieren oder zu deaktivieren:

* **[!DNL Brand]** - Führt die mit [!DNL Brand] Richtlinien verbundenen Prüfungen durch
* **Platform-Richtlinien** - Führt die mit der kanalspezifischen Plattform verbundenen Prüfungen durch, z. B. Meta
* **Barrierefreiheit** - Führt die Prüfungen durch, die mit den ADA-Barrierefreiheitsstandards verbunden sind

Um **Inhaltstyp festzulegen** für die Prüfungen, die Sie durchführen möchten, klicken Sie auf , um sie zu deaktivieren, oder auf die verfügbaren Typen und klicken Sie auf **Anwenden**.

## Verbesserung der Markenausrichtung

Um die Effektivität der generierten Inhalte zu maximieren und eine konsistente Markenidentität zu gewährleisten, verwenden Sie die [_Inhaltsüberprüfung_ Zusammenfassung ](#content-check-summary) das Bedienfeld [_Inhaltsüberprüfung_](#content-check-panel). Sie können bestimmte Abschnitte manuell ändern, um sie an Ihre [[!DNL Brand] Richtlinien](brands.md), Platform-Richtlinien, Prüfungen und Barrierefreiheitsstandards anzupassen.

**So verbessern Sie die Markenausrichtung für generierte Varianten**:

1. Klicken Sie auf das _Inhaltsüberprüfung_ Bedienfeldsymbol in der rechten Aktionsleiste, um Informationen zur Validierung und Barrierefreiheit für eine einzelne Variante anzuzeigen.

   Sie können eine Zusammenfassung der Prüfungen _Überprüfung erforderlich_ und _bestanden_ anzeigen, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   >[!NOTE]
   >
   > Die _Markensprache_ Richtlinie im Bedienfeld _Inhaltsprüfung_ gilt für die gesamte Variante, nicht für einen einzelnen Abschnitt. Die gesamte Inhaltsvariante ist hervorgehoben, um Verbesserungsvorschläge zu erhalten.

1. Klicken Sie hier, um Richtlinien zu korrigieren, die derzeit nicht konform sind.
1. Klicken Sie hier, um jede Prüfung, die überprüft werden muss, in verfügbaren Abschnitten wie _Überschrift_ und _Markensprache_ zu erweitern und zu überprüfen.

   Verwenden Sie die für jede Prüfung angegebenen Begründungen, um Sie bei der Überarbeitung der Varianten zu unterstützen.

1. Nachdem Sie die erforderlichen Änderungen vorgenommen haben, klicken Sie auf **[!UICONTROL Punktzahl erneut überprüfen]**, um Ihre Änderungen erneut zu überprüfen und zu validieren, sodass sie mehr an Ihre Markenidentität, Ihre Plattformrichtlinien und Ihre Barrierefreiheitsstandards angepasst sind.

   Der Inhaltsprüfungsprozess wird erneut ausgeführt. Wenn die überarbeiteten Elemente die Validierung bestehen, wird unten auf der Arbeitsfläche ein grünes Banner angezeigt, um zu bestätigen, dass die Bewertung aktualisiert wurde. Wenn es nach einer erneuten Prüfung keine Änderung gab, bestätigt das Banner, dass es keine Änderung am Score gab. Der Prozentsatz im Symbol _Inhaltsprüfung_ Zusammenfassung für die überarbeitete Variante zeigt auch Ihren Fortschritt an.

1. Fahren Sie mit der Überarbeitung der Abschnitte fort, um sicherzustellen, dass die gesamte Variante die Validierungs- und Barrierefreiheitsprüfungen besteht. Navigieren Sie durch jede Variante mithilfe der Pfeile neben einer einzelnen Variante auf der Arbeitsfläche.

