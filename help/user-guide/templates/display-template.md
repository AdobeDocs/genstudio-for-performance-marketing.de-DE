---
title: Anzeigenvorlagen-Richtlinien anzeigen
description: Befolgen Sie die Best Practices bei der Verwendung von Anzeigen- und Bannervorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
source-git-commit: 78313c2a2177a2ccb39e37a87ca3c657e7906d0a
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 1%

---

# Anzeigenvorlagen-Richtlinien anzeigen

Anzeigevorlagen sind vorkonfigurierte Layouts, mit denen visuell ansprechende Banner- und Display-Anzeigen erstellt werden. Sie bieten ein flexibles Framework für die Integration von Bildern, Text und call to action und stellen so Konsistenz und Effizienz bei der Produktion mehrerer Anzeigenvarianten sicher. Wenn Sie Ihre Vorlage für die Verwendung in GenStudio for Performance Marketing vorbereiten, stellen Sie sicher, dass alle Assets für die Web-Anzeige optimiert sind und die erforderlichen Dateiformate und -größen erfüllen.

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie die Anzeigenvorlagen für Banner und Anzeigen an GenStudio for Performance Marketing anpassen:

- Verwenden von Adobe- oder Google-Schriftarten
- Vorbereiten von Assets, die in schlanken Dimensionen gut angezeigt werden
- Es ist genau ein Bildfeld erforderlich
- Verwenden **nicht** eingebettete oder kodierte Hintergrundbilder
- Verwenden von Hintergrundbildern (`image`), die in das GenStudio for Performance Marketing Content Repository hochgeladen wurden
- Verwenden **nicht** JavaScript
- Es kann nur ein Abschnitt verwendet werden, wodurch ein einziger Satz von Vorlagenelementen erzeugt wird

## Erkannte Feldnamen

Für Banner- und Display-Anzeigen generiert GenStudio for Performance Marketing automatisch das `cta`. Verwenden Sie beim Anpassen Ihrer Vorlage Platzhalter für Inhalte für die folgenden erforderlichen Felder:

- `headline`
- `sub_headline`
- `body`
- `image` (erforderlich, ausgewählt aus Content JPEG, PNG oder GIF)

Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](/help/user-guide/content/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## Unterstützte Dimensionen

Breite x Höhe (Pixel) müssen festgelegt werden.

| Ausrichtung | Abmessungen (Pixel) | Anmerkungen |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertikal | 300 x 600<br>160 x 600 | Häufig für Wolkenkratzer und Banner mit halben Seiten |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standardmäßige Leaderboard-, mittlere Rechteck- und Bannergrößen |
| Benutzerdefiniert | 50 x 50 bis 2000 x 2000 | Für nicht standardmäßige oder eindeutige Platzierungen verwenden; Plattformbeschränkungen überprüfen |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
