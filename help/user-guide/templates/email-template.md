---
title: Richtlinien für E-Mail-Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von E-Mail-Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Richtlinien für E-Mail-Vorlagen

Eine Marketing-E-Mail-Vorlage dient als Grundlage für visuell ansprechende und responsive E-Mail-Kampagnen. Im Allgemeinen können Sie mit HTML-Vorlagen das Layout, die Typografie, die Farben und die Bildsprache entsprechend Ihren Markenrichtlinien steuern. Verwenden Sie beim Vorbereiten Ihrer Vorlage für die Verwendung in GenStudio for Performance Marketing semantische HTML und Inline-CSS für die Formatierung und vermeiden Sie Skripte oder externe Abhängigkeiten. Gut strukturierte HTML-Vorlagen können das Erlebnis der Empfängerinnen und Empfänger verbessern und die Zustellbarkeit und Interaktionsraten verbessern.

Befolgen Sie die folgenden Best Practices für das Design, wenn Sie E-Mail-Vorlagen für die Arbeit mit GenStudio for Performance Marketing anpassen:

- Verwenden von Adobe- oder Google-Schriftarten
- Verwenden Sie saubere und responsive HTML und Inline-CSS
- Verwenden **nicht** JavaScript
- Verwenden **nicht** eine feste Breite im Textkörper oder Container
- Verwenden **nicht** die Base64-Kodierung für Bilder, da dadurch die Vorlagengröße erheblich erhöht werden kann
- Die maximale Dateigröße für HTML beträgt 102 KB

## Erkannte Feldnamen

GenStudio for Performance Marketing generiert automatisch das `subject` für E-Mails. Verwenden Sie beim Anpassen Ihrer Vorlage Platzhalter für Inhalte für die folgenden erforderlichen Felder:

- `pre_header` (Rich-Text nicht aktiviert)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (ausgewählt aus Content JPEG, PNG oder GIF)

Die maximal zulässigen Felder in einer Vorlage sind 20. Weitere Informationen [ Verwendung von Feldnamen in Vorlagen finden ](/help/user-guide/content/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## E-Mail mit mehreren Abschnitten

_Abschnitte_ ermöglichen es Ihnen, Inhalte in verschiedene Gruppen zu organisieren, was komplexere Layouts unterstützt. In Genstudio für Performance Marketing können Sie jeden Abschnitt mithilfe einer Gruppennamenskonvention definieren. Siehe [Anpassen von Vorlagenbereichen](/help/user-guide/content/customize-template.md#sections-or-groups).

Vorlagen mit mehreren Abschnitten können 0, 2 oder 3 Abschnitte enthalten:

- Eine einfache Vorlage (null Abschnitte) kann einen einzigen Satz von Vorlagenelementen generieren, wofür keine Namenskonvention für Gruppen erforderlich ist.
- Eine komplexe Vorlage (mehrere Abschnitte) kann bis zu drei Sätze von Vorlagenelementen generieren, wozu die Einhaltung der Gruppennamen-Konvention erforderlich ist: (`groupname_fieldname`)

Beispielfeldnamen für zwei Abschnitte:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
