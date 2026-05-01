---
title: Einrichten des Logo-Austausches in Vorlagen
description: Konfigurieren Sie die Platzhalter für Markenlogos in Vorlagen, um den Logoaustausch in zu aktivieren [!DNL GenStudio for Performance Marketing].
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# Einrichten des Logoaustauschs in Vorlagen

In diesem Handbuch wird erläutert, wie Sie Platzhalter für Markenlogos in Ihren Vorlagen konfigurieren, um die Funktion [Logo-Tausch](/help/user-guide/create/logo-swap.md) in [!DNL GenStudio for Performance Marketing] zu aktivieren. Verwenden Sie diese Richtlinien, um sicherzustellen, dass der Platzhalter über verschiedene Bildgrößen und Seitenverhältnisse hinweg korrekt angezeigt wird.

## Schnell-Setup

Verwenden Sie den folgenden grundlegenden Vorlagencode für Ihr Logo-Bild:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

Erforderlich:

- `src="{{brand_logo}}"` - Aktiviert die Funktion zum Austausch von Logos.
- `style="{{defaultLogo}}"` - Wendet den Platzhalter-Rahmenstil an.

Optional:

- `class="my-logo"` - Ihre benutzerdefinierte CSS-Klasse für Größenänderung und Stil.

## Grundlegendes zum Platzhalterrahmen

Wenn kein Logo ausgewählt ist, enthält `{{brand_logo}}` ein transparentes 1×1-Pixel-Bild. Der `{{defaultLogo}}` wendet automatisch einen Umriss an, sodass der Platzhalter sichtbar ist:

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

Rahmenverhalten:

- Wird angezeigt, wenn der standardmäßige Platzhalter angezeigt wird.
- verschwindet automatisch nach dem Austauschen eines Logos.
- Skaliert anhand der Größe der übergeordneten Schriftart.

### Rahmendimensionierung

Die `clamp()` passt die Konturstärke an die Vorlagengröße an:

| Größe der übergeordneten Schriftart | Gliederungsgröße |
| --- | --- |
| 10px | 1px (min) |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5 Pixel (max.) |

Formel: `0.1em` entspricht 10 % der übernommenen Schriftgröße und wird zwischen `1px` und `5px` festgehalten.

## Anpassen des Platzhalterrahmens

Sie können den Standardumriss mithilfe von CSS-Klassen überschreiben. Der `{{defaultLogo}}` wendet die Grundlinie an, und die Klasse kann Farbe, Breite und Stil anpassen.

Vorlagen-HTML:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

Vorlagen-CSS:

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>Benutzerdefinierte Gliederungsstile wirken sich nur auf den Platzhalter aus. Sobald ein Logo ausgetauscht wurde, werden alle Gliederungsstile automatisch entfernt.

## Empfohlene Logogröße festlegen

Um sicherzustellen, dass der Platzhalter sichtbar ist und Layout-Verschiebungen verhindert, legen Sie die explizite Größe in Ihrer CSS-Klasse fest:

Vorlagen-HTML:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

Vorlagen-CSS:

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## Positionierung des Kontrolllogos

Verwenden Sie `object-fit` und `object-position`, um zu steuern, wie das Logo in seinem Container skaliert wird.

### Logo zentriert (am häufigsten)

Das Logo kann auf 150,80 × skaliert werden und ist sowohl horizontal als auch vertikal zentriert.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### Logo links ausgerichtet

Logo skaliert, um zu passen, ausgerichtet an der linken Kante, vertikal zentriert.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### Logo oben rechts

Logo skaliert, um zu passen, in der oberen rechten Ecke positioniert.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## Vollständige Beispiele

### Minimale Einrichtung

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>Diese Einrichtung funktioniert, aber der Platzhalter ist möglicherweise fast unsichtbar, da das transparente 1,×-Pixel-Bild auf seine natürliche Größe reduziert wird. Verwenden Sie eine CSS-Klasse mit `width` und `height` für einen sichtbaren Platzhalter.

### Empfohlene Einrichtung

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### Erweitertes Setup mit benutzerdefiniertem Rahmen

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### Flexibles Setup mit Größenbegrenzungen

Verwenden Sie `min-*`- und `max-*` für responsive Vorlagen oder verschiedene Logogrößen.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

Funktionsweise:

- `min-width` und `min-height` halten den Platzhalter sichtbar.
- `max-width` und `max-height` verhindern, dass übergroße Logos das Layout beschädigen.
- Das Logo skaliert proportional innerhalb dieser Grenzen.

## Referenz zu CSS-Eigenschaften

| Kategorie | Eigenschaft | Wert | Zweck |
| --- | --- | --- | --- |
| Erforderlich (HTML) | `src` | `{{brand_logo}}` | Aktiviert die Funktion zum Austauschen von Logos. |
| Erforderlich (HTML) | `style` | `{{defaultLogo}}` | Wendet den Platzhalterumriss an. |
| Empfohlen (CSS-Klasse) | `width` | `120px` | Legt die maximale Logobreite fest. |
| Empfohlen (CSS-Klasse) | `height` | `60px` | Legt die maximale Logohöhe fest. |
| Empfohlen (CSS-Klasse) | `object-fit` | `contain` | Skaliert das Logo ohne Zuschnitt. |
| Empfohlen (CSS-Klasse) | `object-position` | `center center` | Steuert die Ausrichtung des Logos. |
| Optional (CSS-Klasse) | `outline-color` | `#FF0000` | Ändert die Konturfarbe. |
| Optional (CSS-Klasse) | `outline-width` | `3px` | Ändert die Konturstärke. |
| Optional (CSS-Klasse) | `outline-style` | `solid` | Ändert den Gliederungsstil. |
| Flexible Größenanpassung (CSS-Klasse) | `min-width` | `20px` | Stellt die Sichtbarkeit der Platzhalter sicher. |
| Flexible Größenanpassung (CSS-Klasse) | `min-height` | `20px` | Stellt die Sichtbarkeit der Platzhalter sicher. |
| Flexible Größenanpassung (CSS-Klasse) | `max-width` | `200px` | Verhindert Überlauf. |
| Flexible Größenanpassung (CSS-Klasse) | `max-height` | `100px` | Steuert Layout-Grenzen. |

## Best Practices

Führen Sie Folgendes aus:

- Geben Sie immer `{{brand_logo}}` und `{{defaultLogo}}` an.
- Definieren Sie `width` und `height` so, dass der Platzhalter sichtbar ist.
- Verwenden Sie CSS-Klassen für die Größenanpassung und Gliederungsanpassung.
- Verwenden Sie `object-fit: contain`, um die Seitenverhältnisse der Logos beizubehalten.
- Testen Sie mit Logos in verschiedenen Größen und Seitenverhältnissen.

Nicht:

- Verwenden Sie `border` anstelle von `outline` (der Rahmen wird nicht automatisch ausgeblendet).
- Legen Sie Größeneigenschaften in Inline-Stile fest.
- Größenbeschränkungen auslassen (der Platzhalter wird mit 1,1 × dargestellt).
- `object-fit: cover` verwenden (Logos können zugeschnitten werden).

## Fehlerbehebung

Rahmen nicht sichtbar:

- Stellen Sie sicher, dass `style="{{defaultLogo}}"` enthalten ist.
- Vergewissern Sie sich, dass `width` und `height` in Ihrer CSS-Klasse definiert sind.

Platzhalter ist zu klein (1px):

- Fügen Sie Ihrer CSS-Klasse explizite `width` und `height` hinzu.

Rahmen verschwindet nicht nach dem Austausch:

- Verwenden Sie Gliederungseigenschaften in Ihrer CSS-Klasse, nicht `border`.

Logo wird abgeschnitten:

- Verwenden Sie `object-fit: contain` anstelle von `cover`.

Logo zu klein oder zu groß:

- Passen Sie `width` und `height` in Ihrer CSS-Klasse an.

Benutzerdefinierter Rahmen wird nicht angezeigt:

- Bestätigen Sie, `{{defaultLogo}}` sich im `style` befindet.
- Fügen Sie benutzerdefinierte `outline-*` in die CSS-Klasse ein.
