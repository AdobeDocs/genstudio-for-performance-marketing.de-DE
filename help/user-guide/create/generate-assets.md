---
title: Erzeugen von Bildvarianten
description: Erstellen Sie in Adobe ein Bild, das dem Stil eines Referenzbilds entspricht [!DNL GenStudio]  für Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
TQID: https://experienceleague.adobe.com/NXtN00EKTe0lGI8jJMJWJfWx6mHoMQI1of1mJhgrR5U
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dcid: dee4e9a9-78d1-4953-8179-f8da6117027did: e4a0febc-5163-4017-82ce-fc7594509fb6id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 6d1053bf94b0a0ba65be90359e4d176e64dfffae
workflow-type: tm+mt
source-wordcount: 752
ht-degree: 0%

---

# Erzeugen von Bildvarianten

Mit GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (Pinselsymbol) können Sie _[!DNL Image variants]_generieren - generierte Assets, die sich von einem ausgewählten Bild inspirieren lassen und dessen visuelle Wirkung und allgemeine Ästhetik einfangen.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL Image variants]_ and _[!DNL Similar images]_. -->

Um ein ansprechendes und effektives Bild zu entwerfen, wird empfohlen, dass Sie [Richtlinien zu GenStudio for Performance Marketing hinzufügen](/help/user-guide/guidelines/add-guidelines.md) und die [Grundlagen von Eingabeaufforderungen“ ](/help/user-guide/effective-prompts.md).

## Bildtypen

_[!DNL Image variants]_sind generierte Assets, die sich von einem ausgewählten Bild inspirieren lassen und dessen visuelle Wirkung und Gesamtästhetik einfangen. Diese Bilder werden mithilfe von Bildern erstellt, die bereits in [!DNL Content] verfügbar sind, sowie anhand einer sorgfältig gestalteten Eingabeaufforderung, die das Design steuert. Sie halten sich strikt an die Markenrichtlinien und Parameter, die während des Generierungsprozesses ausgewählt wurden.

_[!DNL Image variants]_<!-- and _[!DNL Similar images]_ --> Richtlinien, Parameter und eine [sorgfältig gestaltete Eingabeaufforderung](/help/user-guide/effective-prompts.md) enthalten, um ansprechende Bild-Assets bereitzustellen.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Erzeugen von Bildvarianten

Sie können [!DNL Image variants] mithilfe definierter Richtlinien, Parameter und eines ausgewählten Referenzbilds generieren. Neben Ihrer Eingabeaufforderung leiten diese Elemente die Erstellung konsistenter [!DNL Image variants].

### Referenzbild auswählen

Um _[!DNL Image variants]_zu erstellen, wählen Sie ein vorhandenes Bild aus, das in [!DNL Content] gespeichert wurde. Siehe [Best Practices für Vorlagen](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines) für Informationen zu unterstützten Bildabmessungen.

**So wählen Sie ein Referenzbild aus**:

1. Klicken Sie _[!DNL Create]_auf **[!UICONTROL Bildvarianten generieren]**.
   ![Erzeugen von Bildvarianten](./gen-image-variants.png){width="400" zoomable="yes"}
1. Um ein Referenzbild auszuwählen, verwenden Sie die Schaltfläche _[!UICONTROL Aus Inhalt auswählen]_, um ein bestimmtes Bild zu finden.
   ![Aus Inhalt auswählen](./gen-variant-select-from-content.png){width="200" zoomable="yes"}

   Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie und wählen Sie ein Bild aus.

   ![Referenzbild auswählen](/help/assets/select-img.png){width="400" zoomable="yes"}

1. Klicken Sie in _Ansicht_ Bild auswählen“ auf ein Bild, um das Auswahlfeld zu aktivieren.

   Das ausgewählte Bild kann bis zu 10 MB groß sein. Es kann jeweils nur ein Bild ausgewählt werden.

1. Klicken Sie **[!UICONTROL Verwenden]**.

   Die Arbeitsfläche, die als zentraler Hub für die Inhaltserstellung dient, wird angezeigt.

### Parameter hinzufügen

Die Integration [Richtlinien](/help/user-guide/guidelines/overview.md) und Parameter verbessert den Prozess der Inhaltserstellung und ist ein wichtiger Schritt zur Vorbereitung der [!DNL Image variants].

**Hinzufügen von Richtlinien und Parametern**:

1. Wählen _auf der Registerkarte_ Standard“ eine [!DNL Brand] aus, um über die Inhaltserstellung zu informieren.

   Wenn in diesem Menü keine Marken verfügbar sind, [ Sie „Richtlinien zu Ihrer GenStudio for Performance Marketing hinzufügen](/help/user-guide/guidelines/add-guidelines.md).
1. Wählen Sie ein Modell aus, das für die Bildgenerierung verwendet werden soll _[!UICONTROL Model]_.
1. Wählen Sie unter (Seitenverhältnis) das _[!UICONTROL Seitenverhältnis]_.

### Eingabeaufforderung eingeben

Erstellen Sie nach Auswahl der Parameter eine Eingabeaufforderung in natürlicher Sprache, um mit der Generierung von Bildvarianten zu beginnen.

Siehe [Effektive Eingabeaufforderungen schreiben](/help/user-guide/effective-prompts.md).

**So geben Sie eine Eingabeaufforderung ein**:

1. Geben Sie in das Eingabeaufforderungsfeld eine Eingabeaufforderung ein.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

Standardmäßig werden vier Varianten - angetrieben von der Eingabeaufforderung, den Parametern und dem Inhalt, den Sie hinzugefügt haben - generiert und auf der Arbeitsfläche angezeigt.

### In Adobe Express bearbeiten

Nachdem Sie Bildvarianten generiert haben, können Sie sie mit Adobe Express direkt in Adobe GenStudio for Performance Marketing bearbeiten.

**So bearbeiten Sie ein einzelnes Bild mit Adobe Express**:

1. Bewegen Sie den Mauszeiger über eine generierte Bildvariante und klicken Sie auf _[!UICONTROL Bearbeiten in Adobe Express]_.

   Ein _Powered by Adobe Express_-Fenster wird angezeigt.

1. Führen Sie eine Bildbearbeitung durch, z[ B. ](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html)Zuschneiden eines Bildes[ „Entfernen eines ](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html)&quot; und Anwenden von Effekten.

   Siehe [Dokumentation zu Adobe Express](https://helpx.adobe.com/express/user-guide.html) um zu erfahren, wie Sie Bilder in GenStudio for Performance Marketing mit Adobe Express überarbeiten können.

1. Klicken Sie _[!UICONTROL Änderungen übernehmen]_ um Ihre Änderungen zu speichern.
1. Fahren Sie mit der Bearbeitung einzelner Bildvarianten nach Bedarf fort und wenden Sie Änderungen an, um Ihren Fortschritt zu speichern.

### Überprüfen der Ausrichtung der Inhaltsprüfung

Um die generierten Varianten zu optimieren und die strikte Einhaltung von Markenidentität, Plattformrichtlinien und Barrierefreiheitsstandards sicherzustellen, nutzen Sie die Leistungsfähigkeit des Bedienfelds [_Inhaltsprüfung_ ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Dieses Bedienfeld zeigt umfassende Details zur Inhaltsprüfung an und beleuchtet Bereiche mit Verbesserungsmöglichkeiten.

**So führen Sie Inhaltsprüfungen durch**:

1. Klicken Sie auf _Symbol für das Bedienfeld_ Inhaltsüberprüfung“ in der rechten Aktionsleiste, um das Bedienfeld [_Inhaltsüberprüfung_ zu ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Zeigen Sie eine Zusammenfassung der Prüfungen *Überprüfung erforderlich* und *bestanden* an, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   ![_Inhaltsüberprüfung_ Bedienfeld](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Ändern Sie Bildvarianten, um sicherzustellen, dass Ihre Varianten eng mit den durchgeführten Inhaltsprüfungen abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

<!-- 
## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} 
-->

## Veröffentlichen und Exportieren von Bildern

Die generierten Bildentwürfe werden im Abschnitt _Zuletzt verwendet_ der [!DNL Create] Startseite angezeigt.

Um die generierten Bilder für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihre neuen Bilder zu veröffentlichen** klicken Sie in der oberen Symbolleiste auf **[!UICONTROL Veröffentlichen]**.
   1. _[!UICONTROL Fügen Sie Details]_, wie _[!UICONTROL Kampagnen]_ oder _[!UICONTROL Kanäle]_ hinzu, falls gewünscht.
   1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

1. **Um Ihre neuen Bilder zu exportieren** klicken Sie in der oberen Symbolleiste **[!UICONTROL Exportieren]**.
   1. Wählen Sie das Format aus - JPG oder PNG - und klicken Sie auf **[!UICONTROL Exportieren]**.

Siehe [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
