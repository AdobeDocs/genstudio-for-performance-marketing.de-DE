---
title: Erstellen eines Bannererlebnisses
description: Erfahren Sie, wie Sie in Adobe Banner-Erlebnisse  [!DNL GenStudio]  Performance-Marketing erstellen.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c5d541a9-a97b-44da-a15c-61aceefd0e8c
source-git-commit: f49a2bd241f98dda23f6612f8c699ec49d222a12
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# Erstellen eines Bannererlebnisses

In diesem Tutorial erfahren Sie, wie Sie mit [ GenStudio for Performance Marketing-[[!DNL Create]](/help/user-guide/create/overview.md) (Paintbrush](banner-experiences.md)Symbol im linken Navigationsbereich) markenspezifische (Bannererlebnisse) erstellen.

Um ein ansprechendes Bannererlebnis zu gestalten, wird empfohlen, [GenStudio for Performance Marketing Richtlinien hinzuzufügen](/help/user-guide/guidelines/add-guidelines.md) und die [Grundlagen von Eingabeaufforderungen“ ](/help/user-guide/effective-prompts.md) lesen, bevor Sie beginnen.

## Vorlage wählen

Verwenden Sie zum Erstellen eines Bannererlebnisses eine verfügbare Vorlage, um das Framework für Ihren Inhalt bereitzustellen. Informationen [ unterstützten Bannerdimensionen finden Sie ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) „Best Practices für Vorlagen“.

**So wählen Sie eine Bannervorlage**:

1. Klicken Sie _[!DNL Create]_auf **[!UICONTROL Banner]**.
1. Verwenden Sie die Suchoption neben _Filter_, um eine bestimmte Bannervorlage zu finden.
1. Klicken _in der Ansicht_ Vorlage auswählen“ auf eine Bannervorlage.
1. Klicken Sie **[!UICONTROL Verwenden]**.

   Die Arbeitsfläche, die die Basis für die Inhaltserstellung ist, wird angezeigt.

## Parameter hinzufügen

Die Integration [Richtlinien](/help/user-guide/guidelines/overview.md) und Assets in _Parameter_ in der Eingabeaufforderungsschublade verbessert den Inhaltserstellungsprozess und ist ein wichtiger Vorbereitungsschritt für die Erstellung eines Bannererlebnisses.

**Hinzufügen von Parametern und Assets**:

1. Klicken Sie auf _Parameter_, um die Eingabeaufforderungsschublade zu erweitern.
1. Wählen Sie _Abschnitt_ Parameter“ Richtlinien - [!DNL Brands], [!DNL Personas] und [!DNL Products] - aus, um über die Inhaltserstellung zu informieren.

   Wenn in diesen Menüs keine Marken, Rollen oder Produkte verfügbar sind, [fügen Sie Ihrer GenStudio for Performance Marketing Richtlinien hinzu](/help/user-guide/guidelines/add-guidelines.md).

1. So fügen Sie Inhalte hinzu, die in den Erlebnissen (*) verwendet werden* beeinflussen die Inhaltserstellung:
   * Klicken Sie **[!UICONTROL Aus Inhalt auswählen]**, um Assets (Bilder) aus Ihrem [!DNL Content]-Repository auszuwählen, zu filtern und ein oder mehrere Bilder auszuwählen.

     Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie ein oder mehrere Bilder und wählen Sie sie aus.

   * Oder ziehen Sie Assets per Drag-and-Drop in den Abschnitt **[!UICONTROL Aus Inhalt auswählen]**, um ein oder mehrere neue Assets hochzuladen.
1. Klicken Sie **[!UICONTROL Verwenden]**.

Wenn Sie mit dem Hinzufügen von Parametern fertig sind, reduzieren Sie die Eingabeaufforderungsschublade, indem Sie erneut auf _Parameter_ klicken.

## Eingabeaufforderung eingeben

Nachdem Sie die Richtlinien ausgewählt haben, verwenden Sie die natürliche Sprache, um eine Eingabeaufforderung zu erstellen, um die Inhaltserstellung für Ihr neues Bannererlebnis einzuleiten. Um hochwertige Ergebnisse zu gewährleisten, ist es wichtig, Eingabeaufforderungen zu erstellen, die detailliert und beschreibend sind.

![Eingabeaufforderung eingeben](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Weitere [ zu Eingabeaufforderungen finden Sie ](/help/user-guide/effective-prompts.md)Schreiben effektiver Eingabeaufforderungen).

**So geben Sie eine Eingabeaufforderung ein**:

1. Geben Sie in das _„Beschreiben der Erlebnisse, die Sie generieren möchten“ eine Eingabeaufforderung_.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

Standardmäßig werden vier Varianten - angetrieben von der Eingabeaufforderung, Richtlinien und dem hinzugefügten Inhalt - generiert und auf der Arbeitsfläche angezeigt.

## Überarbeiten generierter Banner

Bevor Sie auswählen, was zur Genehmigung oder Veröffentlichung an [!DNL Content] gesendet werden soll, können Sie Bannerabschnitte und Textfelder bearbeiten oder eine generierte Variante löschen.

**Überarbeiten generierter Varianten**:

* **Um [ Namen des Bannerentwurfs zu bearbeiten](/help/user-guide/create/manage-variants.md#change-draft-name)** klicken Sie oben auf der Arbeitsfläche auf den Titel _Nicht benannter_&quot; und geben Sie einen neuen Titel ein.
* **Um [ Banner manuell zu bearbeiten](/help/user-guide/create/manage-variants.md#manually-edit-text)** doppelklicken Sie in einen der Bannerbereiche oder -felder (z. B. Überschrift oder CTA) und bearbeiten Sie es nach Bedarf.
* **Um [ Abschnitt einer Variante neu zu erstellen](/help/user-guide/create/manage-variants.md#re-generate-sections)** klicken Sie auf ein bearbeitbares Textfeld und verwenden Sie die _[!UICONTROL Vorgeschlagene Bearbeitungen]_ oder geben Sie eine neue Eingabeaufforderung im Abschnitt _[!UICONTROL Neuen Text generieren_ ein ] klicken Sie auf **[!UICONTROL Generieren]**.
* **Um [Bilder in einer Variante hinzuzufügen oder auszutauschen](/help/user-guide/create/manage-variants.md#swap-image)** klicken Sie auf ein Bild-Asset (oder den Bereich des Bild-Assets, wenn derzeit kein Bild vorhanden ist) und klicken Sie auf das Symbol **[!UICONTROL Austauschen]** Inhalt.
* **Um [einen Link zu einem Bild in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-image-link)** klicken Sie auf ein Bild-Asset (oder den Bereich des Bild-Assets, wenn derzeit kein Bild vorhanden ist) und klicken Sie auf das Link-Symbol.
* **Um [ALT-Text für Bilder in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klicken Sie auf ein Bild-Asset und verwenden Sie die Option _ALT-Text_, um manuell ALT-Text pro Bild hinzuzufügen oder zu generieren.
* **Um [Größe und Seitenverhältnis der Anzeige zu ändern](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klicken Sie auf die Schaltfläche _[!UICONTROL Größe ändern]_ (Feld mit einem Schaltflächensymbol auf der linken Seite der Arbeitsfläche) und wählen Sie eine neue Größe und ein neues Seitenverhältnis aus, das auf alle Varianten angewendet werden soll. Die Varianten werden dupliziert und in der Größe angepasst.
* **Um [ Bilder zuzuschneiden oder neu](/help/user-guide/create/manage-variants.md#crop-assets)** positionieren, bewegen Sie den Mauszeiger über das Bild, klicken Sie auf das angezeigte Zuschnittsymbol und passen Sie die Bildgröße und -platzierung an. Klicken Sie auf **[!UICONTROL Übernehmen]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Feedback zur Senden-Generierung

Um [Feedback](/help/user-guide/create/manage-variants.md#generation-feedback) zur Qualität der Generierungsausgabe zu senden, klicken Sie auf das Optionssymbol (drei Punkte) und wählen Sie **[!UICONTROL Gute Ausgabe]** oder **[!UICONTROL Schlechte Ausgabe]**.

## Überprüfen der Ausrichtung der Inhaltsprüfung

Um die generierten Varianten zu optimieren und die strikte Einhaltung von Markenidentität, Plattformrichtlinien und Barrierefreiheitsstandards sicherzustellen, nutzen Sie die Leistungsfähigkeit des Bedienfelds [_Inhaltsprüfung_ ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Dieses Bedienfeld zeigt umfassende Details zur Inhaltsprüfung an und beleuchtet Bereiche mit Verbesserungsmöglichkeiten.

**So führen Sie Inhaltsprüfungen für eine Variante durch**:

1. Klicken Sie auf _Symbol für das Bedienfeld_ Inhaltsüberprüfung“ in der rechten Aktionsleiste, um das Bedienfeld [_Inhaltsüberprüfung_ zu ](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Zeigen Sie eine Zusammenfassung der Prüfungen _Überprüfung erforderlich_ und _bestanden_ an, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   ![_Inhaltsüberprüfung_ Bedienfeld](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Varianten manuell überarbeiten](#revise-generated-variants) um sicherzustellen, dass Ihre Varianten eng mit den durchgeführten Inhaltsprüfungen abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

## Abrufen von Bewertungen und Genehmigungen

Verwenden Sie das _Genehmigungen_-Bedienfeld, das als Symbol in der rechten Aktionsleiste der Arbeitsfläche zugänglich ist, um Bewertungen abzurufen, Überprüfungskommentare zu verfolgen und Genehmigungen von Stakeholdern zu erhalten.

**Um Bewertungen und Genehmigungen zu erhalten**:

1. [eine Genehmigungsanfrage starten](/help/user-guide/approvals/request-review.md) um eine [Genehmigung entworfener Bannererlebnisse“ ](/help/user-guide/approvals/approve-content.md).
1. [Entfernen oder Hinzufügen von Reviewern](/help/user-guide/approvals/review-and-edit.md#manage-approvals) während des Überprüfungsprozesses
1. [Zugriff auf den Inhalt zur Überprüfung](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) und Anzeigen der Überarbeitungsanfragen.
1. Bearbeiten Sie die Kommentare zu Entwürfen pro Überprüfung und [veröffentlichen Sie Ihre Bannererlebnisse](#publish-and-export-experience).

Siehe [Überprüfungen und Genehmigungen](/help/user-guide/approvals/overview.md).

## Erlebnis veröffentlichen und exportieren

Um die generierten Banner für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihre neuen Banner-Erlebnisse zu veröffentlichen** klicken Sie in der oberen Symbolleiste oder **[!UICONTROL Genehmigungsfluss auf Veröffentlichen]**.
   1. Wählen Sie _[!UICONTROL [!DNL Campaigns]]_und fügen Sie_[!UICONTROL  Weitere Details ]_hinzu, falls gewünscht.
   1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

      ![Veröffentlichen eines Banners](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Um Ihre neuen Banner zu exportieren** klicken Sie in der oberen Symbolleiste **[!UICONTROL Exportieren]**.
   1. Wählen Sie das Format aus - HTML und Bilder, PNG oder JPG - und klicken Sie auf **[!UICONTROL Exportieren]**.

      Exportierte HTML sollten in einer vordefinierten Web-Eigenschaft platziert werden, z. B. einer Vorlage oder `div`. Ohne diese festgelegten Abmessungen können Bilder bei unabhängiger Betrachtung verzerrt erscheinen.

Siehe [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
