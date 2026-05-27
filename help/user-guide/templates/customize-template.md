---
title: Anpassen einer Vorlage
description: Erfahren Sie, wie Sie Ihre HTML-Vorlage mithilfe von Platzhaltern für Inhalte anpassen, die von Adobe GenStudio for Performance Marketing Generative AI erkannt werden.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
TQID: https://experienceleague.adobe.com/6gHxPvfz-30X3w2MYIc2Aj5SiGZokzOqSvOHYTQ-u7I
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: e8e0898054576454bad9ecdbd1a48b17f955e138
workflow-type: tm+mt
source-wordcount: 1646
ht-degree: 0%

---

# Anpassen einer Vorlage

Sie können eine Vorlage für die Verwendung in GenStudio for Performance Marketing anpassen, indem Sie Platzhalter oder Felder für Inhalte einfügen, die die generative KI zum Einfügen von Inhalten verwendet.

In den nächsten Abschnitten wird erläutert, wie Sie Ihre HTML-Vorlagen für GenStudio for Performance Marketing mithilfe der _[!DNL Handlebars]_&#x200B;anpassen. Die [!DNL Handlebars] Syntax verwendet regulären Text mit doppelten Klammern als Platzhalter für Inhalte. Unter [Was ist [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) im_ Handlebars-Sprachhandbuch _erfahren Sie, wie Sie Ihre Vorlage vorbereiten.

Sobald Ihre Vorlage fertig ist, können Sie sie [in GenStudio for Performance Marketing hochladen](use-templates.md#upload-a-template) und mit der Erstellung personalisierter E-Mails beginnen, die auf Ihrer benutzerdefinierten Vorlage basieren.

Befolgen Sie [Richtlinien für &#x200B;](accessibility-for-templates.md) Barrierefreiheit[&#x200B; und „Best &#x200B;](/help/user-guide/templates/best-practices-for-templates.md)&quot;, damit Sie mehr Ihrer Audience erreichen und ein optimales Erlebnis bieten können.

## Platzhalter für Inhalte

>[!TIP]
>
>Platzhalter für Inhalte sind **nicht** dasselbe wie Platzhaltertext in Inhalten, die zu einem späteren Zeitpunkt von einem Benutzer ausgefüllt werden sollen. Weitere Informationen finden Sie [Verwenden von Platzhaltertext in Vorlagen](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates).

GenStudio for Performance Marketing erkennt bestimmte Inhaltstypen oder [Elemente](use-templates.md#template-elements) innerhalb einer Vorlage, jedoch nur, wenn Sie sie mit einem [erkannten Feldnamen](#recognized-field-names) identifizieren.

Im Kopf oder Text einer HTML-Vorlage können Sie die [!DNL Handlebars] verwenden, um einen Platzhalter für Inhalte einzufügen, bei dem GenStudio for Performance Marketing die Vorlage mit tatsächlichem Inhalt füllen muss. GenStudio for Performance Marketing erkennt und interpretiert diese Platzhalter anhand des [erkannten _Feldnamens_](#recognized-field-names). Jeder Feldname ist mit bestimmten Regeln und Verhaltensweisen verknüpft, die bestimmen, wie Inhalte generiert und in Ihre Vorlage eingefügt werden.

Sie können beispielsweise `{{headline}}` mit der [!DNL Handlebars] Syntax verwenden, um anzugeben, wo die Überschrift der E-Mail platziert werden soll. GenStudio erkennt dieses Feld, generiert eine entsprechende Überschrift auf der Grundlage Ihrer Richtlinien und Eingabeaufforderungskriterien und fügt die Überschrift an dieser Stelle ein:

```handlebars
<div>{{headline}}</div>
```

### Erkannte Feldnamen

In der folgenden Tabelle sind die Feldnamen aufgeführt, die von GenStudio for Performance Marketing zum Hinzufügen eines Platzhalters zu einer Vorlage erkannt werden. Jedes Feld folgt bestimmten Kanal-Richtlinien, LLM-Anweisungen und rollenbasierten Regeln. Fügen Sie diese Feldnamen mithilfe der [!DNL Handlebars]-Syntax zu Ihrer Vorlage hinzu, wenn GenStudio for Performance Marketing einen bestimmten Inhaltstyp generieren soll.

| Feld | Rolle | Kanalvorlage |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Preheader | email |
| `{{headline}}` | Überschrift | E-Mail <br>Meta-Anzeige <br>Banner und Display-Anzeige <br>LinkedIn-Anzeige |
| `{{sub_headline}}` | Unterüberschrift | email<br>banner und Display-Anzeige |
| `{{introductory_text}}` | Einführungstext | LinkedIn-Anzeige |
| `{{body}}` | Textkörper | E-Mail-<br>Meta-Anzeige <br>Banner und Display-Anzeige |
| `{{cta}}` | Call to action<br>Siehe [Aktionsaufrufe](#calls-to-action) | E-Mail <br>Meta-Anzeige <br>Banner und Display-Anzeige <br>LinkedIn-Anzeige |
| `{{image}}` | Bild (Image) - Auswahl aus [!DNL Content] | E-Mail <br>Meta-Anzeige <br>Banner und Display-Anzeige <br>LinkedIn-Anzeige |
| `{{on_image_text}}` | Bei Bildtext<br> Siehe [Bei Bildtext](#on-image-text). | Meta-Anzeige <br>LinkedIn-Anzeige |
| `{{link}}` | Call to action on image<br>Siehe [Link on image](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing generiert in den folgenden Vorlagen automatisch bestimmte Felder:

- **E-Mail** Vorlage: Erfordert nicht, dass das `subject` Feld identifiziert wird
- **Meta-Anzeigenvorlage** erfordert nicht, dass Sie die `headline`-, `body`- und `CTA` identifizieren
- **Banner- und Display** Anzeigenvorlage erfordert keine Identifizierung des `CTA` Felds
- **LinkedIn** Anzeigenvorlage erfordert nicht, dass Sie die Felder `headline`, `introductory_text` und `CTA` identifizieren

>[!WARNING]
>
>Bei Instagram-Anzeigen wird die generierte Überschrift nicht im endgültigen Erlebnis angezeigt.

Beim Hochladen einer Vorlage auf GenStudio for Performance Marketing gibt es eine Grenze von 20 Feldern. Da das `subject` automatisch in einer E-Mail generiert wird, zählt es als ein Feld. Das bedeutet, dass in einer E-Mail-Vorlage 19 Felder zulässig sind.

>[!TIP]
>
>Sie können Ihre Vorlage mithilfe der [Vorlagenvorschau](#template-preview) in GenStudio for Performance Marketing überprüfen.

### Handlungsaufforderungen

Eine Call to action (CTA) enthält einen Satz und einen Link. Damit die Funktionen _[!UICONTROL Umformulieren]_ und _[!UICONTROL Link hinzufügen]_ während des Variantengenerierungsprozesses ordnungsgemäß funktionieren, müssen Sie Platzhalter für den Link und den Satz in Ihrer Vorlage einfügen.

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

GenStudio for Performance Marketing kann auch Ausdrücke mit varianten Aktionsaufrufen bereitstellen. Siehe [Call to action überarbeiten](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Verknüpfung auf Bild

Sie können Ihre E-Mail-Vorlage anpassen, damit Kreative einem Bild einen Link hinzufügen können. Ähnlich wie beim CTA-Link können Sie mithilfe der folgenden Anleitung einen `link` Platzhalter auf ein Bild-Tag anwenden:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

Beschreibung dieses Beispiels:

- `{{link}}` ist ein Platzhalter für die tatsächliche URL.
- `src="image-source.jpg"` sollte durch die tatsächliche Bildquellen-URL ersetzt werden.
- `{{imageDescription}}` ist ein benutzerdefinierter Feldname, der einen Platzhalter für den Alternativtext des Bildes bereitstellt, was für Barrierefreiheit und SEO nützlich ist.

### Alternativtext

Verwenden Sie einen benutzerdefinierten Feldnamen als Platzhalter, um eine Alternativtextbeschreibung (HTML-`alt="text"`) für ein Bild zu generieren. Der folgende `{{imageDescription}}`-Platzhalter wird mit dem Feld `{{image}}` innerhalb desselben `<img>`-Tags verwendet, um sicherzustellen, dass die Beziehung zwischen dem Bild und seiner Beschreibung bestehen bleibt.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

Beschreibung dieses Beispiels:

- `{{image}}` ist der Platzhalter für die Bildquellen-URL.
- `{{imageDescription}}` ist der Platzhalter für den Alternativtext, der eine Beschreibung des Bildes für Barrierefreiheits- und SEO-Zwecke bereitstellt.

### Barrierefreiheits-Kennzeichnung

Das Attribut `aria-label` wird verwendet, um einen barrierefreien Namen für Elemente zu definieren, die keine sichtbaren Beschriftungen haben. Dieses Attribut ist besonders nützlich in Vorlagen, in denen es wichtig ist, Kontext für interaktive Elemente bereitzustellen, z. B. eine CTA-Schaltfläche.

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

### Bei Bildtext

Der `{{on_image_text}}` Platzhalter wird verwendet, um eine Textüberlagerung kurzer wirkungsvoller Nachrichten anzugeben, die direkt auf dem Bild in einem Erlebnis platziert werden.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- 
this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Manuelle Feldnamen

Alle anderen Feldnamen sind benutzerdefiniert und werden als manuell ausgefüllte Felder behandelt. Beispielsweise können Sie einen Abschnitt für den Inhalt der Fußzeile reservieren.

Um einen bearbeitbaren Abschnitt zu erstellen, fügen Sie doppelte Klammern um den Abschnittsnamen hinzu:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

### Rich-Text-Bearbeitung

Verbessern Sie Ihre kreativen Inhalte während des [!DNL Create]-Prozesses mit Rich-Text-Bearbeitung. Die Arbeitsfläche bestimmt die Rich-Text-Funktion anhand des Speicherorts des Inhalts-Platzhalters. Die Rich-Text-Funktion ist nur verfügbar, wenn Sie Platzhalter für Inhalte als eigenständige Elemente oder in HTML-Tags auf Blockebene wie `<p>`, `<div>` oder `<span>` verwenden.

Die Rich-Text-Bearbeitung ist für eigenständige Inhalte in einem Absatz verfügbar:

```html
<p>{{body}}</p>
```

Wenn Sie einen Platzhalter für Inhalte in einem HTML-Attribut verwenden (z. B. `alt`, `href` oder `src`), wird die Rich-Text-Bearbeitung für dieses Feld nicht unterstützt.

Rich-Text-Bearbeitung **nicht** für `alt` Inhalte verfügbar:

```html
<img src="image.jpg" alt="{{image_description}}">
```

Wenn ein Feld mehrmals angezeigt wird, wird die Rich-Text-Funktion davon abhängig bestimmt, ob es in einer der Instanzen als HTML-Attribut verwendet wird. Wenn die Überschrift beispielsweise als Überschrift und als Alternativtext für ein Bild verwendet wird, hat das `alt`-Tag Vorrang.

Die Rich-Text-Bearbeitung **nicht** für `headline` verfügbar, da sie als `alt`-Inhalt verwendet wird:

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

Rich-Text-Bearbeitung kann für bestimmte Felder innerhalb bestimmter Kanäle verfügbar sein, z. B. `on_image_text` in Social Media (Meta, LinkedIn).

## Abschnitte oder Gruppen

Wenn für Ihre E-Mail-Vorlage mehrere Inhaltsbereiche erforderlich sind, z. B. mehrere Angebote oder Geschichten, können Sie diese mithilfe von Abschnitten oder Gruppen organisieren. _Abschnitte_ informieren GenStudio for Performance Marketing, dass die Felder in diesem Abschnitt ein hohes Maß an Kohärenz erfordern. Durch Festlegen dieser Beziehung kann die KI Inhalte generieren, die den kreativen Elementen im Abschnitt entsprechen.

Verwenden Sie einen Gruppennamen Ihrer Wahl als Präfix, um anzugeben, dass ein Feld Teil eines Abschnitts oder einer Gruppe ist. Verwenden Sie einen Feldnamen (z. B. `headline`, `body`, `image` oder `cta`) nach dem Unterstrich (`_`).

Syntax: `groupname_fieldname`

- _Richtig_ (👍): `pod1_body`
- _Falsch_ (❌): `pod1body`

Jeder Abschnitt kann nur einen der Feldtypen verwenden. Beispielsweise gehören die folgenden Felder zum Abschnitt `pod1` :

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Aufgrund dieser Regel können die Abschnitte nicht verschachtelt werden.

Jeder Vorlagentyp, z. B. E-Mail oder Meta-Anzeige, unterliegt kanalspezifischen Einschränkungen für die Verwendung von Abschnitten. Siehe [Kanalspezifische Richtlinien](/help/user-guide/templates/best-practices-for-templates.md) im Thema _Best Practices für die Verwendung von Vorlagen_.

Eine E-Mail-Vorlage kann beispielsweise bis zu drei Abschnitte enthalten. Daher können Sie drei Überschriften- und Hauptteilabschnitte haben:

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

GenStudio for Performance Marketing weiß, dass `pod1_headline` enger mit `pod1_body` als mit `pod2_body` verbunden ist.

>[!TIP]
>
>Unter [Strukturierte Eingabeaufforderungen](/help/user-guide/effective-prompts.md#structured-prompts) erfahren Sie, wie Sie eine Eingabeaufforderung erstellen, die für jeden Abschnitt in einer E-Mail mit mehreren Abschnitten unterschiedliche Inhalte generiert.

## Vorlagenvorschau

Wenn Sie [eine Vorlage hochladen](use-templates.md#upload-a-template) durchsucht GenStudio for Performance Marketing die HTML-Datei nach erkannten Feldern. Verwenden Sie die Vorschau, um Ihre [Vorlagenelemente](use-templates.md#template-elements) zu überprüfen und sicherzustellen, dass Sie sie ordnungsgemäß mit den [erkannten Feldnamen“ &#x200B;](#recognized-field-names).

Beispielvorschau für eine E-Mail-Vorlage:

![Erkannte Vorschaufelder](/help/assets/template-detected-fields.png "Erkannte Felder überprüfen"){zoomable="yes"}

Siehe [Vorlagen-Code-Editor](/help/user-guide/templates/code-editor.md).

### Vorschau steuern

Sie können die Sichtbarkeit spezieller Inhalte mithilfe integrierter Helper (spezielle Ausdrücke in der [!DNL Handlebars]-Vorlagensprache, die bestimmte Aktionen ausführen) steuern. Sie können beispielsweise eine bedingte Anweisung hinzufügen, die Tracking-Parameter zu Links in der exportierten Vorlage hinzufügt, während die Vorschau-Links sauber bleiben.

Der `_genStudio.canvas` wird beim Rendern einer Vorlage festgelegt und der `genStudio.export` wird beim Exportieren einer Vorlage festgelegt. Sie können sich dafür entscheiden, bestimmte Inhalte am Anfang einer E-Mail mit einem bedingten Wrapper einzuschließen, z. B. wenn die Vorlage für den Export verwendet wird:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ein weiteres Beispiel könnte sein, die Verwendung von Trackingcodes bei der Vorschau einer Vorlage in GenStudio for Performance Marketing zu verhindern. Das folgende Beispiel zeigt, wie Sie Tracking-Parameter zu Links in der exportierten Vorlage hinzufügen und dabei die Vorschau-Links sauber halten:

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Statischer Inhalt

E-Mail- und Meta-Vorlagen sind häufig mit Bildern und CSS-Dateien verknüpft, die auf anderen Domains gehostet werden. Wenn GenStudio for Performance Marketing Miniaturansichten für Vorlagenvorschauen oder die daraus abgeleiteten Erlebnisse generiert, validiert es die Inhaltsquelle und bettet eine Kopie zu Vorschauzwecken ein.

Externe Dateien werden vorübergehend nur zum Zweck der Erstellung der Vorlagenvorschau eingebettet, wodurch sichergestellt wird, dass die Vorschau den Inhalt so wiedergibt, wie er zum Zeitpunkt der Erstellung angezeigt wird. Diese externen Dateien werden **nicht** dauerhaft in GenStudio for Performance Marketing gespeichert. Nachdem die Vorlagenvorschau erstellt wurde, verweist GenStudio for Performance Marketing weiterhin auf den in der Vorlage bereitgestellten Quell-Link.

### Inhalt aktualisieren

Wenn sich die Quelle nach der Erstellung der ersten Vorschau ändert, verwenden Sie die Funktion [Aktualisieren](/help/user-guide/templates/use-templates.md#refresh-template), um die Vorlagenvorschau mit der neuesten Version des Inhalts aus den externen Quellen zu aktualisieren.
