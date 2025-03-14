---
title: Anpassen einer Vorlage
description: Erfahren Sie, wie Sie Ihre Vorlage für Adobe GenStudio for Performance Marketing personalisieren und optimieren können.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: eb7f19ebc0854db3a33599b56c857875ee67982b
workflow-type: tm+mt
source-wordcount: '1442'
ht-degree: 0%

---

# Anpassen einer Vorlage

Sie können eine Vorlage für die Verwendung in GenStudio for Performance Marketing anpassen, indem Sie Platzhalter oder Felder für Inhalte einfügen, die die generative KI zum Einfügen von Inhalten verwendet.

In den nächsten Abschnitten wird erläutert, wie Sie Ihre HTML-Vorlagen für GenStudio for Performance Marketing mithilfe der _[!DNL Handlebars]_anpassen. Die [!DNL Handlebars] Syntax verwendet regulären Text mit doppelten Klammern als Platzhalter für Inhalte. Unter [Was ist [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) im_ Handlebars-Sprachhandbuch _erfahren Sie, wie Sie Ihre Vorlage vorbereiten.

Sobald Ihre Vorlage fertig ist, können Sie sie [in GenStudio for Performance Marketing hochladen](use-templates.md#upload-a-template) und mit der Erstellung personalisierter E-Mails beginnen, die auf Ihrer benutzerdefinierten Vorlage basieren.

>[!TIP]
>
>Befolgen Sie [Richtlinien für ](accessibility-for-templates.md) Barrierefreiheit[ und „Best ](/help/user-guide/content/best-practices-for-templates.md)&quot;, damit Sie mehr Ihrer Audience erreichen und ein optimales Erlebnis bieten können.

## Platzhalter für Inhalte

GenStudio for Performance Marketing erkennt bestimmte [Elemente](use-templates.md#template-elements) innerhalb einer Vorlage, jedoch nur, wenn Sie sie mit einem [erkannten Feldnamen](#recognized-field-names) identifizieren.

Im Kopf oder Text einer HTML-Vorlage können Sie die [!DNL Handlebars] verwenden, um einen Platzhalter für Inhalte einzufügen, bei dem GenStudio for Performance Marketing die Vorlage mit tatsächlichem Inhalt füllen muss. GenStudio for Performance Marketing erkennt und interpretiert die Platzhalter für Inhalte anhand des [erkannten _Feld_ Namens](#recognized-field-names).

Sie können beispielsweise `{{ headline }}` mit der [!DNL Handlebars] Syntax verwenden, um anzugeben, wo die Überschrift der E-Mail platziert werden soll. GenStudio erkennt dieses Feld, generiert eine entsprechende Überschrift auf der Grundlage Ihrer Richtlinien und Eingabeaufforderungskriterien und fügt die Überschrift an dieser Stelle ein:

```handlebars
<div>{{ headline }}</div>
```

### Erkannte Feldnamen

In der folgenden Tabelle sind die Feldnamen aufgeführt, die von GenStudio for Performance Marketing zum Hinzufügen eines Platzhalters zu einer Vorlage erkannt werden. Fügen Sie diese Feldnamen mithilfe der [!DNL Handlebars]-Syntax zu Ihrer Vorlage hinzu, wenn GenStudio for Performance Marketing einen bestimmten Inhaltstyp generieren soll.

| Feld | Rolle | Kanalvorlage |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Preheader | E-Mail |
| `{{headline}}` | Überschrift | E<br>Mail-Anzeige <br>Banner und Display-Anzeige <br>LinkedIn-Anzeige |
| `{{introductory_text}}` | Einführungstext | LinkedIn-Anzeige |
| `{{body}}` | Textkörper | E<br>Mail-Anzeige <br>Banner und Display-Anzeige |
| `{{cta}}` | Handlungsaufforderung | E<br>Mail-Anzeige <br>Banner und Display-Anzeige <br>LinkedIn-Anzeige |
| `{{image}}` | Bild (Image) - Auswahl aus [!DNL Content] | E<br>Mail-Anzeige <br>Banner und Display-Anzeige <br>LinkedIn-Anzeige |
| `{{on_image_text}}` | Bei Bildtext | Meta-Anzeige <br>LinkedIn-Anzeige |
| `{{link}}` | Aktionsaufruf für Bild<br> Siehe [Link auf Bild](#link-on-image). | E-Mail |
| `{{brand_logo}}` | Logo der ausgewählten Marke<br> Siehe [Feldname für das Markenlogo](#brand-logo-field-name). | email<br>Meta-Anzeige <br>LinkedIn-Anzeige |

GenStudio for Performance Marketing füllt bestimmte Felder in den folgenden Vorlagen automatisch:

- **E-Mail** Vorlage: Erfordert nicht, dass das `subject` Feld identifiziert wird
- **Meta-Anzeigenvorlage** erfordert nicht, dass Sie die Felder `headline`, `body` und `CTA` identifizieren
- **Banner- und Display-Anzeigenvorlage** erfordert keine Identifizierung des `CTA` Felds
- **LinkedIn** Anzeigenvorlagen erfordern nicht, dass Sie die Felder `headline`, `introductory_text` und `CTA` identifizieren

>[!WARNING]
>
>Bei Instagram-Anzeigen wird die generierte Überschrift nicht im endgültigen Erlebnis angezeigt.

Beim Hochladen einer Vorlage in GenStudio for Performance Marketing gibt es eine Beschränkung von 20 Feldern. Da das `subject` automatisch in einer E-Mail generiert wird, zählt es als ein Feld. Das bedeutet, dass in einer E-Mail-Vorlage 19 Felder zulässig sind.

>[!TIP]
>
>Sie können Ihre Vorlage mithilfe der [Vorlagenvorschau](#template-preview) in GenStudio for Performance Marketing überprüfen.

### Handlungsaufforderungen

Ein Aktionsaufruf (CTA) enthält einen Satz und einen Link. Damit die CTA-Funktionen _[!UICONTROL Umformulieren]_ und _[!UICONTROL Link hinzufügen]_ während des Variantengenerierungsprozesses ordnungsgemäß funktionieren, müssen Sie Platzhalter für den Link und den Satz in Ihrer Vorlage einfügen.

Verwenden Sie die folgende Anleitung zum Einrichten von CTA-Platzhaltern:

- CTA-Umformulierung ist verfügbar und Link kann bearbeitet werden

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTA-Umformulierung ist verfügbar, aber Link **nicht** bearbeitbar, da der eigentliche Link in der Vorlage bereitgestellt wird

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- CTA-Link ist bearbeitbar, aber Umformulierung ist **nicht** verfügbar, da die Phrase in der Vorlage bereitgestellt wird

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing kann auch Ausdrücke mit varianten Aktionsaufrufen bereitstellen. Siehe [Revidieren einer Handlungsaufforderung](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Verknüpfung auf Bild

Sie können Ihre E-Mail-Vorlage anpassen, damit Kreative einem Bild einen Link hinzufügen können. Ähnlich wie beim CTA-Link können Sie mithilfe der folgenden Anleitung einen `link` Platzhalter auf ein Bild-Tag anwenden:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="description"></a>
```

Beschreibung dieses Beispiels:

- `{{link}}` ist ein Platzhalter für die tatsächliche URL.
- `src="image-source.jpg"` sollte durch die tatsächliche Bildquellen-URL ersetzt werden.
- `alt="description"` bietet einen Alternativtext für das Bild, der für Barrierefreiheit und SEO nützlich ist.

### Feldname für das Markenlogo

Derzeit können Sie das Markenlogo für den Vorlagen-Upload nicht auswählen. Die folgenden Beispiele zeigen zwei Methoden, die das Markenlogo bedingt rendern. Jede Methode überprüft die Quelle, liefert ein Standard- oder Alternativbild für den Fall, dass das Markenlogo nicht verfügbar ist, und wendet einen Stil an:

**Beispiel 1**: Verwenden [!DNL Handlebars] integrierten Helper-Bedingung direkt im HTML-`img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Beispiel 2**: Verwenden [!DNL Handlebars] integrierten Bedingungsanweisung, um das HTML-`img`-Tag einzuschließen:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

### Manuelle Feldnamen

Alle anderen Feldnamen werden als manuell ausgefüllte Felder behandelt. Beispielsweise können Sie einen Abschnitt für den Inhalt der Fußzeile reservieren.

Um einen bearbeitbaren Abschnitt zu erstellen, fügen Sie doppelte Klammern um den Abschnittsnamen hinzu:

```html
<tbody>
    <tr>
        <td>
            <p><span class="s1">{{ footerLegal }}</span></p>
        </td>
    </tr>
</tbody>
```

## Abschnitte oder Gruppen

_Abschnitte_ informieren GenStudio for Performance Marketing, dass die Felder in diesem Abschnitt ein hohes Maß an Kohärenz erfordern. Durch Festlegen dieser Beziehung kann die KI Inhalte generieren, die den kreativen Elementen im Abschnitt entsprechen.

Verwenden Sie ein Präfix Ihrer Wahl im Feldnamen, um anzugeben, dass ein Feld Teil eines Abschnitts oder einer Gruppe ist. Verwenden Sie einen Feldnamen (`headline`, `body`, `image` oder `cta`) nach dem Unterstrich (`_`). Beispielsweise gehören die folgende Überschrift und der folgende Hauptteil zum Abschnitt `pod1`:

- `pod1_headline`
- `pod1_body`

Jeder Abschnitt kann nur einen der Feldtypen verwenden. Im obigen Beispiel kann der Abschnitt `pod1` nur ein `pod1_headline` verwenden. Aufgrund dieser Regel können die Abschnitte nicht verschachtelt werden.

Jeder Vorlagentyp, z. B. E-Mail- oder Meta-Anzeige, unterliegt kanalspezifischen Einschränkungen für die Verwendung von Abschnitten. Siehe [Kanalspezifische Richtlinien](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) im Thema _Best Practices für die Verwendung von Vorlagen_.

Eine E-Mail-Vorlage kann beispielsweise bis zu drei Abschnitte enthalten. Daher können Sie drei Überschriften- und Hauptteilabschnitte haben:

- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing weiß, dass `pod1_headline` enger mit `pod1_body` als mit `pod2_body` verbunden ist.

Unter [Strukturierte Eingabeaufforderungen](/help/user-guide/effective-prompts.md#structured-prompts) erfahren Sie, wie Sie eine Eingabeaufforderung erstellen, die für jeden Abschnitt in einer E-Mail mit mehreren Abschnitten unterschiedliche Inhalte generiert.


## Vorlagenvorschau

Wenn Sie [eine Vorlage hochladen](use-templates.md#upload-a-template) durchsucht GenStudio for Performance Marketing die HTML-Datei nach erkannten Feldern. Verwenden Sie die Vorschau, um Ihre [Vorlagenelemente](use-templates.md#template-elements) zu überprüfen und sicherzustellen, dass Sie sie ordnungsgemäß mit den [erkannten Feldnamen“ ](#recognized-field-names).

Beispielvorschau für eine E-Mail-Vorlage:

![Erkannte Vorschaufelder](/help/assets/template-detected-fields.png "Erkannte Felder überprüfen"){zoomable="yes"}

Siehe [Vorlagen-Code-Editor](/help/user-guide/content/code-editor.md).

### Vorschau steuern

Sie können die Sichtbarkeit spezieller Inhalte mithilfe integrierter Helper (spezielle Ausdrücke in der [!DNL Handlebars]-Vorlagensprache, die bestimmte Aktionen ausführen) steuern. Sie können beispielsweise eine bedingte Anweisung hinzufügen, die Tracking-Parameter zu Links in der exportierten Vorlage hinzufügt, während die Vorschau-Links sauber bleiben.

Der `_genStudio.browser` wird beim Rendern einer Vorlage festgelegt und der `genStudio.export` wird beim Exportieren einer Vorlage festgelegt. Sie können sich dafür entscheiden, bestimmte Inhalte am Anfang einer E-Mail mit einem bedingten Wrapper einzuschließen, z. B. wenn die Vorlage für den Export verwendet wird:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ein weiteres Beispiel könnte sein, die Verwendung von Trackingcodes bei der Vorschau einer Vorlage in GenStudio for Performance Marketing zu verhindern. Das folgende Beispiel zeigt, wie Sie Tracking-Parameter zu Links in der exportierten Vorlage hinzufügen und dabei die Vorschau-Links sauber halten:

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statischer Inhalt

E-Mail- und Meta-Vorlagen sind häufig mit Bildern und CSS-Dateien verknüpft, die auf anderen Domains gehostet werden. Wenn GenStudio for Performance Marketing Miniaturansichten für Vorlagenvorschauen oder die daraus abgeleiteten Erlebnisse generiert, validiert es die Inhaltsquelle und bettet eine Kopie zu Vorschauzwecken ein.

Externe Dateien werden vorübergehend nur zum Zweck der Erstellung der Vorlagenvorschau eingebettet, wodurch sichergestellt wird, dass die Vorschau den Inhalt so wiedergibt, wie er zum Zeitpunkt der Erstellung angezeigt wird. Diese externen Dateien werden **nicht** dauerhaft in GenStudio for Performance Marketing gespeichert. Nachdem die Vorlagenvorschau erstellt wurde, verweist GenStudio for Performance Marketing weiterhin auf den in der Vorlage bereitgestellten Quell-Link.

### Inhalt aktualisieren

Wenn sich die Quelle nach der Erstellung der ersten Vorschau ändert, verwenden Sie die Funktion [Aktualisieren](/help/user-guide/content/use-templates.md#refresh-template), um die Vorlagenvorschau mit der neuesten Version des Inhalts aus den externen Quellen zu aktualisieren.

## Vorlagenbeispiele

+++Beispiel: E-Mail-Vorlage mit einem Abschnitt

Im Folgenden finden Sie ein einfaches Beispiel für eine HTML-Vorlage für eine E-Mail, die einen Abschnitt enthält. Der Kopf enthält einfaches Inline-CSS für die Formatierung. Der Textkörper enthält einen `pre_header`, einen `headline` und `image`[ Platzhalter](#content-placeholders), der von GenStudio for Performance Marketing verwendet wird, um während des E-Mail-Generierungsprozesses Inhalte einzufügen.

```html {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><a href="{{ link }}">
           <img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></a></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Beispiel: E-Mail-Vorlage mit mehreren Abschnitten

Im Folgenden sehen Sie dieselbe HTML-Vorlage wie im obigen Beispiel, jedoch mit zwei weiteren Abschnitten. Die Kopfzeile enthält Inline-CSS für die Formatierung einer Gruppe. Der Textkörper verwendet zwei Gruppen mit [Inhalts-Platzhaltern](#content-placeholders) die ein Präfix verwenden.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p>{{ body }}</p>
        <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p><img alt="{{ headline }}" src="{{ pod1_image }}" width="200" height="200" border="0"></p>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
        <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p><img alt="{{ headline }}" src="{{ pod2_image }}" width="200" height="200" border="0"></p>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Beispiel: Meta-Anzeigenvorlage

Im Folgenden finden Sie ein einfaches Beispiel für eine Meta-Anzeigenvorlage. Der Kopf enthält Inline-CSS für die Formatierung. Der Textkörper verwendet [Inhalts-Platzhalter](#content-placeholders) mit einem Präfix.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">{{ headline }}</div>
    <div class="ad-body">{{ body }}</div>
    <a href="{{ link }}" class="ad-cta">{{ CTA }}</a>
</div>
</body>
</html>
```

+++
