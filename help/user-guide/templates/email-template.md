---
title: Richtlinien für E-Mail-Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von E-Mail-Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '441'
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

Verwenden Sie beim Anpassen Ihrer E-Mail-Vorlage Platzhalter für Inhalte für die folgenden erforderlichen Felder:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (ausgewählt aus Content JPEG, PNG oder GIF)

GenStudio for Performance Marketing generiert automatisch die folgenden Felder. Rich-Text ist nicht aktiviert. Sie müssen keine Platzhalter für Inhalte anwenden für:

- `pre_header`
- `subject`

Die maximal zulässigen Felder in einer Vorlage sind 20. Weitere Informationen [&#x200B; Verwendung von Feldnamen in Vorlagen finden &#x200B;](/help/user-guide/templates/customize-template.md#content-placeholders) unter „Platzhalter für Inhalte“.

## E-Mail mit mehreren Abschnitten

_Abschnitte_ ermöglichen es Ihnen, Inhalte in verschiedene Gruppen zu organisieren und komplexere Layouts zu unterstützen. In GenStudio for Performance Marketing können Sie jeden Abschnitt mithilfe einer Gruppennamenskonvention definieren. Siehe [Anpassen von Vorlagenbereichen](/help/user-guide/templates/customize-template.md#sections-or-groups).

Vorlagen mit mehreren Abschnitten können 0, 2 oder 3 Abschnitte enthalten:

- Eine einfache Vorlage (keine Abschnitte) kann einen einzigen Satz von Vorlagenelementen generieren, wofür keine Namenskonvention für Gruppen erforderlich ist.
- Eine komplexe Vorlage (mehrere Abschnitte) kann bis zu drei Sätze von Vorlagenelementen generieren, wofür Sie die Namenskonvention für Gruppen einhalten müssen: `<groupname_fieldname>`.
- Bei Verwendung mehrerer Abschnitte werden die Elemente, die außerhalb eines Abschnitts verbleiben, nicht befüllt.

Im Folgenden finden Sie Beispiele für Feldnamen, die die Gruppennamenskonvention für zwei Abschnitte verwenden:

- In Abschnitt 1:`pod1_headline`, `pod1_body`, `pod1_cta`
- In Abschnitt 2:`pod2_headline`, `pod2_body`, `pod2_cta`

## Vorlagenbeispiele

+++Beispiel: E-Mail-Vorlage mit einem Abschnitt

Im Folgenden finden Sie ein einfaches Beispiel für eine HTML-E-Mail-Vorlage mit einem Abschnitt. Die `<head>` enthält einfaches Inline-CSS für die Formatierung, und die `<body>` verwendet Platzhalter für Inhalte wie `pre_header`, `headline`, `sub_headline`, `body`, `cta` und `image` mit Link und . Diese Platzhalter ermöglichen es GenStudio for Performance Marketing, dynamische Inhalte während der E-Mail-Generierung einzufügen.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++Beispiel: E-Mail-Vorlage mit mehreren Abschnitten

Hier sehen Sie dieselbe HTML-Vorlage im obigen Beispiel, jedoch mit zwei weiteren Abschnitten. Die Kopfzeile enthält Inline-CSS für die Formatierung einer Gruppe. Der Textkörper verwendet zwei Gruppen mit [Inhalts-Platzhaltern](#content-placeholders) die ein Präfix verwenden.

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
