---
title: Anzeigenvorlagen-Richtlinien anzeigen
description: Befolgen Sie die Best Practices bei der Verwendung von Anzeigen- und Bannervorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
TQID: https://experienceleague.adobe.com/HjkLWiyqK1quHoZB5lEE-qyB3zci12KlRAZC8ME-9Ao
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 1%

---

# Anzeigenvorlagen-Richtlinien anzeigen

Anzeigevorlagen sind vorkonfigurierte Layouts, mit denen visuell ansprechende Banner- und Display-Anzeigen erstellt werden. Sie bieten ein flexibles Framework für die Integration von Bildern, Text und call to action und stellen so Konsistenz und Effizienz bei der Produktion mehrerer Anzeigenvarianten sicher. Wenn Sie Ihre Vorlage für die Verwendung in GenStudio for Performance Marketing vorbereiten, stellen Sie sicher, dass alle Assets für die Web-Anzeige optimiert sind und die erforderlichen Dateiformate und -größen erfüllen.

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie die Anzeigenvorlagen für Banner und Anzeigen an GenStudio for Performance Marketing anpassen:

- Verwenden von Adobe- oder Google-Schriftarten
- Vorbereiten von Assets, die in schlanken Dimensionen gut angezeigt werden
- Es ist genau ein Bildfeld erforderlich
- Verwenden **nicht** eingebettete oder kodierte Hintergrundbilder
- Verwenden Sie Hintergrundbilder (`image` Feld), die in das GenStudio for Performance Marketing-Inhalts-Repository hochgeladen wurden. Die besten Ergebnisse erzielen Sie, wenn Sie die Richtlinien unter [Hochladen von Bildern ](#uploading-images-for-display-ads) Display-Anzeigen“ befolgen
- Verwenden **nicht** JavaScript
- Es kann nur ein Abschnitt verwendet werden, wodurch ein einziger Satz von Vorlagenelementen erzeugt wird

## Erkannte Feldnamen

Verwenden Sie beim Anpassen Ihres Banners oder Ihrer Anzeigenvorlage Platzhalter für Inhalte für die folgenden erforderlichen Felder:

- `headline`
- `sub_headline`
- `body`
- `image` (erforderlich, ausgewählt aus Content JPEG, PNG oder GIF)

GenStudio for Performance Marketing generiert automatisch die folgenden Felder. Sie müssen keine Platzhalter für Inhalte anwenden für:

- `cta`

Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](/help/user-guide/templates/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## Unterstützte Dimensionen

Breite x Höhe (Pixel) müssen festgelegt werden.

| Ausrichtung | Abmessungen (Pixel) | Anmerkungen |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertikal | 300 x 600<br>160 x 600 | Häufig für Wolkenkratzer und Banner mit halben Seiten. |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standardmäßige Leaderboard-, mittlere Rechteck- und Bannergrößen. |
| Benutzerdefiniert | 50 x 50 bis 2000 x 2000 | Für nicht standardmäßige oder eindeutige Platzierungen verwenden; Plattformbeschränkungen überprüfen. |

