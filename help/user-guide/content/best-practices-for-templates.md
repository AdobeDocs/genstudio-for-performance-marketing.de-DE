---
title: Best Practices für Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von Vorlagen mit Adobe GenStudio for Performance Marketing.
feature: Templates, Content
last-substantial-update: 2024-12-13T00:00:00Z
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 9cc284cdb00a204baf6b0a2d9d7f67cf9bc9c81f
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Best Practices für die Verwendung von Vorlagen

Vorlagen reduzieren den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellen, der vorkonfigurierte Layouts und Designelemente enthält.

Verwenden Sie bei der Verwendung von Vorlagen mit GenStudio for Performance Marketing die folgenden Empfehlungen:

1. Know about [template elements](#know-about-template-elements)
1. Konfigurieren [Kanalrichtlinien](#configure-channel-guidelines) für die effektive Personalisierung von Inhalten
1. Design mit [Barrierefreiheitsstandards](accessibility-for-templates.md) für ein optimales Erlebnis
1. Befolgen [kanalspezifischen Vorlagenrichtlinien](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Weitere Informationen über grundlegende Vorlagenelemente und Verfahren finden Sie unter [Arbeiten mit Vorlagen](use-templates.md). und detaillierte Einblicke in [Anpassen einer Vorlage](customize-template.md) zur Verwendung in Ihrer nächsten Kampagne.

## Know about template elements

Es empfiehlt sich, sich mit den Teilen einer Vorlage vertraut zu machen. Jeder Vorlagentyp verwendet verschiedene Elemente, um eine Struktur für die kanalspezifische Inhaltserstellung zu erstellen. Um Ihre Vorlage anzupassen, verwenden Sie die Feldnamen anstelle dieser Elemente, für die GenStudio for Performance Marketing Inhalte generieren muss.

Siehe [Vorlagenelemente](use-templates.md#template-elements).

## Konfigurieren von Kanalrichtlinien

Konfigurieren Sie die Kanalrichtlinien für jede Marke, bevor Sie Vorlagen in GenStudio for Performance Marketing verwenden. Die Kanalrichtlinien beeinflussen direkt den Inhaltstyp, der bei Verwendung der Vorlage generiert wird. Sie können beispielsweise Zeichenbeschränkungen für den Textkörper einer E-Mail festlegen.

![Technische Daten des Textkörpers](/help/assets/channel-email-body.png)

Siehe [Kanalrichtlinien](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Befolgen der Richtlinien für kanalspezifische Vorlagen

Erstellen Sie Vorlagen, die das Layout und die visuellen Anforderungen für jeden Kanal berücksichtigen. Beachten Sie bei der Arbeit mit jedem Vorlagentyp die folgenden Tipps und Einschränkungen, um eine optimale Leistung und Kompatibilität zu gewährleisten:

>[!BEGINTABS]

>[!TAB E-Mail]

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie E-Mail-Vorlagen für die Arbeit mit GenStudio for Performance Marketing anpassen:

- Adobe- oder Google-Schriftarten verwenden
- Verwenden von sauberem und responsivem HTML und Inline-CSS
- Verwenden **nicht** JavaScript
- Verwenden **nicht** eine feste Breite im Textkörper oder Container
- Verwenden **nicht** die Base64-Kodierung für Bilder, da dadurch die Vorlagengröße erheblich erhöht werden kann

**Einschränkungen**:

- Verwendung von [Abschnitten](customize-template.md#sections-or-groups):
   - Eine einfache Vorlage (nur ein Abschnitt) kann einen einzigen Satz von Vorlagenelementen generieren.
   - Eine komplexe Vorlage (mehrere Abschnitte) kann bis zu drei Sätze von Vorlagenelementen generieren.
- In einer Vorlage sind maximal 20 Felder zulässig
- Die maximale Größe der HTML-Datei beträgt 102 KB

**Erkannte Feldnamen**:

Für E-Mails wird das `subject` automatisch eingefügt. Verwenden Sie Platzhalter für Inhalte für die folgenden Felder:

- `pre_header`
- `headline`
- `body`
- `cta`
- `image` (aus Inhalt ausgewählt)
- `brand_logo`

Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

>[!TAB Meta-Anzeige]

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie Meta-Anzeigenvorlagen für die Arbeit mit GenStudio for Performance Marketing anpassen:

- Spaltenlayouts mit einer Breite von 360 Pixel verwenden
- Verwenden Sie für Bilder eine Mindestauflösung von 1080 x 1080 Pixel
- Verwenden **nicht** relative Schriftgröße
- Viewports **nicht**
- Verwenden **nicht** JavaScript
- HTML **Element** im CSS nicht überschreiben
- Verwenden Sie die folgenden Einstellungen für Hintergrundbilder:

  Fügen Sie `object-fit: cover` Wert `background-image` CSS-Klasse hinzu:

  ```css
  .background-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  ```

**Einschränkungen**:

- Verwendung von [Abschnitten](customize-template.md#sections-or-groups):
   - Es kann nur ein Abschnitt verwendet werden, wodurch ein einziger Satz von Vorlagenelementen erzeugt wird.

**Unterstützte Seitenverhältnisse**:

- Quadrat 1:1 (1080 x 1080 Pixel)
- Vertikal 4:5 (1080 x 1350 Pixel)
- Story 9:16 (1080 x 1920 Pixel)
- Benutzerdefinierte Bildgröße: (Mindestbildbreite von 50 x 50 Pixeln)

**Erkannte Feldnamen**:

Bei Meta-Anzeigen werden die Felder `headline`, `body` und `CTA` automatisch generiert. Verwenden Sie Platzhalter für Inhalte für die folgenden Felder:

- `image` (aus Inhalt ausgewählt)
- `on-image-text`
- `brand_logo`

Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

>[!TAB Anzeige anzeigen]

[!BADGE Beta]{type=Informative tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."}

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie Display-Anzeigenvorlagen für die Arbeit mit GenStudio for Performance Marketing anpassen:

- Adobe- oder Google-Schriftarten verwenden
- Vorbereiten von Assets, die in schlanken Dimensionen gut angezeigt werden
- Verwenden **nicht** eingebettete oder kodierte Hintergrundbilder
- Verwenden von Hintergrundbildern (`image`), die in das GenStudio for Performance Marketing Content Repository hochgeladen wurden
- Verwenden **nicht** JavaScript

**Einschränkungen**:

- Verwendung von [Abschnitten](customize-template.md#sections-or-groups):
   - Es kann nur ein Abschnitt verwendet werden, wodurch ein einziger Satz von Vorlagenelementen erzeugt wird.

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
- Benutzerdefiniert: (Pixel)
   - 50 x 50 bis 2000 x 2000

**Erkannte Feldnamen**:

Verwenden Sie Platzhalter für Inhalte für die folgenden Felder:

- `headline`
- `body`
- `cta`
- `image` (aus Inhalt ausgewählt)

Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

>[!ENDTABS]
