---
title: Best Practices für Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 71b46454fa6fe2037ea6b103c0dfeedad74b8919
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Best Practices für die Verwendung von Vorlagen

Vorlagen reduzieren den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellen, der vorkonfigurierte Layouts und Designelemente enthält.

Beachten Sie bei der Verwendung von Vorlagen mit GenStudio for Performance Marketing die folgenden Empfehlungen:

1. Know about [template elements](#know-about-template-elements)
1. Konfigurieren [Kanalrichtlinien](#configure-channel-guidelines) für die effektive Personalisierung von Inhalten
1. Design mit [Barrierefreiheitsstandards](accessibility-for-templates.md) für ein optimales Erlebnis
1. Befolgen [kanalspezifischen Vorlagenrichtlinien](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Erfahren Sie mehr über die Grundlagen von Vorlagenelementen und Verfahren in [Arbeiten mit Vorlagen](use-templates.md). Außerdem erhalten Sie detaillierte [&#x200B; zum Anpassen einer Vorlage &#x200B;](customize-template.md) spezifische Anweisungen zur Verwendung in Ihrer nächsten Kampagne.

## Verwenden der richtigen Vorlagenelemente

Jeder Vorlagentyp verwendet verschiedene Elemente, um eine Struktur für die kanalspezifische Inhaltserstellung zu erstellen. [Machen Sie sich mit den Teilen einer Vorlage vertraut &#x200B;](use-templates.md#template-elements) fügen Sie die besten Elemente für Ihren Inhalt und Vorlagentyp hinzu.

Verwenden Sie beim Anpassen Ihrer Vorlage die Feldnamen anstelle dieser Elemente, bei denen GenStudio for Performance Marketing Inhalte generieren muss.

Siehe [Vorlagenelemente](use-templates.md#template-elements).

## Verwenden von Platzhaltertext in Vorlagen

Platzhaltertext kann dazu beitragen, Syntax oder Struktur für Inhalte zu definieren, die später in einer Vorlage von einem Benutzer ausgefüllt werden. Zum Beispiel: {first_name}.{last_name}@email.etc. , um eine E-Mail-Adresse zu definieren. Einige gängige Trennzeichen sind jedoch bereits für andere Bedeutungen in GenStudio for Performance Marketing reserviert:

❌ &lt; > - Wird für HTML-Tags verwendet.
❌ {{ }}{{ }} - Wird für Handlebar-Ausdrücke verwendet.

Verwenden Sie einfache Klammern (gerade oder geschweift), um Platzhaltertext anzugeben, um Verwechslungen mit vorhandenen Tags zu vermeiden.

✅ {first_name} - Platzhalter für Vornamen.

## Konfigurieren von Kanalrichtlinien

Die Definition klarer Kanal-Richtlinien ist wichtig, um sicherzustellen, dass Ihre generierten Inhalte mit den Anforderungen und Zielen Ihrer Marke übereinstimmen. Mit Kanalrichtlinien können Sie Regeln für Elemente wie Ton, Länge und Stil angeben, die in Ihrer Vorlage verwendet werden. Sie können beispielsweise eine maximale Zeichenanzahl für den Textkörper festlegen oder einen bestimmten call-to-action-Stil erfordern. Indem Sie diese Richtlinien im Voraus festlegen, müssen Sie in jeder KI-Eingabeaufforderung keine detaillierten Anweisungen mehr schreiben, den Prozess der Inhaltserstellung optimieren und die Konsistenz Ihrer E-Mails sicherstellen.

Überprüfen und definieren Sie die [Kanalrichtlinien](/help/user-guide/guidelines/brands.md#channel-guidelines) Ihrer Marke für alle Schlüsselfelder in Ihrer Vorlage. Wenn Sie keine Richtlinien definieren, werden die [Standardkanalrichtlinien](/help/user-guide/guidelines/brands.md#default-channel-guidelines) angewendet, die Ihre Markenanforderungen möglicherweise nicht vollständig widerspiegeln.

![Technische Daten des Textkörpers](/help/assets/channel-email-body.png)

Erfahren Sie, wie [Richtlinien für Marken, Produkte und Personas](/help/user-guide/guidelines/overview.md) generierte Inhalte beeinflussen und wie Sie sie an Ihre Marketing-Ziele anpassen können.

## Hochladen von Bildern für Vorlagen

Bilder, die in Vorlagen verwendet werden, sollten aus dem Inhalts-Repository stammen und müssen korrekt hochgeladen werden, um sicherzustellen, dass das Bild korrekt angezeigt wird.

Wenn eine Vorlage ein Bild mit vollständigem Anschnitt aufweist, wird die Größe des ausgewählten Bildes automatisch an die vollständigen Vorlagenabmessungen angepasst. Wenn das Bild jedoch nicht dem Seitenverhältnis der Vorlage entspricht, wird das Bild entsprechend den Vorlagenabmessungen zugeschnitten und möglicherweise nicht wie erwartet angezeigt.

Es gibt keine „AutoFit“-Funktion für Bilder in Vorlagen.

Um das Zuschneiden von Bildern aufzulösen, müssen Benutzende das Seitenverhältnis des Bildes definieren, das in der Vorlage verwendet werden soll, wenn sie in das Inhalts-Repository hochgeladen wird. Beim Hochladen einer genehmigten Vorlage:

1. [Durchlaufen Sie den Upload-Prozess der Vorlage](/help/user-guide/templates/use-templates.md#add-a-template) bis Sie die Seite **[!UICONTROL Details hinzufügen]** erreichen.

2. Definieren Sie das Seitenverhältnis des in der Vorlage zu verwendenden Bildes in **[!UICONTROL Anzeigenbreite (px)]** und **[!UICONTROL Anzeigenhöhe (px)]**. Dadurch wird das Bildfenster für den Bereich der Vorlage definiert, in dem das Bild angezeigt wird.

3. Wählen Sie im Abschnitt **[!UICONTROL Weitere]**) das Dropdown-Menü **[!UICONTROL Bildgröße]** und wählen Sie _Auf eine feste Größe zuschneiden_.
   ![Auf eine feste Größe zugeschnitten](images/crop-to-fixed-size.png "Auf eine feste Größe zugeschnitten"){width="80%"}

So bestimmen Sie die Größe und das Seitenverhältnis eines Bildes im Browser:

1. Überprüfen Sie das Bild.
   - Unter Windows/Linux:
      - Drücken Sie F12.
   - Auf macOS:
      - Drücken Sie Befehlstaste + Wahltaste + I.

1. Bewegen Sie den Mauszeiger über das Bild.

1. Beachten Sie das Seitenverhältnis. Verwenden Sie diese Option, um das Seitenverhältnis des Bildes in der Vorlage zu definieren.

Wenn diese Details beim Hochladen nicht angewendet werden, wird davon ausgegangen, dass das Bild das gesamte Seitenverhältnis der Vorlage ist, und Bilder, die nicht genau diesem Seitenverhältnis entsprechen, werden abgeschnitten angezeigt.

![Bild in einer Anzeige zugeschnitten](images/cropped-display.png "Bildzuschnitt"){width="60%"}

**❌Zugeschnittenes Bild in einer Anzeige-Vorlage**

![Bild, das in einer Anzeige angezeigt wird](images/full-fit.png "Bild, das in der Anzeige angezeigt wird"){width="60%"}

**✅Bild vollständig angezeigt**

## Befolgen der Richtlinien für kanalspezifische Vorlagen

Stellen Sie beim Erstellen von Vorlagen sicher, dass sie die spezifischen Anforderungen des vorgesehenen Kanals erfüllen. Erstellen Sie Vorlagen, die das Layout und die visuellen Anforderungen für jeden Kanal berücksichtigen. Es gibt allgemeine Richtlinien, die für jede Vorlage gelten, z. B.:

- Verwenden Sie saubere und responsive HTML und Inline-CSS
- Verwenden von Adobe- oder Google-Schriftarten
- Verwenden **nicht** JavaScript

{{note-css-effects}}

Weitere Tipps und Einschränkungen beim Arbeiten mit jedem Vorlagentyp finden Sie, um eine optimale Leistung sicherzustellen:

- [E-Mails](/help/user-guide/templates/email-template.md)
- [Anzeigen und Banner](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta Ads](/help/user-guide/templates/meta-template.md)
