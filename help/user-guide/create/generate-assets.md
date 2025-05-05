---
title: Erstellen von Bildern
description: Erstellen Sie in Adobe ein Bild, das dem Stil eines Referenzbilds entspricht [!DNL GenStudio]  für Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 277731aeea966da3cbd1fdabf015bfab3b907d39
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Erstellen von Bildern

Mit GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (Pinselsymbol) können Sie _[!DNL On-brand images]_&#x200B;generieren - generierte Assets, die sich von einem ausgewählten Bild inspirieren lassen und dessen visuelle Wirkung und allgemeine Ästhetik einfangen.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

Um ein ansprechendes und effektives Bild zu entwerfen, wird empfohlen, dass Sie [Richtlinien zu GenStudio for Performance Marketing hinzufügen](/help/user-guide/guidelines/add-guidelines.md) und die [Grundlagen von Eingabeaufforderungen“ ](/help/user-guide/effective-prompts.md).

## Bildtypen

_[!DNL On-brand images]_&#x200B;sind generierte Assets, die sich von einem ausgewählten Bild inspirieren lassen und dessen visuelle Wirkung und Gesamtästhetik einfangen. Diese Bilder werden mithilfe von Bildern erstellt, die bereits in [!DNL Content] verfügbar sind, sowie anhand einer sorgfältig gestalteten Eingabeaufforderung, die das Design steuert. Sie halten sich strikt an die Markenrichtlinien und Parameter, die während des Generierungsprozesses ausgewählt wurden.

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ --> Richtlinien, Parameter und eine [sorgfältig gestaltete Eingabeaufforderung](/help/user-guide/effective-prompts.md) enthalten, um ansprechende Bild-Assets bereitzustellen.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Erstellen von Markenbildern

Sie können [!DNL On-brand images] mithilfe definierter Richtlinien, Parameter und eines ausgewählten Referenzbilds generieren. Diese Elemente leiten zusammen mit Ihrer Eingabeaufforderung die Erstellung konsistenter [!DNL On-brand image].

### Referenzbild auswählen

Um ein _[!DNL On-brand images]_&#x200B;zu erstellen, wählen Sie ein vorhandenes Bild aus, das in [!DNL Content] gespeichert ist. Informationen [ unterstützten [!DNL on-brand image]-Dimensionen finden Sie ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) „Best Practices für Vorlagen“.

**So wählen Sie ein Referenzbild aus**:

1. Klicken Sie _[!DNL Create]_&#x200B;auf **[!UICONTROL Markeninternes Bild]**.
1. Verwenden Sie die Suchoption neben _Filter_, um ein bestimmtes Bild zu finden.

   ![Referenzbild auswählen](/help/assets/select-img.png){width="400" zoomable="yes"}

   Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie und wählen Sie ein Bild aus.

1. Klicken Sie in _Ansicht_ Bild auswählen“ auf ein Bild.

   Das ausgewählte Bild kann bis zu 10 MB groß sein.

1. Klicken Sie **[!UICONTROL Verwenden]**.

   Die Arbeitsfläche, die als zentraler Hub für die Inhaltserstellung dient, wird angezeigt.

### Parameter hinzufügen

Die Integration [Richtlinien](/help/user-guide/guidelines/overview.md) und Parameter verbessert den Prozess der Inhaltserstellung und ist ein entscheidender Vorbereitungsschritt für die Erstellung eines [!DNL on-brand image].

**Hinzufügen von Richtlinien und Parametern**:

1. Wählen _auf der Registerkarte_ Standard“ eine [!DNL Brand] aus, um über die Inhaltserstellung zu informieren.

   Wenn in diesem Menü keine Marken verfügbar sind, [ Sie „Richtlinien zu Ihrer GenStudio for Performance Marketing hinzufügen](/help/user-guide/guidelines/add-guidelines.md).

1. Wählen Sie unter „Bildkategorie“ eine Bildkategorie aus _[!UICONTROL die Ihrem]_ am besten entspricht.

   Bildkategorien sind verfügbar, wenn ein [!DNL Brand] ausgewählt wurde. Die Optionen werden durch die ausgewählten [!DNL Brand] bestimmt.

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. Wählen Sie unter (Seitenverhältnis) das _[!UICONTROL Seitenverhältnis]_.
1. Klicken Sie **[!UICONTROL Aus Inhalt auswählen]** in _[!UICONTROL Stilverweis]_, um ein Referenzbild hinzuzufügen. Das ausgewählte Bild beeinflusst die visuelle Ästhetik und Tiefe der von Ihnen generierten Bilder.

   Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie und wählen Sie ein Bild aus.

1. Wählen Sie auf _Registerkarte_ den _Inhaltstyp_ aus.

   Diese ist basierend auf der für die ausgewählte [!DNL Brand] vorhandenen Bildkategorie - _Art_ oder _Foto_ - vorausgewählt und kann nicht bearbeitet werden.

1. Passen Sie die Gesamtintensität der vorhandenen visuellen Eigenschaften des Bildes in &quot;_[!UICONTROL &quot;]_.

### Eingabeaufforderung eingeben

Erstellen Sie nach Auswahl der Parameter eine Eingabeaufforderung in natürlicher Sprache, um mit der Generierung von Markenbildern zu beginnen.

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

1. Führen Sie eine Bildbearbeitung durch, z[ B. ](https://helpx.adobe.com/de/express/create-and-edit-images/edit-images/crop-images.html)Zuschneiden eines Bildes[ „Entfernen eines ](https://helpx.adobe.com/de/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html)&quot; und Anwenden von Effekten.

   Siehe [Dokumentation zu Adobe Express](https://helpx.adobe.com/de/express/user-guide.html) um zu erfahren, wie Sie Bilder in GenStudio for Performance Marketing mit Adobe Express überarbeiten können.

1. Klicken Sie _[!UICONTROL Änderungen übernehmen]_ um Ihre Änderungen zu speichern.
1. Fahren Sie mit der Bearbeitung einzelner Bildvarianten nach Bedarf fort und wenden Sie Änderungen an, um Ihren Fortschritt zu speichern.

### Überprüfen der Ausrichtung der Inhaltsprüfung

Um die generierten Varianten zu optimieren und die strikte Einhaltung von Markenidentität, Plattformrichtlinien und Barrierefreiheitsstandards sicherzustellen, nutzen Sie die Leistungsfähigkeit des Bedienfelds [_Inhaltsprüfung_ ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Dieses Bedienfeld zeigt umfassende Details zur Inhaltsprüfung an und beleuchtet Bereiche mit Verbesserungsmöglichkeiten.

**So führen Sie Inhaltsprüfungen durch**:

1. Klicken Sie auf _Symbol für das Bedienfeld_ Inhaltsüberprüfung“ in der rechten Aktionsleiste, um das Bedienfeld [_Inhaltsüberprüfung_ zu ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Zeigen Sie eine Zusammenfassung der Prüfungen *Überprüfung erforderlich* und *bestanden* an, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   ![_Inhaltsüberprüfung_ Bedienfeld](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Ändern Sie Bildvarianten, um sicherzustellen, dass Ihre Varianten eng mit den durchgeführten Inhaltsprüfungen abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## Veröffentlichen und Exportieren von Bildern

Die generierten Bildentwürfe werden im Abschnitt _Zuletzt verwendet_ der [!DNL Create] Startseite angezeigt.

Um die generierten Bilder für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihre neuen Bilder zu veröffentlichen** klicken Sie in der oberen Symbolleiste auf **[!UICONTROL Veröffentlichen]**.
   1. _[!UICONTROL Fügen Sie Details]_, wie _[!UICONTROL Kampagnen]_ oder _[!UICONTROL Kanäle]_ hinzu, falls gewünscht.
   1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

1. **Um Ihre neuen Bilder zu exportieren** klicken Sie in der oberen Symbolleiste **[!UICONTROL Exportieren]**.
   1. Wählen Sie das Format aus - JPG oder PNG - und klicken Sie auf **[!UICONTROL Exportieren]**.

Siehe [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
