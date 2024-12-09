---
title: Best Practices für Vorlagen
description: Befolgen Sie bei der Verwendung von Vorlagen mit Adobe GenStudio for Performance Marketing die Best Practices.
feature: Templates, Content
last-substantial-update: 2024-12-09T00:00:00Z
source-git-commit: 7ba2ecfbdd6853934be5210685bf447848715d28
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Best Practices für die Verwendung von Vorlagen

Vorlagen reduzieren die Zeit und den Aufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt mit vorkonfigurierten Layouts und Designelementen bereitstellen.

Verwenden Sie die folgenden Empfehlungen bei der Verwendung von Vorlagen mit GenStudio for Performance Marketing:

1. Wissenswertes über [Vorlagenelemente](#know-about-template-elements)
1. Konfigurieren von [Kanalrichtlinien](#configure-channel-guidelines) für eine effektive Personalisierung von Inhalten
1. Design mit [Barrierefreiheitsstandards](accessibility-for-templates.md) für ein optimales Erlebnis
1. Befolgen Sie die [kanalspezifischen Vorlagenrichtlinien](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Erfahren Sie mehr über grundlegende Vorlagenelemente und -verfahren in [Arbeiten mit Vorlagen](use-templates.md). Machen Sie sich mit [der Anpassung einer Vorlage](customize-template.md) für die Verwendung in Ihrer nächsten Kampagne vertraut.

## Informationen zu Vorlagenelementen

Als Best Practice sollten Sie sich mit den Teilen einer Vorlage vertraut machen. Jeder Vorlagentyp verwendet unterschiedliche Elemente, um eine Struktur für die kanalspezifische Inhaltserstellung zu erstellen. Verwenden Sie zum Anpassen Ihrer Vorlage die Feldnamen anstelle dieser Elemente, für die GenStudio for Performance Marketing Inhalte generieren muss.

Siehe [Vorlagenelemente](use-templates.md#template-elements).

## Konfigurieren von Kanalrichtlinien

Konfigurieren Sie die Kanalrichtlinien für jede Marke, bevor Sie Vorlagen in GenStudio for Performance Marketing verwenden. Die Kanalrichtlinien beeinflussen direkt den Inhaltstyp, der bei Verwendung der Vorlage generiert wird. Sie können beispielsweise Zeichenbeschränkungen für den Text einer E-Mail festlegen.

![Textkörperspezifikationen](/help/assets/channel-email-body.png)

Siehe [Kanalrichtlinien](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Befolgen Sie die kanalspezifischen Vorlagenrichtlinien

Erstellen Sie Vorlagen, die die Layout- und visuellen Anforderungen der einzelnen Kanäle berücksichtigen. Beachten Sie beim Arbeiten mit jedem Vorlagentyp die folgenden Tipps und Einschränkungen, um eine optimale Leistung und Kompatibilität sicherzustellen:

>[!BEGINTABS]

>[!TAB E-Mail]

Befolgen Sie diese Best Practices beim Design, wenn Sie E-Mail-Vorlagen für die Verwendung mit GenStudio for Performance Marketing anpassen:

- Verwenden von Adobe- oder Google-Schriftarten
- Verwenden von sauberem und responsivem HTML und Inline-CSS
- Verwenden Sie **nicht** JavaScript
- Verwenden Sie **nicht** eine feste Breite im Körper oder Container
- Verwenden Sie die base64-Kodierung für Bilder **nicht**, da dadurch die Vorlagengröße erheblich erhöht werden kann.

**Einschränkungen**:

- Verwendung von [Abschnitten](customize-template.md#sections-or-groups):
   - Eine einfache Vorlage (nur ein Abschnitt) kann einen einzigen Satz von Vorlagenelementen generieren.
   - Eine komplexe Vorlage (mehrere Abschnitte) kann bis zu drei Sätze von Vorlagenelementen generieren.
- In einer Vorlage sind maximal 20 Felder zulässig
- Die maximale HTML-Dateigröße beträgt 102 KB.

**Erkannte Feldnamen**:

Für E-Mails wird das Feld `subject` automatisch eingefügt. Verwenden Sie Platzhalter für die folgenden Felder:

- `pre_header`
- `headline`
- `body`
- `cta`
- `image` (aus Inhalt ausgewählt)
- `brand_logo`

Weitere Informationen zur Verwendung von Feldnamen in Vorlagen finden Sie unter [Platzhalter für Inhalte](customize-template.md#content-placeholders) .

>[!TAB Metaanzeige]

Befolgen Sie diese Best Practices beim Design, wenn Sie Meta-Anzeigenvorlagen für die Verwendung mit GenStudio for Performance Marketing anpassen:

- Verwenden Sie 360 Pixel Breite für Spaltenlayouts
- Mindestens 1080 x 1080 Pixel für Bilder verwenden
- Verwenden Sie **nicht** die relative Schriftgröße
- Definieren Sie Viewports durch **nicht**
- Verwenden Sie **nicht** JavaScript
- Überschreiben Sie **nicht** ein HTML-Element im CSS.
- Verwenden Sie die folgenden Einstellungen für Hintergrundbilder:

  Fügen Sie `object-fit: cover` -Wert zur CSS-Klasse `background-image` hinzu:

  ```css
  .background-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  ```

**Einschränkungen**:

- Verwendung von [Abschnitten](customize-template.md#sections-or-groups):
   - Es kann nur ein Abschnitt verwendet werden, der einen einzigen Satz von Vorlagenelementen generiert.

**Unterstützte Seitenverhältnisse**:

- Quadrat 1:1 (1080 x 1080 Pixel)
- Vertikal 4:5 (1080 x 1350 Pixel)
- Story 9:16 (1080 x 1920 Pixel)

**Erkannte Feldnamen**:

Bei Metaanzeigen werden die Felder `headline`, `body` und `CTA` automatisch generiert. Verwenden Sie Platzhalter für die folgenden Felder:

- `image` (aus Inhalt ausgewählt)
- `on-image-text`
- `brand_logo`

Weitere Informationen zur Verwendung von Feldnamen in Vorlagen finden Sie unter [Platzhalter für Inhalte](customize-template.md#content-placeholders) .

>[!TAB Display ad]

Befolgen Sie diese Best Practices für das Design beim Anpassen von Display-Anzeigenvorlagen für die Verwendung mit GenStudio for Performance Marketing:

- Verwenden von Adobe- oder Google-Schriftarten
- Vorbereiten von Assets, die in schlanken Dimensionen gut angezeigt werden
- Verwenden Sie **nicht** eingebettete oder kodierte Hintergrundbilder
- Hintergrundbilder verwenden (`image` -Feld), die in das GenStudio for Performance Marketing-Inhalts-Repository hochgeladen wurden
- Verwenden Sie **nicht** JavaScript

**Einschränkungen**:

- Verwendung von [Abschnitten](customize-template.md#sections-or-groups):
   - Es kann nur ein Abschnitt verwendet werden, der einen einzigen Satz von Vorlagenelementen generiert.

**Unterstützte Dimensionen**:

- Vertikal: (Pixel)
   - 300 x 600
   - 160 x 600 &#x200B;
- Horizontal: (Pixel)
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250 &#x200B;

**Erkannte Feldnamen**:

Verwenden Sie Platzhalter für die folgenden Felder:

- `headline`
- `body`
- `cta`
- `image` (aus Inhalt ausgewählt)

Weitere Informationen zur Verwendung von Feldnamen in Vorlagen finden Sie unter [Platzhalter für Inhalte](customize-template.md#content-placeholders) .

>[!ENDTABS]
