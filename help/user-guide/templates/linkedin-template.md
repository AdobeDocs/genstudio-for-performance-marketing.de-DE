---
title: Richtlinien für LinkedIn-Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von LinkedIn-Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 3%

---

# Richtlinien für LinkedIn-Vorlagen

LinkedIn-Vorlagen bieten eine strukturierte Möglichkeit zum Erstellen und Anpassen von Werbekampagnen für LinkedIn-Kampagnen. Diese Richtlinien stellen sicher, dass Ihre Anzeigen den Spezifikationen von LinkedIn entsprechen, während der Kreativprozess in GenStudio for Performance Marketing optimiert wird. Dieser Leitfaden hilft Ihnen bei der Vorbereitung auf ein konsistentes Branding und eine effektive Leistung auf den Desktop- und Mobilplattformen von LinkedIn.

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie LinkedIn-Anzeigenvorlagen für die Arbeit mit GenStudio for Performance Marketing anpassen:

- Es ist genau ein Bildfeld erforderlich
- Maximale Bildgröße von 5 MB
- Maximale Überschrift 70 Zeichen
- Maximaler Einführungstext 150 Zeichen
- Es kann nur ein Abschnitt verwendet werden, wodurch ein einziger Satz von Vorlagenelementen erzeugt wird

## Erkannte Feldnamen

Wenden Sie beim Anpassen Ihrer LinkedIn-Vorlage Platzhalter für Inhalte für diese Pflichtfelder an:

- `image` (erforderlich, ausgewählt aus Content JPEG, PNG oder GIF)
- `on_image_text` (Text, der über dem Bild erscheint)

GenStudio for Performance Marketing generiert automatisch die folgenden Felder. Sie müssen keine Platzhalter für Inhalte anwenden für:

- `headline`
- `introductory_text`
- `cta` (Call to action)

Weitere Informationen [&#x200B; Verwendung von Feldnamen in Vorlagen finden &#x200B;](/help/user-guide/content/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## Unterstützte Seitenverhältnisse

| Seitenverhältnis | Platform | Mindestgröße (px) | Max. Größe (px) | Anmerkungen |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| Quadrat 1:1 | Desktop, Mobilgerät | 360 x 360 | 4320 x 4320 | Am vielseitigsten. Ideal für ein konsistentes Erscheinungsbild über Geräte und Platzierungen hinweg. |
| Horizontal 1,91:1 | Desktop | 640 x 360 | 7680 x 4320 | Standard-Querformat. Wird häufig für gesponserte Inhalte und Nachrichten-Feed-Anzeigen verwendet. |
| Vertikal 1:1,91 | Mobile | 360 x 640 | 2430 x 4320 | Hohes vertikales Format Optimiert für mobile Anzeige, mehr Bildschirmpräsenz. |
| Vertikal 2:3 | Mobile | 360 x 640 | 2430 x 4320 | Etwas kleiner als 1:1,91. Gut für Mobile-First-Kampagnen. |
| Vertikal 4:5 | Mobile | 360 x 640 | 2430 x 4320 | Empfohlen für Mobilgeräte. Gleicht Sichtbarkeit und Inhalte aus, was oft eine höhere Wirkung erzielt. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
