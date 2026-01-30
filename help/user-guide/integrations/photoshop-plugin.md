---
title: Photoshop-Plug-in für Adobe GenStudio for Performance Marketing
description: Erfahren Sie, wie Sie das Photoshop-Plug-in für GenStudio for Performance Marketing installieren, konfigurieren und verwenden.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# Photoshop-Plug-in für GenStudio for Performance Marketing

Das GenStudio for Performance Marketing Photoshop-Plug-in fügt ein Bedienfeld zu Adobe Photoshop hinzu, mit dem Sie markeninterne Inhalte generieren können.

Auf dieser Seite wird beschrieben, wie Sie das Plug-in installieren und konfigurieren und verwenden.

Zu den Funktionen dieses Plug-ins gehören:

* Melden Sie sich bei einer GenStudio for Performance Marketing-Instanz mit einer Adobe ID an
* Zuordnen von GenStudio for Performance Marketing-Feldern zur Inhaltserstellung zu Textebenen in einem Photoshop-Dokument
* Geben Sie eine Marke, ein Produkt, eine Rolle und eine Eingabeaufforderung zum Generieren von Inhalten an
* Optional können Sie ein Bild hinzufügen, um Ihr Vorlagenbild zu ersetzen
* Vorschau generierter On-Brand-Inhaltsvarianten
* Anwenden von generiertem Inhalt auf zugeordnete Ebenen im aktuellen Dokument
* Erstellen von Übersetzungen markeninterner Inhalte
* Generierte [!DNL Experiences] nach GenStudio for Performance Marketing exportieren

>[!VIDEO](https://video.tv.adobe.com/v/3478829?captions=ger&learn=on)

## Installieren des Plug-ins

Folgen Sie diesen Anweisungen, um das Plug-in zu installieren.

### Voraussetzungen

* Creative Cloud Desktop-Programm
* Photoshop, Mindestversion 25.6.0

### Installationsschritte

1. Laden Sie das Plug-in vom Creative Cloud Marketplace in Adobe Exchange herunter und aktualisieren Sie es.
1. Suchen Sie in Adobe Exchange nach dem **GenStudio-Plug** in für Photoshop.
1. Befolgen Sie die Anweisungen, um das Plug-in zu installieren.

### Deinstallieren des Plug-ins

1. Starten Sie das Creative Cloud-Desktop-Programm.
1. Klicken Sie auf die Option **[!UICONTROL Plug-ins]**.
1. Klicken Sie auf der Karte GenStudio für Creative Cloud auf die Auslassungspunkte **[!UICONTROL (…]**, um weitere Optionen anzuzeigen.
1. Wählen Sie **Deinstallieren**.

## Erstellen einer Vorlage

Um Inhalte zu generieren, benötigen Sie eine GenStudio for Performance Marketing-Vorlage, die aus Ihrem Photoshop-Dokument erstellt wurde.

So erstellen Sie eine GenStudio-fähige Vorlage:

1. Öffnen Sie ein Dokument in Photoshop.
1. Identifizieren Sie eine Textebene für generierte Inhalte.
1. Benennen Sie die Ebene mit dem Konventionsformat des Feldnamens um: `{<name_of_generated_field>}`. Beispiel: `{body}`, `{headline}`, `{cta}`.
1. Umbenennen von Ebenen für alle [Felder, die für den Kanal erforderlich sind, der für den Vorlagentyp bestimmt ist](../../user-guide/templates/customize-template.md#recognized-field-names).

| Kanal | Erforderliche Felder für die Generierung | Optionale Felder für die Generierung |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| Anzeige | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

Beachten Sie, dass mehrere Ebenen dieselbe Feldbezeichnung teilen können, aber jede Ebene nur ein Feld angeben kann. Wenn das Dokument beispielsweise mehrere Zeichenflächen enthält:

* Sie können in jeder Zeichenfläche eine `{headline}` festlegen.
* Sie können mehrere `{headline}` Ebenen in einer Zeichenfläche angeben.
* Sie können nicht angeben, dass eine einzelne Ebene sowohl die `{headline}`- als auch die `{cta}` Feldnamen erhält.

### Anforderungen an die Vorlagengröße

#### Meta-Vorlagen

Für Instagram- und Facebook-Posts:

* Breite: 1080 px (fest)
* Höhe: 1080 px oder 1350 px

Für Instagram- und Facebook-Stories:

* Breite: 1080 px (fest)
* Höhe: 1920 px

Das -Plug-in bestimmt das Chrom des generierten Erlebnisses anhand der Höhe der Vorlage.

#### Vorlagen anzeigen

Es gibt keine Anforderung für eine feste Größe. Anzeigevorlagen unterstützen jede Größe.

#### LinkedIn-Vorlagen

* Breite: 1200 px (fest)
* Höhe: 1200 px, 628 px, 2292 px, 1800 px oder 1500 px

Das Dokument kann jetzt mit dem Plug-in verwendet werden.

## Neuen Inhalt generieren

1. Öffnen Sie Photoshop.
1. Öffnen Sie ein von Ihnen erstelltes GenStudio-fähiges Vorlagendokument (siehe Anweisungen oben) oder verwenden Sie die GenStudio for Performance Marketing Starter-Vorlage: `branding-template-acrobat-handlebars.psd`.
1. Öffnen Sie das Plug-in-Bedienfeld unter **[!UICONTROL Plug-ins]** > **[!UICONTROL GenStudio]**.
1. Klicken Sie auf **[!UICONTROL Schaltfläche &quot;]**&quot;. Wenn Sie nach der Berechtigung zum Öffnen einer URL gefragt werden, aktivieren Sie optional **Merken nach Auswahl** und klicken Sie dann auf **[!UICONTROL Zulassen]**.
1. Verwenden Sie den Webbrowser, um sich mit einem Profil anzumelden, das Zugriff auf GenStudio for Performance Marketing hat.
1. Wählen Sie den Kanal (Meta, LinkedIn oder Display) aus, der für die geöffnete Vorlage gilt.
   ![Kanalauswahl](./ps-select-channel.png){width="300" zoomable="yes"}
1. Wählen Sie den [!DNL Brand]-, [!DNL Persona]- und [!DNL Product] für die Inhaltserstellung aus.
   ![Marke, Rolle und Produktauswahl](./ps-select-box.png){width="300" zoomable="yes"}
1. Wählen Sie die Anzahl der zu erstellenden Varianten aus.
1. Verwenden Sie die Schaltfläche unter **[!UICONTROL Inhalt auswählen]**, um Bilder aus Ihren Assets zu suchen und auszuwählen. Die 40 zuletzt hinzugefügten Assets werden zuerst angezeigt, und Sie können nach anderen Assets suchen. Die Größe der ausgewählten Bilder wird automatisch an die Vorlagen angepasst.
1. Geben Sie eine Textaufforderung für den Inhalt im Feld **[!UICONTROL Textaufforderung]** an.
1. Klicken Sie auf die **[!UICONTROL Generieren]**-Schaltfläche. Varianten werden auf Karten im Plug-in-Bedienfeld angezeigt.

Neue Dokumente werden Ihrem Photoshop-Arbeitsbereich hinzugefügt, wobei die generierten Inhalte auf die Vorlagenfelder angewendet werden. Diese Dokumente werden mit einem nummerierten Variantensuffix benannt.

## Inhalte übersetzen

Benutzer können Inhalte nach der Erstellung einer Kopie in unterstützte Sprachen übersetzen.

1. Klicken Sie auf **[!UICONTROL Übersetzen]**, nachdem Sie eine Anzeigenkopie mit dem Plug-in erstellt haben.
1. Eine oder mehrere Sprachen für die Übersetzung auswählen.
1. Klicken Sie auf **[!UICONTROL Übersetzen]**-Schaltfläche.

Neue Dokumente werden Ihrem Photoshop-Arbeitsbereich hinzugefügt, wobei die generierten Inhalte auf die Vorlagenfelder angewendet werden. Diese Dokumente werden mit einem nummerierten Variantensuffix benannt.

## Exportieren von Erlebnissen nach GenStudio

Benutzer können nach der Inhaltserstellung oder Übersetzung die Option „Exportieren“ auswählen. Exportierte Erlebnisse werden im Abschnitt Inhalt von GenStudio for Performance Marketing angezeigt.

![Exportierte Assets im Abschnitt Inhalt angezeigt](./content-assets.png){width="90%"}

## Fehlerbehebung

Beachten Sie die folgenden Best Practices und Tipps, wenn Text oder Bilder in generierten Varianten nicht ersetzt werden.

### Zugeordnete Felder

Wenn Text oder Bilder nicht ersetzt werden, bestätigen Sie, dass die Felder korrekt mit geschweiften Klammern `{}` (keine Klammern `()`) zugeordnet sind.

### Bestätigen der Verfügbarkeit von Schriftarten

Die Schriftart eines Textfelds muss auf Ihrem Computer verfügbar sein, damit sie während der Generierung ersetzt wird. Vergewissern Sie sich, dass alle in der Datei verwendeten Schriftarten auf Ihrem Computer verfügbar sind, insbesondere wenn die Datei auf dem Computer eines anderen Benutzers erstellt wurde.

### Ausnahmen bei der Feldzuordnung

{{$include /help/_includes/field-mapping-exceptions.md}}
