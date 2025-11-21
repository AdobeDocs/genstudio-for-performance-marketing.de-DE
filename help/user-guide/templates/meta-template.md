---
title: Richtlinien für Meta-Anzeigenvorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von Meta-Anzeigenvorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Richtlinien für Meta-Anzeigenvorlagen

Meta-Anzeigenvorlagen helfen Ihnen, visuell konsistente und effektive Anzeigen auf allen Meta-Plattformen zu erstellen. Indem Sie die empfohlenen Design-Verfahren befolgen und unterstützte Felder verwenden, können Sie sicherstellen, dass Ihre Vorlagen für GenStudio for Performance Marketing optimiert sind. In diesem Handbuch wird erläutert, wie Sie Meta-Anzeigenvorlagen für eine nahtlose Integration und wirkungsvolle Ergebnisse strukturieren, anpassen und vorbereiten.

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie Meta-Anzeigenvorlagen für die Arbeit mit GenStudio for Performance Marketing anpassen:

- Spaltenlayouts mit einer Breite von 360 Pixel verwenden
- Verwenden Sie für Bilder eine Mindestauflösung von 1080 x 1080 Pixel
- Es ist genau ein Bildfeld erforderlich
- Verwenden **nicht** relative Schriftgröße
- Viewport **nicht**
- Verwenden **nicht** JavaScript
- Überschreiben **nicht** ein HTML-Element in CSS
- Verwenden Sie das `<img>` Tag anstelle von `background-image`
- Maskieren verwenden, um die Lesbarkeit von Text gegenüber Hintergrundbildern zu verbessern
- Es kann nur ein Abschnitt verwendet werden, wodurch ein einziger Satz von Vorlagenelementen erzeugt wird

## Erkannte Feldnamen

Wenden Sie beim Anpassen Ihrer Meta-Anzeigenvorlage Platzhalter für Inhalte für diese Pflichtfelder an:

- `image` (erforderlich, ausgewählt aus Content JPEG, PNG oder GIF)
- `on_image_text` (Text, der über dem Bild erscheint)

GenStudio for Performance Marketing generiert automatisch die folgenden Felder. Sie müssen keine Platzhalter für Inhalte anwenden für:

- `headline`
- `body`
- `cta`

Weitere Informationen [&#x200B; Verwendung von Feldnamen in Vorlagen finden &#x200B;](/help/user-guide/templates/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## Unterstützte Seitenverhältnisse

| Seitenverhältnis | Abmessungen (Pixel) | Anmerkungen |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Quadrat 1:1 | 1080 x 1080 | Standard für die meisten Meta-Platzierungen; empfohlen für weit reichende Kompatibilität. |
| Hochformat 4:5 | 1080 x 1350 | Optimiert für mobile Feeds; bietet mehr vertikalen Raum. |
| Story 9:16 | 1080 x 1920 | Ideal für Stories und Rollen; füllt den gesamten Bildschirm für Mobilgeräte. |
| Querformat 1.91:1 | 1080 x 566 | Am besten geeignet für Link-Anzeigen und Platzierungen von Nachrichten-Feeds; Breitformat. |
| Benutzerdefiniert | Mindestens 50 x 50 (Breite) | Nur verwenden, wenn erforderlich; kann zu Zuschnitt oder Skalierung führen. |

Wenn die Anzeige nicht in einem dieser Seitenverhältnisse entworfen wurde, schneidet GenStudio for Performance Marketing das Bild automatisch in die entsprechende Größe zu.

## Vorlagenbeispiel

+++Beispiel: Meta-Anzeigenvorlage

<!-- Does this need to be a precise size? -->

Im Folgenden finden Sie ein einfaches Beispiel für eine Meta-Anzeigenvorlage. Der Kopf enthält Inline-CSS für die Formatierung. Der Textkörper verwendet [Platzhalter für Inhalte](#content-placeholders) wie `image` und `on_image_text`, um anzugeben, wo GenStudio for Performance Marketing Inhalte generieren kann.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
