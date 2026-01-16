---
title: E-Mail-Erlebnis erstellen
description: Erfahren Sie, wie Sie E-Mail-Erlebnisse in Adobe GenStudio for Performance Marketing erstellen.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 168ea3d21f5771aeb05553ffe992dc9648b0e4e4
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# E-Mail-Erlebnis erstellen

In diesem Tutorial erfahren Sie, wie Sie mit [&#x200B; GenStudio for Performance Marketing &#x200B;](/help/user-guide/create/email-experiences.md) (Pinselsymbol im linken Navigationsbereich[[!DNL Create]](/help/user-guide/create/overview.md) markenspezifische E-Mail-Erlebnisse generieren können.

Um ein effektives E-Mail-Erlebnis zu schaffen, wird empfohlen, dass Sie [Richtlinien zu GenStudio for Performance Marketing hinzufügen](/help/user-guide/guidelines/add-guidelines.md) und die [Grundlagen der Erstellung einer Eingabeaufforderung) &#x200B;](/help/user-guide/effective-prompts.md), bevor Sie beginnen.

## Vorlage wählen

Um ein neues E-Mail-Erlebnis zu erstellen, verwenden Sie eine verfügbare Vorlage, um das Framework für Ihren Inhalt bereitzustellen.

**So wählen Sie eine E-Mail-Vorlage aus**:

1. Klicken Sie _[!DNL Create]_&#x200B;auf **[!UICONTROL E-Mail]**.
1. Verwenden Sie die Suchoption neben _Filter_, um eine bestimmte E-Mail-Vorlage zu finden.
1. Wählen Sie eine E-Mail-Vorlage aus und klicken Sie auf **[!UICONTROL Verwenden]**.

   Die Arbeitsfläche, das Epizentrum der Inhaltserstellung, wird angezeigt.

## Parameter hinzufügen

Das Hinzufügen [Richtlinien](/help/user-guide/guidelines/overview.md) und Assets in _Parameter_ in der Eingabeaufforderungsschublade lädt den Inhaltserstellungsprozess auf und ist ein integraler Vorbereitungsschritt für die Erstellung eines E-Mail-Erlebnisses.

Wenn Sie eine Vorlage mit vordefinierten Richtlinien (z. B. [!DNL Brands], [!DNL Personas] oder [!DNL Products]) verwenden, gelten diese Richtlinien für Ihre Varianten. Sie können sie bei Bedarf ändern.

**Hinzufügen von Parametern und Assets**:

1. Klicken Sie auf _Parameter_, um die Eingabeaufforderungsschublade zu erweitern.
1. Wählen Sie _Abschnitt_ Parameter“ Richtlinien - [!DNL Brands], [!DNL Personas] und [!DNL Products] - aus, um über die Inhaltserstellung zu informieren.

   ![Persona auswählen](/help/assets/persona-select-email2.png){width="300" align="center"}

   Wenn in diesen Menüs keine Marken, Rollen oder Produkte verfügbar sind, [fügen Sie Ihrer GenStudio for Performance Marketing Richtlinien hinzu](/help/user-guide/guidelines/add-guidelines.md).

1. Fügen Sie Inhalte für die Verwendung in der -Version *und* hinzu, um die Inhaltserstellung zu beeinflussen:
   * Klicken Sie **[!UICONTROL Aus Inhalt auswählen]**, um Assets (Bilder) aus Ihrem [!DNL Content]-Repository auszuwählen, zu filtern und ein oder mehrere Bilder auszuwählen.

     ![Auswählen visueller Inhalte](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Um Assets aus einem verbundenen [!DNL AEM Assets Content Hub]-Repository zu verwenden, wählen Sie ein Repository aus dem Dropdown-Menü _Speicherort_ aus. Filtern Sie ein oder mehrere Bilder und wählen Sie sie aus.

   * Oder ziehen Sie Assets per Drag-and-Drop in den Abschnitt **[!UICONTROL Aus Inhalt auswählen]**, um ein oder mehrere neue Assets hochzuladen.
1. Klicken Sie **[!UICONTROL Verwenden]**.

   >[!NOTE]
   >Wenn Ihre E-Mail-Vorlage mehrere Abschnitte enthält, wählen Sie [!DNL Products] und Inhalt (visuelle Assets) für jeden E-Mail-Abschnitt in _E-Mails mit mehreren Abschnitten_. E-Mails mit mehreren Abschnitten unterstützen ein visuelles Asset pro Abschnitt. Sie können visuelle Assets nur aus [!DNL Content] zu mehrteiligen E-Mails hinzufügen. Assets können nicht per Drag-and-Drop aus Ihrer lokalen Quelle gezogen oder hochgeladen werden.
   >![Fügen Sie Inhalt und Parameter für jeden E-Mail-Abschnitt hinzu](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

Wenn Sie mit dem Hinzufügen von Parametern fertig sind, können Sie die Eingabeaufforderungsschublade reduzieren, indem Sie erneut auf das Symbol _Parameter_ klicken.

## Eingabeaufforderung eingeben

Nachdem Richtlinien ausgewählt wurden, erstellen Sie eine Eingabeaufforderung mit natürlicher Sprache, um mit der Generierung von Inhalten für Ihr neues E-Mail-Erlebnis zu beginnen. Detaillierte Eingabeaufforderungen liefern eine höhere Qualität als vage oder mehrdeutige Eingabeaufforderungen.

Weitere [&#x200B; zu Eingabeaufforderungen finden Sie &#x200B;](/help/user-guide/effective-prompts.md)Schreiben effektiver Eingabeaufforderungen).

**So geben Sie eine Eingabeaufforderung ein**:

1. Geben Sie in das _„Beschreiben der Erlebnisse, die Sie generieren möchten“ eine Eingabeaufforderung_.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

Standardmäßig werden vier Varianten - alle basierend auf der Eingabeaufforderung, Richtlinien und hinzugefügten Inhalten - generiert und auf der Arbeitsfläche angezeigt.

Erzeugte Inhalte werden progressiv geladen : Wenn jeder Abschnitt der E-Mail-Erlebnisse generiert wird, erscheinen sie auf der Arbeitsfläche. Unter [E-Mail-Erlebnisse](/help/user-guide/create/meta-experiences.md#progressive-loading) erfahren Sie, wie diese Änderungen auf die Arbeitsfläche geladen werden.

## Überarbeiten generierter Varianten

Bevor Sie auswählen, was zur Genehmigung oder Veröffentlichung an [!DNL Content] gesendet werden soll, können Sie E-Mail-Abschnitte bearbeiten oder eine Variante aus dem Satz der generierten E-Mails löschen.

**Überarbeiten generierter Varianten**:

* **Um [&#x200B; E-Mail-Entwurfsnamen zu bearbeiten](/help/user-guide/create/manage-variants.md#change-draft-name)** klicken Sie auf den Titel _Nicht benannter_&quot; oben auf der Arbeitsfläche und geben Sie einen neuen Titel ein.
* **Um [E-Mail manuell zu bearbeiten](/help/user-guide/create/manage-variants.md#manually-edit-text)** klicken Sie in eines der bearbeitbaren Textfelder (z. B. Betreffzeile, Kopfzeile oder Textkörper) und bearbeiten Sie sie nach Bedarf
* **Um [Call to action zu ändern oder auszuwählen](/help/user-guide/create/manage-variants.md#revise-call-to-action)** klicken Sie auf die Schaltfläche call-to-action und wählen Sie _[!UICONTROL Umformulieren]_ oder _[!UICONTROL Link hinzufügen]_.
* **Um [&#x200B; Textformatierung anzuwenden](/help/user-guide/create/manage-variants.md#manually-edit-text)** in einer Variante klicken Sie auf den Nicht-Bild-Text für eine Variante und klicken Sie auf **[!UICONTROL Text formatieren]**.
* **Um [&#x200B; Abschnitt einer Variante neu zu erstellen](/help/user-guide/create/manage-variants.md#re-generate-sections)** klicken Sie auf ein bearbeitbares Textfeld und verwenden Sie die _[!UICONTROL Vorgeschlagene Bearbeitungen]_ oder geben Sie eine neue Eingabeaufforderung ein und klicken Sie auf **[!UICONTROL Generieren]**.
* **Um [Bilder in einer Variante hinzuzufügen oder auszutauschen](/help/user-guide/create/manage-variants.md#swap-image)** klicken Sie auf ein Bild-Asset (oder den Bereich des Bild-Assets, wenn derzeit kein Bild vorhanden ist) und klicken Sie auf das Symbol **[!UICONTROL Austauschen]** Inhalt.
* **Um [einen Link zu einem Bild in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-image-link)** klicken Sie auf ein Bild-Asset (oder den Bereich des Bild-Assets, wenn derzeit kein Bild vorhanden ist) und klicken Sie auf das Link-Symbol.
* **Um [ALT-Text für Bilder in einer Variante hinzuzufügen](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klicken Sie auf ein Bild-Asset und verwenden Sie die Option _ALT-Text_, um manuell ALT-Text pro Bild hinzuzufügen oder zu generieren.
* **Um [Barrierefreiheitsbeschriftungen](/help/user-guide/create/manage-variants.md#add-accessibility-labels) zu Ihren Varianten hinzuzufügen,** Sie auf ein Bild oder einen call-to-action-Link und geben Sie dann eine kurze Beschreibung ein, die erklärt, was der Link oder die Schaltfläche bewirkt.
* **Um [E-Mail zu löschen](/help/user-guide/create/manage-variants.md#delete-variant)** klicken Sie auf , um den E-Mail-Titel auszuwählen (z. B. „E-Mail 1/4„), und klicken Sie dann auf **[!UICONTROL Variante löschen]**.

## Feedback zur Senden-Generierung

Um [Feedback](/help/user-guide/create/manage-variants.md#generation-feedback) zur Qualität der Generierungsausgabe zu senden, klicken Sie auf das Optionssymbol (drei Punkte) und wählen Sie **[!UICONTROL Gute Ausgabe]** oder **[!UICONTROL Schlechte Ausgabe]**.

## Vorschau für Gerät

Beim Überarbeiten und Vorbereiten von E-Mail-Erlebnissen können Sie [zwischen Vorschauen für Desktop- und Mobilansichten wechseln](/help/user-guide/create/manage-variants.md#preview-for-device) um Kohärenz und visuelle Attraktivität von Entwurfsvarianten sicherzustellen.

## Überprüfen der Ausrichtung der Inhaltsprüfung

Um die generierten Varianten zu optimieren und die strikte Einhaltung von Markenidentität, Plattformrichtlinien und Barrierefreiheitsstandards sicherzustellen, nutzen Sie die Leistungsfähigkeit des Bedienfelds [_Inhaltsprüfung_ &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Dieses Bedienfeld zeigt umfassende Details zur Inhaltsprüfung an und beleuchtet Bereiche mit Verbesserungsmöglichkeiten.

**So führen Sie Inhaltsprüfungen für eine Variante durch**:

1. Klicken Sie auf _Symbol für das Bedienfeld_ Inhaltsüberprüfung“ in der rechten Aktionsleiste, um das Bedienfeld [_Inhaltsüberprüfung_ zu &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Zeigen Sie eine Zusammenfassung der Prüfungen *Überprüfung erforderlich* und *bestanden* an, um zu sehen, welche Abschnitte und Richtlinien verbessert werden müssen.

   ![_Inhaltsüberprüfung_ Bedienfeld](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Varianten manuell überarbeiten](#revise-generated-variants) um sicherzustellen, dass Ihre Varianten eng mit den durchgeführten Inhaltsprüfungen abgestimmt sind.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

## Abrufen von Bewertungen und Genehmigungen

Verwenden Sie das Genehmigungsbedienfeld, das als Symbol in der rechten Aktionsleiste der Arbeitsfläche verfügbar ist, um Überprüfungen abzurufen, Kommentare zu Überprüfungen zu verfolgen und Genehmigungen von Stakeholdern zu erhalten.

**Um Bewertungen und Genehmigungen zu erhalten**:

1. [eine Genehmigungsanfrage starten](/help/user-guide/approvals/request-review.md) um eine [Genehmigung entworfener E-Mail-Erlebnisse“ &#x200B;](/help/user-guide/approvals/approve-content.md).
1. [Entfernen oder Hinzufügen von Reviewern](/help/user-guide/approvals/review-and-edit.md#manage-approvals) während des Überprüfungsprozesses
1. [Zugriff auf den Inhalt zur Überprüfung](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) und Anzeigen der Überarbeitungsanfragen.
1. Bearbeiten Sie die Kommentare zu Entwürfen pro Überprüfung und [veröffentlichen Sie Ihre E-Mail-Erlebnisse](#publish-and-export-experience).

Weitere Informationen finden [&#x200B; unter &#x200B;](/help/user-guide/approvals/overview.md) und Genehmigungen .

## Erlebnis veröffentlichen und exportieren

Um die generierten E-Mails für die aktuelle und zukünftige Verwendung verfügbar zu machen, veröffentlichen Sie sie in [!UICONTROL Inhalt] und exportieren Sie sie zur Verwendung in Ihren Marketing-Kampagnen.

1. **Um Ihre neuen E-Mail-Erlebnisse zu veröffentlichen** klicken Sie auf **[!UICONTROL Veröffentlichen]** in der oberen Symbolleiste oder im Genehmigungsfluss.
1. **Um Ihre neuen E-Mail-Erlebnisse zu exportieren** klicken Sie in der oberen Symbolleiste **[!UICONTROL Exportieren]**.
   1. Wählen Sie das Format aus (nur CSV und Bilder oder HTML) und klicken Sie auf **[!UICONTROL Exportieren]**.

Weitere Informationen finden Sie unter [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) .
