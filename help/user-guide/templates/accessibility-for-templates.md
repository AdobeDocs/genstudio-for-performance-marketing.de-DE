---
title: Erstellen barrierefreier Vorlagen
description: Erstellen Sie Vorlagen in Adobe GenStudio for Performance Marketing, die mehr Zielgruppen erreichen und ein optimales Erlebnis bieten.
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# Erstellen barrierefreier Vorlagen

Adobe möchte allen Zielgruppen ein optimales Erlebnis bieten. Siehe [Initiativen zur Barrierefreiheit in Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) für weitere Informationen.

In GenStudio for Performance Marketing können Sie Assets und Vorlagen hochladen, die die Inhaltserstellung für eine Vielzahl von Erlebnissen ermöglichen. Die Einhaltung von Barrierefreiheitsstandards hilft Ihnen, Ihre Inhalte an die gewünschte Zielgruppe anzupassen.

Bereiten Sie Ihre Vorlagen unter Verwendung optimaler Barrierefreiheitsstandards anhand der folgenden Empfehlungen vor.

## Alternativtext

Bieten Sie Textalternativen für nicht-textliche Inhalte wie Bilder.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Collage von Ideen, Bücher, Mann mit Riesenstift, Computer](/help/assets/card-create-assets.png){width="400"}

Verwenden Sie beim Anpassen Ihrer Vorlage Platzhalter für Inhalte für die Attribute `alt` und `aria-label`:

- [Alternativtext](/help/user-guide/templates/customize-template.md#alternative-text)
- [Barrierefreiheits-Kennzeichnung](/help/user-guide/templates/customize-template.md#accessibility-label)

## Schriften

Verwenden Sie leicht lesbare Schriftarten. Zum Beispiel haben Sans Serif-Schriftarten ein sauberes, blockartiges Erscheinungsbild, was zu einer besseren Lesbarkeit beiträgt.

Stellen Sie einen angemessenen Kontrast zwischen Text und Hintergrund bereit. Vermeiden Sie Schriftfarben, die dunklen Text auf einem dunklen Hintergrund und hellen Text auf einem hellen Hintergrund erzeugen. Beachten Sie die Kontrastrichtlinien für ein optimales Verhältnis:

- Text und Bilder von Text: Kontrastverhältnis von mindestens 4,5 :1
- Großer Text und Bilder von großformatigem Text: Kontrastverhältnis von mindestens 3:1

## Link-Zweck (nur Link)

Erstellen Sie einen klaren Link-Text, der den Zweck und die Position des Links beschreibt.

Beispielsweise beschreibt die Verwendung von Link-Text wie „Hier klicken“ oder „Mehr lesen“ nicht klar den Zweck des Links:

```html
<a href="product-site.html">Click here</a>
```

Als Best Practice sollten Sie Text verwenden, der klar beschreibt, wohin der Link führt. Ein besseres Beispiel könnte den Titel der Link-Quelle und den Zweck verwenden:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Sprache

Viele Produkte und Dienstleistungen verwenden Sprache auf kreative oder einzigartige Weise. Vermeiden Sie Jargon, lange Sätze und komplexe Phrasen. Verwenden Sie eine klare, knappe, leicht verständliche Sprache, die mit Ihrer Zielgruppe kompatibel ist.

- Verwenden Sie nach Möglichkeit klare Beschreibungen, Inline-Definitionen oder verknüpfbare Beispiele. Es kann schwierig sein, eine einzigartige Fachsprache zu übersetzen.

- Schreiben Sie die ersten Instanzen eines Akronyms oder einer Abkürzung aus oder verknüpfen Sie sie mit einer Definition. Es kann schwierig sein, Abkürzungen zu übersetzen.

- Verwenden Sie visuelle Elemente, um Text oder komplexe Ideen nach Möglichkeit zu ergänzen.
