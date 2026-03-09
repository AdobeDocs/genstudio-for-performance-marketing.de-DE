---
title: Richtlinien für LinkedIn-Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von LinkedIn-Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
TQID: https://experienceleague.adobe.com/YyG3WuMkdVAaACX03qLKzzw-fFA3WfT9K2ohjnQNPcI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 2%

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

Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](/help/user-guide/templates/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## Unterstützte Seitenverhältnisse

Alle LinkedIn-Vorlagenbreiten sind mit 1200 Pixel hartcodiert.

| Seitenverhältnis | Platform | Abmessungen (px) | Anmerkungen |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| Quadrat 1:1 | Desktop, Mobilgerät | 1200 x 1200 | Am vielseitigsten. Ideal für ein konsistentes Erscheinungsbild über Geräte und Platzierungen hinweg. |
| Horizontal 1,91:1 | Desktop | 1200 x 628 | Standard-Querformat. Wird häufig für gesponserte Inhalte und Nachrichten-Feed-Anzeigen verwendet. |
| Vertikal 1:1,91 | Mobile | 1200 x 2292 | Hohes vertikales Format Optimiert für mobile Anzeige, mehr Bildschirmpräsenz. |
| Vertikal 2:3 | Mobile | 1200 x 1800 | Etwas kleiner als 1:1,91. Gut für Mobile-First-Kampagnen. |
| Vertikal 4:5 | Mobile | 1200 x 1500 | Empfohlen für Mobilgeräte. Gleicht Sichtbarkeit und Inhalte aus, was oft eine höhere Wirkung erzielt. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
