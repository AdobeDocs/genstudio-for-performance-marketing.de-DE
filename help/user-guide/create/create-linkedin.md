---
title: Erstellen eines LinkedIn-Erlebnisses
description: Erfahren Sie, wie Sie mit Adobe GenStudio for Performance Marketing markenkonforme LinkedIn-Erlebnisse erstellen.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: 6c2a8ca1fd981bc4f6eb15f1487b304c0c8f67b4
workflow-type: tm+mt
source-wordcount: '1224'
ht-degree: 0%

---

# Erstellen eines LinkedIn-Erlebnisses

In diesem Tutorial erfahren Sie, wie Sie [LinkedIn-Erlebnisse](/help/user-guide/create/meta-experiences.md) generieren, die Ihren Markenrichtlinien entsprechen, mithilfe von GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (Pinselsymbol im linken Navigationsbereich).

Bevor Sie mit der Erstellung einer LinkedIn-Anzeige beginnen, ist es wichtig, [Richtlinien hinzufügen](/help/user-guide/guidelines/add-guidelines.md) in GenStudio for Performance Marketing kennenzulernen und die Grundlagen zum [&#x200B; einer Eingabeaufforderung &#x200B;](/help/user-guide/effective-prompts.md).

## Vorlage wählen

Um ein neues LinkedIn-Erlebnis zu generieren, benötigen Sie eine Vorlage, die das Framework für Ihre Inhalte bereitstellt. Informationen [&#x200B; unterstützten LinkedIn](/help/user-guide/templates/linkedin-template.md)Seitenverhältnisse finden Sie unter „LinkedIn-Vorlagenrichtlinien“.

Sie können aus Ihrer Liste benutzerdefinierter Vorlagen auswählen oder eine erste Vorlage auswählen.

**So wählen Sie eine LinkedIn-Vorlage aus**:

1. Klicken Sie _[!DNL Create]_&#x200B;auf **[!UICONTROL LinkedIn]**.
1. Wählen Sie **[!UICONTROL Benutzerdefinierte Vorlagen]** aus, um Ihre hochgeladenen Vorlagen zu durchsuchen, oder **[!UICONTROL Startervorlagen]**, um die vordefinierten Vorlagen zu durchsuchen.

   Wenn Sie Video-Assets zu Ihren Meta-Varianten hinzufügen möchten, müssen Sie eine Startvorlage auswählen. Sie sind mit systemdefinierten Inhaltsbereichen vorgeladen, die die Verwendung von Videos erleichtern.

1. Klicken Sie auf eine Vorlage, um sie auszuwählen, und klicken Sie auf **[!UICONTROL Verwenden]**.

   Diese Aktion öffnet die Arbeitsfläche, die den zentralen Hub für die Inhaltserstellung darstellt.

## Parameter hinzufügen

Das Hinzufügen [Richtlinien](/help/user-guide/guidelines/overview.md) und Assets in _Parameter_ in der Eingabeaufforderungsschublade verbessert den Inhaltserstellungsprozess und ist ein wichtiger Schritt bei der Vorbereitung zum Generieren eines LinkedIn-Erlebnisses.

**Hinzufügen von Parametern und Assets**:

1. Klicken Sie auf _Parameter_, um die Eingabeaufforderungsschublade zu erweitern.
1. Wählen Sie _Abschnitt_ Parameter“ Richtlinien - [!DNL Brands], [!DNL Personas] und [!DNL Products] - aus, um über die Inhaltserstellung zu informieren.

   ![Persona auswählen](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Wenn in diesen Menüs keine Marken, Rollen oder Produkte verfügbar sind, [fügen Sie Ihrer GenStudio for Performance Marketing Richtlinien hinzu](/help/user-guide/guidelines/add-guidelines.md).

1. Fügen Sie Inhalte (Bilder oder Videos) für die Verwendung im Erlebnis hinzu *und* um die Inhaltserstellung zu beeinflussen, indem Sie auf **[!UICONTROL Aus Inhalt auswählen]** klicken. Oder ziehen Sie Bilder per Drag-and-Drop in den **[!UICONTROL Aus Inhalt auswählen]**, um ein oder mehrere neue Assets hochzuladen.

   Verwenden Sie den Filter, um nach Inhalten zu suchen und ein oder mehrere Bilder auszuwählen.

   Wenn Sie eine Vorlage mit einem Abschnitt für Videos verwenden, werden Videoinhalte (.mp4) vorausgewählt und für Sie gefiltert. Bewegen Sie den Mauszeiger über ein Video, um eine automatisch wiedergegebene Vorschau anzuzeigen.

   ![Auswählen visueller Inhalte](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

   Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie ein oder mehrere Bilder und wählen Sie sie aus.

1. Klicken Sie **[!UICONTROL Verwenden]**.

Wenn Sie mit dem Hinzufügen von Parametern fertig sind, können Sie die Eingabeaufforderungsschublade reduzieren, indem Sie erneut auf das Symbol _Parameter_ klicken.

## Eingabeaufforderung eingeben

Nachdem Sie Richtlinien ausgewählt haben, erstellen Sie eine Eingabeaufforderung mit natürlicher Sprache, um mit der Erstellung von Inhalten für Ihr neues LinkedIn-Erlebnis zu beginnen. Detaillierte Eingabeaufforderungen stellen sicher, dass Sie eine gute Qualität und nützliche Ausgabe erhalten.

Weitere [&#x200B; zu Eingabeaufforderungen finden Sie &#x200B;](/help/user-guide/effective-prompts.md)Schreiben effektiver Eingabeaufforderungen).

**So geben Sie eine Eingabeaufforderung ein**:

1. Geben Sie in das _„Beschreiben der Erlebnisse, die Sie generieren möchten“ eine Eingabeaufforderung_.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

   Unter [Verwalten von Videos](#manage-videos) erfahren Sie, wie sie generiert werden und wie Sie sie verwalten.

Standardmäßig werden vier Varianten - alle basierend auf der Eingabeaufforderung, Richtlinien und hinzugefügten Inhalten - generiert und auf der Arbeitsfläche angezeigt.

Erzeugte Inhalte werden progressiv geladen : Wenn jeder Abschnitt der LinkedIn-Erlebnisse generiert wird, erscheinen sie auf der Arbeitsfläche. Unter [LinkedIn-Erlebnisse](/help/user-guide/create/linkedin-experiences.md#progressive-loading) erfahren Sie, wie diese Änderungen auf die Arbeitsfläche geladen werden.

## Generierte LinkedIn-Anzeigen überarbeiten

Bevor Sie Varianten zur Genehmigung oder Veröffentlichung an [!DNL Content] senden, können Sie die LinkedIn-Anzeigen bearbeiten oder eine Variante aus dem Satz der generierten Anzeigen löschen.

**Überarbeiten generierter Varianten**:

* **Um [&#x200B; Namen des LinkedIn-Anzeigenentwurfs zu bearbeiten](/help/user-guide/create/manage-variants.md#change-draft-name)** klicken Sie oben auf der Arbeitsfläche auf den Titel _Nicht benannter_&quot; und geben Sie einen neuen Titel ein.
* **Um [&#x200B; LinkedIn-Anzeige manuell zu bearbeiten](/help/user-guide/create/manage-variants.md#manually-edit-text)** klicken Sie auf einen der Anzeigenabschnitte (z. B. die Betreffzeile, die Kopfzeile oder die Textkörper-Kopie) und bearbeiten Sie ihn nach Bedarf.
* **Um die call to action zu ändern oder auszuwählen** klicken Sie auf die Schaltfläche call-to-action und wählen Sie aus den verfügbaren Textoptionen für die Schaltfläche aus. Geben _unter_ eine URL für den call-to-action-Text ein.
* **Um [&#x200B; Textformatierung anzuwenden](/help/user-guide/create/manage-variants.md#manually-edit-text)** in einer Variante klicken Sie auf den Nicht-Bild-Text für eine Variante und klicken Sie auf **[!UICONTROL Text formatieren]**.
* **Um [&#x200B; Abschnitt einer Variante neu zu erstellen](/help/user-guide/create/manage-variants.md#re-generate-sections)** klicken Sie auf ein bearbeitbares Textfeld und verwenden Sie die _[!UICONTROL Vorgeschlagene Bearbeitungen]_ oder geben Sie eine neue Eingabeaufforderung im Abschnitt _[!UICONTROL Neuen Text generieren_ ein &#x200B;] klicken Sie auf **[!UICONTROL Generieren]**.
* **Um [Generative Erweitern zu verwenden, um Bilder zu &#x200B;](/help/user-guide/create/manage-variants.md#use-generative-expand) und an Ihre Arbeitsvorlage anzupassen** klicken Sie auf ein Bild, klicken Sie auf **[!UICONTROL Bearbeiten]** (Bleistiftsymbol) und dann auf **[!UICONTROL Erweitern]**. Passen Sie das Bild an das erforderliche Seitenverhältnis und die Vorlage an.
* **Um Bilder [zuzuschneiden oder neu zu positionieren](/help/user-guide/create/manage-variants.md#crop-assets)** bewegen Sie den Mauszeiger über ein Bild, klicken Sie auf das angezeigte Zuschnittssymbol und passen Sie die Bildgröße und -platzierung an.
* **Um [Größe und Seitenverhältnis der Anzeige zu ändern](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klicken Sie auf die Schaltfläche _[!UICONTROL Größe ändern]_ (Feld mit einem Schaltflächensymbol auf der linken Seite der Arbeitsfläche) und wählen Sie eine neue Größe und ein neues Seitenverhältnis aus, das auf alle Varianten angewendet werden soll. Die Varianten werden dupliziert und in der Größe angepasst.
* **Um Assets (Bild oder Video) in einer Variante [hinzuzufügen oder auszutauschen](/help/user-guide/create/manage-variants.md#swap-image)** klicken Sie auf ein Asset (oder den Asset-Bereich) und klicken Sie auf das Symbol **[!UICONTROL Aus Inhalt austauschen]**.
* **Um [ALT-Text für Bilder in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klicken Sie auf ein Bild-Asset und verwenden Sie die Option _ALT-Text_, um manuell ALT-Text pro Bild hinzuzufügen oder zu generieren.
* **Um [Barrierefreiheitsbeschriftungen](/help/user-guide/create/manage-variants.md#add-accessibility-labels) zu Ihren Varianten hinzuzufügen,** Sie auf ein Bild oder einen call-to-action-Link und geben Sie dann eine kurze Beschreibung ein, die erklärt, was der Link oder die Schaltfläche bewirkt.
* **Um [&#x200B; LinkedIn-Anzeige zu löschen](/help/user-guide/create/manage-variants.md#delete-variant)** klicken Sie auf das Optionsmenü für eine Variante und anschließend auf **[!UICONTROL Variante löschen]**.

### Videos verwalten

Bewegen Sie den Mauszeiger über die einzelnen Videos, um die schleifenförmige automatische Wiedergabe anzuzeigen.

Die Videos werden umrahmt, damit sie während der Erstellung dem ausgewählten Seitenverhältnis entsprechen. Kehren Sie zum ursprünglichen, nicht umrahmten Video zurück, indem Sie auf **[!UICONTROL Video umrahmen]** klicken und es deaktivieren.

## Feedback zur Senden-Generierung

Um [Feedback](/help/user-guide/create/manage-variants.md#generation-feedback) zur Qualität der Generierungsausgabe zu senden, klicken Sie auf das Optionssymbol (drei Punkte) und wählen Sie **[!UICONTROL Gute Ausgabe]** oder **[!UICONTROL Schlechte Ausgabe]**.

## Überprüfen der Ausrichtung der Inhaltsprüfung

Um die generierten Varianten zu optimieren und die strikte Einhaltung von Markenidentität, Plattformrichtlinien und Barrierefreiheitsstandards sicherzustellen, nutzen Sie die Leistungsfähigkeit des Bedienfelds [_Inhaltsprüfung_ &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Dieses Bedienfeld zeigt umfassende Details zur Inhaltsprüfung an und beleuchtet Bereiche mit Verbesserungsmöglichkeiten.

**So führen Sie Inhaltsprüfungen für eine Variante durch**:

1. Klicken Sie auf _Symbol für das Bedienfeld_ Inhaltsüberprüfung“ in der rechten Aktionsleiste, um das Bedienfeld [_Inhaltsüberprüfung_ zu &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Zeigen Sie eine Zusammenfassung der Prüfungen *Überprüfung erforderlich* und *bestanden* an, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   ![_Inhaltsüberprüfung_ Bedienfeld](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Varianten manuell überarbeiten](#revise-generated-linkedin-ads) um sicherzustellen, dass Ihre Varianten eng mit den dann abgeschlossenen Inhaltsprüfungen abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

## Abrufen von Bewertungen und Genehmigungen

Verwenden Sie das Bedienfeld Genehmigungen , auf das über die obere Menüleiste der Arbeitsfläche zugegriffen werden kann, um Überprüfungen abzurufen, Kommentare zu überprüfen und Genehmigungen von Stakeholdern abzurufen.

**Um Bewertungen und Genehmigungen zu erhalten**:

1. [eine Genehmigungsanfrage starten](/help/user-guide/approvals/request-review.md) um eine [Genehmigung entworfener Meta-Anzeigen-Erlebnisse“ &#x200B;](/help/user-guide/approvals/approve-content.md).

   ![Entwürfe zur Überprüfung und Genehmigung senden](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Entfernen oder Hinzufügen von Reviewern](/help/user-guide/approvals/review-and-edit.md#manage-approvals) während des Überprüfungsprozesses
1. [Zugriff auf den Inhalt zur Überprüfung](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) und Anzeigen der Überarbeitungsanfragen.
1. Bearbeiten Sie die Kommentare zu Entwürfen pro Überprüfung und [veröffentlichen Sie Ihre Meta-Anzeigenerlebnisse](#publish-and-export-experience).

Weitere Informationen finden [&#x200B; unter &#x200B;](/help/user-guide/approvals/overview.md) und Genehmigungen .

## Erlebnis veröffentlichen und exportieren

Um die generierten LinkedIn-Anzeigen für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihr(e) neue(s) Erlebnis(**) zu veröffentlichen, klicken **[!UICONTROL in der oberen Symbolleiste auf]** Veröffentlichen“ oder im Genehmigungsfluss.
1. **Um Ihre neuen Erlebnisse zu exportieren** klicken Sie in der oberen Symbolleiste **[!UICONTROL Exportieren]**.
   1. Wählen Sie das Format aus - JPG, PNG oder GIF - und klicken Sie auf **[!UICONTROL Exportieren]**.

Weitere Informationen finden Sie unter [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) .
