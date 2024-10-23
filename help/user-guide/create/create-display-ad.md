---
title: Erstellen eines Display-Anzeigenerlebnisses
description: Erfahren Sie, wie Sie Display-Anzeigenerlebnisse in Adobe [!DNL GenStudio] für Performance-Marketing erstellen.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 816aeb55eee92758e7ef022ced0ebc3308d27dc9
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Erstellen eines Display-Anzeigenerlebnisses

In diesem Tutorial erfahren Sie, wie Sie mit GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (Paintbrush-Symbol im linken Navigationsbereich) mit dem Branding [Display-Anzeigenerlebnisse](display-ad-experiences.md) generieren.

Um ein überzeugendes Display-Anzeigenerlebnis zu entwerfen, sollten Sie [GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) Richtlinien hinzufügen und die [Grundlagen der Schreibaufforderungen](/help/user-guide/effective-prompts.md) überprüfen, bevor Sie beginnen.

## Vorlage auswählen

Verwenden Sie zum Erstellen eines Display-Anzeigenerlebnisses eine verfügbare Vorlage, um das Framework für Ihren Inhalt bereitzustellen.

**So wählen Sie eine Display-Anzeigenvorlage aus**:

1. Klicken Sie in &quot;_[!DNL Create]_&quot;unter &quot;_&quot;Was möchten Sie heute erstellen&quot;auf &quot;**[!UICONTROL Anzeigen anzeigen]**&quot;.Abschnitt &quot;_&quot;.
1. Verwenden Sie die Suchoption neben _Filter_ , um eine bestimmte Display-Anzeigenvorlage zu finden.
1. Klicken Sie in der Ansicht _Vorlage auswählen_ auf eine Display-Anzeigenvorlage.
1. Klicken Sie auf **[!UICONTROL Use]**.

   Die Arbeitsfläche, die als zentrale Schnittstelle für die Inhaltserstellung dient, wird angezeigt.

## Parameter hinzufügen

Durch das Hinzufügen von [Führungslinien](/help/user-guide/guidelines/overview.md) und Assets in _Parameter_ in der Eingabeaufforderung wird der Inhaltserstellungsvorgang überschrieben. Dies ist ein integraler vorbereitender Schritt zum Generieren eines Display-Anzeigenerlebnisses.

**Hinzufügen von Parametern und Assets**:

1. Klicken Sie auf das Symbol _Parameter_ , um die Eingabeaufforderung zu erweitern.
1. Wählen Sie im Abschnitt _Parameter_ die Richtlinien [!DNL Brands], [!DNL Personas] und [!DNL Products] aus, um die Inhaltserstellung zu informieren.

   Wenn in diesen Menüs keine Marken, Personas oder Produkte verfügbar sind, fügt [Ihrer GenStudio Richtlinien für Performance-Marketing hinzu](/help/user-guide/guidelines/add-guidelines.md).

1. So fügen Sie Inhalte hinzu, die im Erlebnis *und* verwendet werden, um die Inhaltserstellung zu beeinflussen:
   * Klicken Sie auf **[!UICONTROL Aus Inhalt auswählen]** , um Assets (Bilder) aus Ihrem [!DNL Content]-Repository auszuwählen, ein oder mehrere Bilder zu filtern und auszuwählen.

     Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Position_ aus. Filtern und wählen Sie ein oder mehrere Bilder aus.

   * Alternativ können Sie Assets per Drag-and-Drop in den Abschnitt **[!UICONTROL Aus Inhalt auswählen]** ziehen, um ein oder mehrere neue Assets hochzuladen.
1. Klicken Sie auf **[!UICONTROL Use]**.

Wenn Sie alle Parameter hinzugefügt haben, reduzieren Sie die Eingabeaufforderung, indem Sie erneut auf das Symbol _Parameter_ klicken.

## Eingabeaufforderung eingeben

Nachdem Richtlinien ausgewählt wurden, erstellen Sie eine Eingabeaufforderung mit natürlicher Sprache, um Inhalte für Ihr neues Display-Anzeigenerlebnis zu generieren. Um die Qualität der generierten Display-Anzeigenerlebnisse zu verbessern, ist es wichtig, detaillierte und beschreibende Aufforderungen zu erstellen.

![Geben Sie eine Eingabeaufforderung ein](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Weitere Informationen zum Schreiben von Eingabeaufforderungen finden Sie unter [Gültige Eingabeaufforderungen schreiben](/help/user-guide/effective-prompts.md) .

**So geben Sie eine Eingabeaufforderung ein**:

1. Geben Sie in das Eingabeaufforderungsfeld _&quot;Beschreiben Sie die Erlebnisse, die Sie generieren möchten&quot;_ eine Eingabeaufforderung ein.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

Standardmäßig wird eine Variante - basierend auf der Eingabeaufforderung, den Richtlinien und dem hinzugefügten Inhalt - generiert und auf der Arbeitsfläche angezeigt.

## Generierte Display-Anzeigen überarbeiten

Bevor Sie auswählen, was Sie zur Genehmigung oder Veröffentlichung an [!DNL Content] senden möchten, können Sie die Abschnitte der Display-Anzeige und die Textfelder bearbeiten oder eine generierte Variante löschen.

**So überarbeiten Sie generierte Varianten**:

* **Um [den Namen des Anzeigeentwurfs zu bearbeiten, klicken Sie auf den Titel _Unbenannter Entwurf_ oben auf der Arbeitsfläche und geben Sie einen neuen Titel ein.](/help/user-guide/create/manage-variants.md#change-draft-name)**
* **Um [eine Display-Anzeige manuell zu bearbeiten](/help/user-guide/create/manage-variants.md#manually-edit-text)**, doppelklicken Sie auf einen der Bereiche oder Felder der Display-Anzeige (z. B. die Betreffzeile, Kopfzeile oder Textkopie) und bearbeiten Sie sie nach Bedarf.
* **Ändern Sie in [ Größe und Seitenverhältnis der Anzeige.](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** Klicken Sie auf die Schaltfläche _[!UICONTROL Größe ändern]_ (Feld mit einem Schaltflächensymbol auf der linken Seite der Arbeitsfläche) und wählen Sie eine neue Größe und ein neues Seitenverhältnis aus, die auf alle Varianten angewendet werden sollen. Die Varianten werden dupliziert und die Größe wird angepasst.
* **Um [Bilder zu beschneiden oder neu zu positionieren](/help/user-guide/create/manage-variants.md#crop-assets)**, bewegen Sie den Mauszeiger über das Bild, klicken Sie auf das angezeigte Zuschnittsymbol und passen Sie die Bildgröße und -platzierung an. Klicken Sie auf **[!UICONTROL Übernehmen]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Feedback zur Sendegenerierung

Um [Feedback zur Qualität der Generierungsausgabe zu senden](/help/user-guide/create/manage-variants.md#generation-feedback), klicken Sie auf das Optionssymbol (drei Punkte) und wählen Sie **[!UICONTROL Gute Ausgabe]** oder **[!UICONTROL Schlechte Ausgabe]** aus.

## Markenausrichtung überprüfen

Um die generierten Anzeigen zu optimieren und die strikte Einhaltung der Markenidentität sicherzustellen, nutzen Sie die Leistungsfähigkeit des [_Markenvalidierungs-Panels_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel), das umfassende Details zur Markenvalidierung anzeigt und Verbesserungsbereiche beleuchtet.

**Überprüfen der Markenausrichtung**:

1. Klicken Sie in der oberen Menüleiste auf das Symbol für die Markenvalidierung, um das Fenster [_Markenvalidierung_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) zu öffnen. Sie können Details zu den Fragmenten und Richtlinien sehen, die verbessert werden müssen.

1. Schalten Sie durch die einzelnen Anzeigen, um zu sehen, wie Sie den generierten Inhalt verbessern können, um markengerechter zu werden.
1. [Passen Sie Anzeigen manuell an](#revise-generated-display-ads), um sicherzustellen, dass Ihre E-Mails eng mit Ihrer Marke abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

## Prüfungen und Genehmigungen abrufen

Verwenden Sie das Bedienfeld Genehmigungen , auf das Sie in der oberen Menüleiste der Arbeitsfläche zugreifen können, um Bewertungen zu erhalten, Kommentare zu Überprüfungen zu verfolgen und Genehmigungen von Interessenträgern zu erhalten.

**So rufen Sie Bewertungen und Genehmigungen ab**:

1. [Starten Sie eine Genehmigungsanfrage](/help/user-guide/approvals/request-review.md), um eine [Genehmigung entworfener E-Mail-Erlebnisse zu erhalten.](/help/user-guide/approvals/approve-content.md)
1. [Entfernen oder fügen Sie während des Überprüfungsprozesses Überprüfer hinzu](/help/user-guide/approvals/review-and-edit.md#manage-approvals).
1. [Greifen Sie auf den Inhalt für die Überprüfung zu](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) und zeigen Sie die Anforderungen für die Überarbeitung an.
1. Bearbeiten Sie die Entwürfe pro Prüfungskommentar und [veröffentlichen Sie Ihre Display-Anzeigenerlebnisse](#publish-and-export-experience).

Siehe [Überprüfungen und Genehmigungen](/help/user-guide/approvals/overview.md).

## Publish- und Exporterlebnis

Um die generierten Display-Anzeigen für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihre neuen Display-Anzeigenerlebnisse zu veröffentlichen, klicken Sie in der oberen Symbolleiste oder im Genehmigungsfluss auf**[!UICONTROL  Publish ]**.**
   1. Wählen Sie _[!UICONTROL [!DNL Campaigns]]_aus und fügen Sie bei Bedarf_[!UICONTROL  Weitere Details ]_hinzu.
   1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

      ![Publish einer Display-Anzeige](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Um Ihre neuen Display-Anzeigenerlebnisse zu exportieren, klicken Sie in der oberen Symbolleiste auf**[!UICONTROL  Exportieren ]**.**
   1. Wählen Sie das Format - nur JPG - und klicken Sie auf **[!UICONTROL Exportieren]**.

Siehe [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
