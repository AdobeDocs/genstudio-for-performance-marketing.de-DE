---
title: Best Practices für Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 3322f783cd49ddcb897942e5e91590d53b554bdd
workflow-type: tm+mt
source-wordcount: 1347
ht-degree: 0%

---

# Best Practices für die Verwendung von Vorlagen

Vorlagen reduzieren den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellen, der vorkonfigurierte Layouts und Designelemente enthält.

Beachten Sie bei der Verwendung von Vorlagen mit GenStudio for Performance Marketing die folgenden Empfehlungen:

1. Know about [template elements](#know-about-template-elements)
1. Konfigurieren [Kanalrichtlinien](#configure-channel-guidelines) für die effektive Personalisierung von Inhalten
1. Design mit [Barrierefreiheitsstandards](accessibility-for-templates.md) für ein optimales Erlebnis
1. Befolgen [kanalspezifischen Vorlagenrichtlinien](#follow-channel-specific-template-guidelines)
1. Beachten Sie bei der Verwendung [Express](/help/user-guide/templates/express-templates.md)Vorlagen“ die spezifischen Tipps unter [Best Practices für Express-zu-GenStudio-Vorlagen](#express-to-genstudio-template-best-practices).
&#x200B;>>
Erfahren Sie mehr über die Grundlagen von Vorlagenelementen und Verfahren in [Arbeiten mit Vorlagen](use-templates.md). Außerdem erhalten Sie detaillierte [&#x200B; zum Anpassen einer Vorlage &#x200B;](customize-template.md) spezifische Anweisungen zur Verwendung in Ihrer nächsten Kampagne.

## Verwenden der richtigen Vorlagenelemente

Jeder Vorlagentyp verwendet verschiedene Elemente, um eine Struktur für die kanalspezifische Inhaltserstellung zu erstellen. [Machen Sie sich mit den Teilen einer Vorlage vertraut &#x200B;](use-templates.md#template-elements) fügen Sie die besten Elemente für Ihren Inhalt und Vorlagentyp hinzu.

Verwenden Sie beim Anpassen Ihrer Vorlage die Feldnamen anstelle dieser Elemente, bei denen GenStudio for Performance Marketing Inhalte generieren muss.

Siehe [Vorlagenelemente](use-templates.md#template-elements).

## Verwenden von Platzhaltertext in Vorlagen

Platzhaltertext kann dazu beitragen, Syntax oder Struktur für Inhalte zu definieren, die später in einer Vorlage von einem Benutzer ausgefüllt werden. Beispiel: {first_name}.{last_name}@email.etc, um eine E-Mail-Adresse zu definieren. Einige gängige Trennzeichen sind jedoch bereits für andere Bedeutungen in GenStudio for Performance Marketing reserviert:

❌ `< >` - Wird für HTML-Tags verwendet.
❌ `{{ }}` - Wird für Handlebar-Ausdrücke verwendet.

Verwenden Sie einfache Klammern (gerade oder geschweift), um Platzhaltertext anzugeben, um Verwechslungen mit vorhandenen Tags zu vermeiden.

✅ `{first_name}` - Platzhalter für Vornamen.

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

## Best Practices für Express-to-GenStudio-Vorlagen

Die folgenden Tipps helfen Ihnen dabei, zuverlässige Ergebnisse zu erhalten, wenn Sie Designs aus [!DNL Adobe Express] in Vorlagen für die [!DNL GenStudio for Performance Marketing] konvertieren.

### Verwenden von Vorlagen mit mehreren Varianten

[!DNL Adobe Express] können Seiten mehrere Größen- oder Seitenverhältnisvariationen in einer Vorlagendatei darstellen.
Wenn Sie die Vorlage in [!DNL GenStudio for Performance Marketing] auswählen, werden alle Varianten auf der Arbeitsfläche angezeigt.

Dieses Verhalten verbessert sich bei HTML-Vorlagen, die nur eine Variante pro Datei unterstützen.

### Sperren von Feldern, um zu steuern, was Marketing-Experten bearbeiten können

Verwenden Sie Sperren, um die Absicht zu kommunizieren. Sperren Sie beispielsweise einen Haftungsausschluss, damit er nie von KI generiert wird, sondern lassen Sie eine flexible Überschrift für die Generierung.

Klicken Sie mit der rechten Maustaste auf ein beliebiges Element in [!DNL Adobe Express], um das Sperrverhalten festzulegen:

- **[!UICONTROL Vollsperre]** - Das Element ist statisch, und KI generiert keine Inhalte dafür.
- **[!UICONTROL Sperren, Bildwechsel zulassen]** - Sperrt Größe und Position, ermöglicht es Benutzenden jedoch, das Bild auszutauschen. Diese Option eignet sich gut für Logos.
- **[!UICONTROL Sperren, Textersetzung zulassen]** - Sperrt Größe und Position, ermöglicht es Benutzenden jedoch, Text zu bearbeiten. KI generiert dafür nicht automatisch Inhalte.
- **Vollständig flexibel** (entsperrt) - Benutzer können das Element verschieben und seine Größe ändern, und KI behandelt es als zu generierenden Inhalt.

### Benennen von Ebenen für eine bessere KI-Zuordnung

Wenn Sie ein Design in eine Vorlage konvertieren, scannt KI das Design und ordnet Felder wie Überschrift, CTA und Textkörper zu. KI ordnet einfache Vorlagen häufiger genau zu als hochkomplexe Layouts.

**Best Practice:** Fügen Sie in die Platzhalterkopie den gewünschten Feldtyp ein (z. B. `headline`, `sub-headline` oder `CTA`), um die KI-Zuordnungsfelder korrekt zu gestalten. Auf diese Weise können Zuordnungsfehler reduziert werden.

### In Vorlage konvertieren

1. Klicken Sie in [!DNL Adobe Express] auf **[!UICONTROL Freigeben]** > **[!UICONTROL In Vorlage konvertieren]**.
1. Nur die Registerkarten **[!UICONTROL Info]** und **[!UICONTROL Sperren]** werden in [!DNL GenStudio for Performance Marketing] übertragen.
1. Wählen Sie zum Zeitpunkt der Konvertierung aus, wie die Entsperrung funktioniert:
   - **[!UICONTROL Benutzenden erlauben, zu entsperren]**
   - **[!UICONTROL Entsperren verhindern]**
   - **[!UICONTROL Passphrase festlegen]** - Ein Mittelweg, der vor gelegentlichen Änderungen abschreckt, ohne den Zugriff dauerhaft zu blockieren.

### Kopie der ursprünglichen Entwurfsdatei aufbewahren

Beim Konvertieren wird eine separate [!DNL Adobe Express]-Vorlagendatei erstellt, die ursprüngliche Design-Datei bleibt jedoch bearbeitbar.

**Tipp** Behalten Sie das Original bei, damit Sie das Design überarbeiten, Varianten erstellen und später neue Vorlagen erstellen können.

### Für bessere Sichtbarkeit freigeben

Nach der Konvertierung ist die Vorlage standardmäßig nur für Sie sichtbar. Sie können sie für Einzelpersonen oder für die gesamte Organisation freigeben.

**Anforderung:** [!DNL Adobe Express] und [!DNL GenStudio for Performance Marketing] müssen dieselbe IMS-Organisation verwenden, damit Vorlagen synchronisiert werden können. Vorlagen werden in der Regel fast sofort nach der Konvertierung in [!DNL GenStudio for Performance Marketing] angezeigt.

### Control AI-Feldzuordnung

Nachdem Sie eine Vorlage ausgewählt haben, ordnet KI Felder einmal pro Vorlage zu und weist Kennzeichnungen wie **[!UICONTROL Primärmedien]**, **[!UICONTROL generiert]** oder **[!UICONTROL gesperrt]** zu. Sie können Zuordnungen manuell anpassen, wenn KI Felder falsch zuweist.

Verwenden Sie den Umschalter **[!UICONTROL Generierung aktivieren]** für jedes Feld, um es vor der Generierung zu aktivieren oder zu deaktivieren. Sie können Zuordnungen manuell anpassen, wenn KI Felder falsch zuweist. Permanente Korrekturen an Vorlagenzuordnungen sind für eine zukünftige Version geplant.

### Design in [!DNL Adobe Express], Montage in [!DNL GenStudio for Performance Marketing]

Erwägen Sie die folgenden Design-Workflows, um jeden Service optimal zu nutzen:

- Vollständige Designarbeiten wie Farben, Layouts und Grafiken in [!DNL Adobe Express].
- Verwenden Sie [!DNL GenStudio for Performance Marketing], um Inhalte aus diesen Vorlagen zusammenzustellen und zu generieren.
- Verwenden Sie [!DNL Adobe Express] Marken (Farben, Logos, Schriftarten und Grafiken) für Design-Governance.
- Verwenden Sie [!DNL GenStudio for Performance Marketing] Marken für Änderungen der Schriftfarbe nach der Generierung.

### Einschränkungen bei E-Mails

E **Mail wird** der Arbeitsfläche „Horizont“ für den Workflow &quot;[!DNL Adobe Express]&quot; nicht unterstützt. E-Mail verwendet weiterhin den herkömmlichen HTML-Vorlagenprozess.

### Nutzung benutzerdefinierter Schriftarten

Teams fragen oft, wie benutzerdefinierte Schriftarten mit [!DNL Adobe Express] Vorlagen funktionieren. Administratoren müssen möglicherweise das Angebot für die Qualifizierung benutzerdefinierter Schriftarten in der Admin Console akzeptieren, bevor diese Schriftarten verfügbar sind. Siehe [Verwenden von  [!DNL Adobe Express] Vorlagen](express-templates.md).
