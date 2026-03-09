---
title: Markenvalidierung in Adobe GenStudio for Performance Marketing
description: Erfahren Sie mehr über das integrierte System zur Markenvalidierung in GenStudio for Performance Marketing.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
TQID: https://experienceleague.adobe.com/0avyL5lvm9hWdlxGE0RwPhP0dX2bA91GNnlKLG1oqEY
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: ad3738c7-91ac-48ed-a914-fd0b03f89396id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: f54ee13b-9545-4d68-9842-a12026e60aafid: fee2c7a9-112e-463c-b451-44aaecaa6966
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 786
ht-degree: 0%

---

# Markenvalidierung

In GenStudio for Performance Marketing ist die Markenvalidierung eine wesentliche Komponente, die mit den generativen KI-Funktionen und -Richtlinien ([[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) und [[!DNL Personas]](/help/user-guide/guidelines/personas.md)) zusammenarbeitet. Dadurch wird sichergestellt, dass Ihr gesamter Inhalt mit Ihrer Markenidentität, Ihren ADA-Standards und den individuellen Richtlinien zur Kanalplattform übereinstimmt.

GenStudio for Performance Marketing führt Markenvalidierungen und andere Inhaltsprüfungen zu verschiedenen Aspekten durch, darunter:

* Definierte oder standardmäßige [!DNL Brand]
* Platform-Richtlinien
* [Unterstützung der Barrierefreiheit](/help/user-guide/guidelines/brand-validation.md#supporting-your-accessibility-strategy)
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

Um die Effektivität der generierten Inhalte zu maximieren und eine konsistente Markenidentität zu gewährleisten, verwenden Sie die [_Inhaltsüberprüfung_ Zusammenfassung ](#content-check-summary) das Bedienfeld [_Inhaltsüberprüfung_](#content-check-panel). Sie können bestimmte Abschnitte manuell ändern, um sie an Ihre [[!DNL Brand] Richtlinien](brands.md), Platform-Richtlinien, Prüfungen und Barrierefreiheitsstandards anzupassen.

**So verbessern Sie die Markenausrichtung für generierte Varianten**:

1. Klicken Sie auf das _Inhaltsüberprüfung_ Bedienfeldsymbol in der rechten Aktionsleiste, um Informationen zu Validierung und Barrierefreiheit anzuzeigen.

   Sie können eine Zusammenfassung der Prüfungen _Überprüfung erforderlich_ und _bestanden_ sehen, um zu sehen, was verbessert werden muss.

   >[!NOTE]
   >
   Die _Markensprache_ Richtlinie im Bedienfeld _Inhaltsprüfung_ gilt für die gesamte Variante, nicht für einen einzelnen Abschnitt. Die gesamte Inhaltsvariante ist hervorgehoben, um Verbesserungsvorschläge zu erhalten.

1. Klicken Sie hier, um Richtlinien zu korrigieren, die derzeit nicht konform sind.
1. Klicken Sie hier, um alle Prüfungen zu erweitern und zu überprüfen, die in verfügbaren Abschnitten wie _Überschrift_, _Farbe_ und _Markenstimme_ überprüft werden müssen.

   Verwenden Sie die für jede Prüfung angegebenen Begründungen, um Sie bei der Überarbeitung von Bildern und Varianten zu unterstützen.

1. Nachdem Sie die erforderlichen Überarbeitungen vorgenommen haben, klicken Sie auf **[!UICONTROL Punktzahl erneut überprüfen]**, um Ihre Änderungen erneut zu überprüfen und zu validieren, um sicherzustellen, dass sie mit Ihrer Markenidentität, den Plattformrichtlinien und den Barrierefreiheitsstandards übereinstimmen.

   Der Inhaltsprüfungsprozess wird erneut ausgeführt. Wenn die überarbeiteten Elemente die Validierung bestehen, wird unten auf der Arbeitsfläche ein grünes Banner angezeigt, um zu bestätigen, dass die Bewertung aktualisiert wurde. Wenn es nach einer erneuten Prüfung keine Änderung gab, bestätigt das Banner, dass es keine Änderung am Score gab. Der Prozentsatz im Symbol _Inhaltsprüfung_ Zusammenfassung für die überarbeitete Variante zeigt auch Ihren Fortschritt an.

1. Fahren Sie mit der Überarbeitung der Abschnitte fort, um sicherzustellen, dass die gesamte Variante die Validierungs- und Barrierefreiheitsprüfungen besteht. Navigieren Sie durch jede Variante mithilfe der Pfeile neben einer einzelnen Variante auf der Arbeitsfläche.

## Unterstützung Ihrer Barrierefreiheitsstrategie

GenStudio for Performance Marketing umfasst Inhaltsprüfungen, die Kunden bei der Unterstützung ihrer eigenen Best Practices für die Barrierefreiheit unterstützen.

Diese Funktion umfasst die folgenden Inhaltsprüfungen:

* Bilder bieten ein `<alt>` Attribut.
* Der generierte Text hat einen Kontrast :1 4,5 % zum Hintergrund.
* Wörter oder Ausdrücke, die auf ungewöhnliche oder eingeschränkte Weise verwendet werden, einschließlich Idiome und Jargon, werden vermieden.
* Es sind erweiterte Formen oder die Bedeutung von Abkürzungen verfügbar.
* Die Inhalte sind auf der Ebene der Sekundarstufe I lesbar.

Kundinnen und Kunden werden ermutigt, diese Funktionen als Teil ihrer umfassenderen Barrierefreiheitsstrategie zu verwenden, obwohl Kundinnen und Kunden für ihre eigenen gesetzlichen Bestimmungen und die Einhaltung der Barrierefreiheitsvorschriften verantwortlich bleiben.
