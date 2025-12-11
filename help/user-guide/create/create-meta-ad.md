---
title: Erstellen eines Meta Ad Experience
description: Erfahren Sie, wie Sie mit Adobe GenStudio for Performance Marketing markeninterne Meta-Anzeigen-Erlebnisse für Facebook oder Instagram erstellen können.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: d3ddbefc47d3289041783a1a277aa2e855d13ccb
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Erstellen eines Meta-Anzeigen-Erlebnisses

In diesem Tutorial wird gezeigt, wie Sie mit GenStudio for Performance Marketing [ (](/help/user-guide/create/meta-experiences.md) im linken Navigationsbereich) Meta-Anzeigen-Erlebnisse mit Branding generieren können.[[!DNL Create]](/help/user-guide/create/overview.md)

Bevor Sie mit der Erstellung eines Meta-Anzeigenerlebnisses beginnen, ist es wichtig, [Richtlinien ](/help/user-guide/guidelines/add-guidelines.md) GenStudio for Performance Marketing zu integrieren und sich mit den Grundlagen der [Eingabeaufforderung“ ](/help/user-guide/effective-prompts.md).

## Vorlage wählen

Verwenden Sie eine verfügbare Vorlage, um das Framework für Ihre Inhalte bereitzustellen, um mit der Erstellung eines neuen Meta-Anzeigenerlebnisses zu beginnen. Informationen zu den unterstützten Seitenverhältnissen für Meta[Anzeigenvorlagen finden Sie unter ](/help/user-guide/templates/meta-template.md)Richtlinien für Meta-Anzeigenvorlagen .

Bei der Auswahl einer Vorlage haben Sie die Möglichkeit, eine der hochgeladenen Vorlagen oder eine Einstiegsvorlage zu verwenden.

**So wählen Sie eine Meta-Anzeigenvorlage**:

1. Klicken Sie _[!DNL Create]_auf **[!UICONTROL Meta-Anzeigen]**.
1. Wählen Sie **[!UICONTROL Benutzerdefinierte Vorlagen]** aus, um Ihre hochgeladenen Vorlagen zu durchsuchen, oder **[!UICONTROL Startervorlagen]**, um die vordefinierten Vorlagen zu durchsuchen.

   Wenn Sie Video-Assets zu Ihren Meta-Varianten hinzufügen möchten, müssen Sie eine Startvorlage auswählen. Sie sind mit systemdefinierten Inhaltsbereichen vorgeladen, die die Verwendung von Videos erleichtern.

1. Klicken Sie, um eine Vorlage auszuwählen, und klicken Sie auf **[!UICONTROL Verwenden]**.

   Diese Aktion öffnet die Arbeitsfläche, die den zentralen Hub für die Inhaltserstellung darstellt.

## Parameter hinzufügen

Das Hinzufügen [Richtlinien](/help/user-guide/guidelines/overview.md) und Assets in _Parameter_ in der Eingabeaufforderungsschublade verbessert den Inhaltserstellungsprozess und ist ein wichtiger Schritt bei der Vorbereitung der Erstellung einer Meta-Anzeige.

Wenn Sie eine Vorlage mit vordefinierten Richtlinien (z. B. [!DNL Brands], [!DNL Personas] oder [!DNL Products]) verwenden, gelten diese Richtlinien für Ihre Varianten. Sie können sie bei Bedarf ändern.

**Hinzufügen von Parametern und Assets**:

1. Klicken Sie auf _Parameter_, um die Eingabeaufforderungsschublade zu erweitern.
1. Wählen Sie _Abschnitt_ Parameter“ Richtlinien - [!DNL Brands], [!DNL Personas] und [!DNL Products] - aus, um über die Inhaltserstellung zu informieren.

   ![Persona auswählen](/help/assets/persona-select-meta.png){width="300" align="center" zoomable="yes"}

   Wenn in diesen Menüs keine Marken, Rollen oder Produkte verfügbar sind, [fügen Sie Ihrer GenStudio for Performance Marketing Richtlinien hinzu](/help/user-guide/guidelines/add-guidelines.md).

1. Fügen Sie Inhalte (Bilder oder Videos) für die Verwendung im -Erlebnis *und* hinzu, um die Inhaltserstellung zu beeinflussen:
   * Klicken Sie **[!UICONTROL Aus Inhalt auswählen]**, um Assets aus Ihrem [!DNL Content]-Repository auszuwählen, zu filtern und ein oder mehrere Bilder auszuwählen.

     Wenn Sie eine Vorlage mit einem Abschnitt für Videos verwenden, werden Videoinhalte (.mp4) vorausgewählt und für Sie gefiltert. Bewegen Sie den Mauszeiger über ein Video, um eine automatisch wiedergegebene Vorschau anzuzeigen.

     ![Auswählen visueller Inhalte](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie ein oder mehrere Bilder und wählen Sie sie aus.

   * Oder ziehen Sie Bilder per Drag-and-Drop in den **[!UICONTROL Aus Inhalt auswählen]**, um ein oder mehrere neue Assets hochzuladen.

1. Klicken Sie **[!UICONTROL Verwenden]**.

Wenn Sie mit dem Hinzufügen von Parametern fertig sind, können Sie die Eingabeaufforderungsschublade reduzieren, indem Sie erneut auf das Symbol _Parameter_ klicken.

## Eingabeaufforderung eingeben

Nachdem Sie Richtlinien ausgewählt haben, erstellen Sie eine Eingabeaufforderung in natürlicher Sprache, um mit der Erstellung von Inhalten für Ihr neues Meta-Anzeigenerlebnis zu beginnen. Detaillierte Eingabeaufforderungen liefern eine höhere Qualität als vage oder mehrdeutige Eingabeaufforderungen.

Weitere [ zu Eingabeaufforderungen finden Sie ](/help/user-guide/effective-prompts.md)Schreiben effektiver Eingabeaufforderungen).

**So geben Sie eine Eingabeaufforderung ein**:

1. Geben Sie in das _„Beschreiben der Erlebnisse, die Sie generieren möchten“ eine Eingabeaufforderung_.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

   Unter [Verwalten von Videos](#manage-videos) erfahren Sie, wie sie generiert werden und wie Sie sie verwalten.

Standardmäßig werden vier Varianten - alle basierend auf der Eingabeaufforderung, Richtlinien und hinzugefügten Inhalten - generiert und auf der Arbeitsfläche angezeigt.

Erzeugte Inhalte werden progressiv geladen : Wenn jeder Abschnitt der Meta-Erlebnisse generiert wird, erscheinen sie auf der Arbeitsfläche. Unter [Meta-Erlebnisse](/help/user-guide/create/meta-experiences.md#progressive-loading) erfahren Sie, wie diese Änderungen auf die Arbeitsfläche geladen werden.

## Meta Ads-Kanal auswählen

Beim Generieren einer Meta-Anzeige können Sie zwischen Facebook- oder Instagram-Anzeigen wählen.

Schalten Sie in der rechten Menüleiste (Facebook **und Instagram** die Kanaloption für Meta-Anzeigen ein (zwischen **Facebook) und** Instagram), um Varianten für jeden Kanal anzuzeigen und zu verwalten.

Bei [Überarbeitung der Meta-Anzeigen](#revise-generated-variants) können Sie das Seitenverhältnis von Facebook- und Instagram-Anzeigen ändern.

## Überarbeiten generierter Varianten

Bevor Sie auswählen, was zur Genehmigung oder Veröffentlichung an [!DNL Content] gesendet werden soll, können Sie die Meta-Anzeigen bearbeiten oder eine Variante aus dem Satz der generierten Anzeigen löschen.

Um eine einzelne zu überarbeitende Ebene zu markieren, klicken Sie auf ein bearbeitbares Feld oder Bild und klicken Sie auf _[!UICONTROL Ebenen anzeigen]_.

**Überarbeiten generierter Varianten**:

* **Um [ Meta-Anzeigenentwurfsnamen zu bearbeiten](/help/user-guide/create/manage-variants.md#change-draft-name)** klicken Sie oben auf der Arbeitsfläche auf den Titel _Nicht benannter_&quot; und geben Sie einen neuen Titel ein.
* **Um [eine Meta-Anzeige manuell zu bearbeiten](/help/user-guide/create/manage-variants.md#manually-edit-text)** klicken Sie auf einen der Anzeigenabschnitte (z. B. die Betreffzeile,
Kopfzeile oder Textkörper) und bearbeiten Sie sie nach Bedarf.
* **Um die call to action zu ändern oder auszuwählen** klicken Sie auf die Schaltfläche call-to-action und wählen Sie aus den verfügbaren Textoptionen für die Schaltfläche aus. Geben _unter_ eine URL für den call-to-action-Text ein.
* **Um [ Textformatierung anzuwenden](/help/user-guide/create/manage-variants.md#manually-edit-text)** in einer Variante klicken Sie auf den On-Image-Text oder Inline-Link für eine Variante und klicken Sie auf **[!UICONTROL Text formatieren]**.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Um [einen Link zu einem Bild in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-image-link)** klicken Sie auf ein Bild-Asset (oder den Bereich des Bild-Assets, wenn derzeit kein Bild vorhanden ist) und klicken Sie auf das Link-Symbol.
* **Um [Größe und Seitenverhältnis der Anzeige zu ändern](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klicken Sie auf die Schaltfläche _[!UICONTROL Größe ändern]_ (Feld mit einem Schaltflächensymbol auf der linken Seite der Arbeitsfläche) und wählen Sie eine neue Größe und ein neues Seitenverhältnis aus, das auf alle Varianten angewendet werden soll. Die Varianten werden dupliziert und in der Größe angepasst.
* **Um [ Abschnitt einer Variante neu zu erstellen](/help/user-guide/create/manage-variants.md#re-generate-sections)** klicken Sie auf ein bearbeitbares Textfeld und verwenden Sie die _[!UICONTROL Vorgeschlagene Bearbeitungen]_ oder geben Sie eine neue Eingabeaufforderung ein und klicken Sie auf **[!UICONTROL Generieren]**.
* **Um [Bilder in einer Variante hinzuzufügen oder auszutauschen](/help/user-guide/create/manage-variants.md#swap-image)** klicken Sie auf ein Bild-Asset (oder den Bereich des Bild-Assets, wenn derzeit kein Bild vorhanden ist) und klicken Sie auf das Symbol **[!UICONTROL Austauschen]** Inhalt.
* **Um [Bilder zuzuschneiden oder neu](/help/user-guide/create/manage-variants.md#crop-assets)**, klicken Sie auf ein Bild, klicken Sie auf **[!UICONTROL Bearbeiten]** (Stiftsymbol) und dann auf **[!UICONTROL Zuschneiden]**. Anpassen der Bildgröße und -platzierung.
* **Um [Generative Erweitern zu verwenden, um Bilder zu ](/help/user-guide/create/manage-variants.md#use-generative-expand) und an Ihre Arbeitsvorlage anzupassen** klicken Sie auf ein Bild, klicken Sie auf **[!UICONTROL Bearbeiten]** (Bleistiftsymbol) und dann auf **[!UICONTROL Erweitern]**. Passen Sie das Bild an das erforderliche Seitenverhältnis und die Vorlage an.
* **Um [ALT-Text für Bilder in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klicken Sie auf ein Bild-Asset und verwenden Sie die Option _ALT-Text_, um manuell ALT-Text pro Bild hinzuzufügen oder zu generieren.
* **Um [Barrierefreiheitsbeschriftungen](/help/user-guide/create/manage-variants.md#add-accessibility-labels) zu Ihren Varianten hinzuzufügen,** Sie auf ein Bild oder einen call-to-action-Link und geben Sie dann eine kurze Beschreibung ein, die erklärt, was der Link oder die Schaltfläche bewirkt.
* **Um [Meta-Anzeige zu löschen](/help/user-guide/create/manage-variants.md#delete-variant)** klicken Sie auf das Optionsmenü für eine Variante und anschließend auf **[!UICONTROL Variante löschen]**.

### Videos verwalten

Bewegen Sie den Mauszeiger über die einzelnen Videos, um die schleifenförmige automatische Wiedergabe anzuzeigen.

Die Videos werden umrahmt, damit sie während der Erstellung dem ausgewählten Seitenverhältnis entsprechen. Kehren Sie zum ursprünglichen, nicht umrahmten Video zurück, indem Sie auf **[!UICONTROL Video umrahmen]** klicken und es deaktivieren.

## Feedback zur Senden-Generierung

Um [Feedback](/help/user-guide/create/manage-variants.md#generation-feedback) zur Qualität der Generierungsausgabe zu senden, klicken Sie auf das Optionssymbol (drei Punkte) und wählen Sie **[!UICONTROL Gute Ausgabe]** oder **[!UICONTROL Schlechte Ausgabe]**.

## Überprüfen der Ausrichtung der Inhaltsprüfung

Um die generierten Varianten zu optimieren und die strikte Einhaltung von Markenidentität, Plattformrichtlinien und Barrierefreiheitsstandards sicherzustellen, nutzen Sie die Leistungsfähigkeit des Bedienfelds [_Inhaltsprüfung_ ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Dieses Bedienfeld zeigt umfassende Details zur Inhaltsprüfung an und beleuchtet Bereiche mit Verbesserungsmöglichkeiten.

**So führen Sie Inhaltsprüfungen für eine Variante durch**:

1. Klicken Sie auf _Symbol für das Bedienfeld_ Inhaltsüberprüfung“ in der rechten Aktionsleiste, um das Bedienfeld [_Inhaltsüberprüfung_ zu ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Zeigen Sie eine Zusammenfassung der Prüfungen *Überprüfung erforderlich* und *bestanden* an, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   ![_Inhaltsüberprüfung_ Bedienfeld](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Varianten manuell überarbeiten](#revise-generated-variants) um sicherzustellen, dass Ihre Varianten eng mit den durchgeführten Inhaltsprüfungen abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

## Abrufen von Bewertungen und Genehmigungen

Verwenden Sie das Genehmigungsbedienfeld, das als Symbol in der rechten Aktionsleiste der Arbeitsfläche verfügbar ist, um Überprüfungen abzurufen, Kommentare zu Überprüfungen zu verfolgen und Genehmigungen von Stakeholdern zu erhalten.

**Um Bewertungen und Genehmigungen zu erhalten**:

1. [eine Genehmigungsanfrage starten](/help/user-guide/approvals/request-review.md) um eine [Genehmigung entworfener Meta-Anzeigen-Erlebnisse“ ](/help/user-guide/approvals/approve-content.md).

   ![Entwürfe zur Überprüfung und Genehmigung senden](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Entfernen oder Hinzufügen von Reviewern](/help/user-guide/approvals/review-and-edit.md#manage-approvals) während des Überprüfungsprozesses
1. [Zugriff auf den Inhalt zur Überprüfung](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) und Anzeigen der Überarbeitungsanfragen.
1. Bearbeiten Sie die Kommentare zu Entwürfen pro Überprüfung und [veröffentlichen Sie Ihre Meta-Anzeigenerlebnisse](#publish-and-export-experience).

Weitere Informationen finden [ unter ](/help/user-guide/approvals/overview.md) und Genehmigungen .

## Erlebnis veröffentlichen und exportieren

Um die generierten Meta-Anzeigen für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihre neue(n) Meta-Anzeige(**) zu veröffentlichen, klicken Sie auf **[!UICONTROL Veröffentlichen]** in der oberen Symbolleiste oder im Genehmigungsfluss.
1. **Um Ihre neue(n) Meta-Anzeige(**) zu exportieren, klicken Sie **[!UICONTROL der oberen Symbolleiste]** Exportieren“.
   1. Wählen Sie das Format aus (HTML und Bilder oder CSV und Bilder (JPG oder PNG)) und klicken Sie auf **[!UICONTROL Exportieren]**.

Weitere Informationen finden Sie unter [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) .

## Meta verbinden

Sie können GenStudio for Performance Marketing mit Meta verbinden, um erweiterte Analysen und Einblicke in die Content-Performance zu erhalten.

Siehe [Meta Ads Connect](/help/user-guide/connectors/meta-ads.md).
