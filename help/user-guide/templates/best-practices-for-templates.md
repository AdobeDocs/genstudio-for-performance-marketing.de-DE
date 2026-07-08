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
workflow-type: ht
source-wordcount: 1330
ht-degree: 100%

---

# Best Practices für die Verwendung von Vorlagen

Vorlagen reduzieren den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellen, der vorkonfigurierte Layouts und Design-Elemente enthält.

Beachten Sie bei der Verwendung von Vorlagen mit GenStudio for Performance Marketing die folgenden Empfehlungen:

1. Erfahren Sie mehr über [Vorlagenelemente](#know-about-template-elements)
1. Konfigurieren Sie die [Kanalrichtlinien](#configure-channel-guidelines) für eine effektive Personalisierung von Inhalten
1. Berücksichtigen Sie beim Entwerfen mit [Barrierefreiheitsstandards](accessibility-for-templates.md) für ein optimales Erlebnis
1. Befolgen Sie die [kanalspezifischen Vorlagenrichtlinien](#follow-channel-specific-template-guidelines)
1. Beachten Sie bei der Verwendung von [Express-Vorlagen](/help/user-guide/templates/express-templates.md) die spezifischen Tipps unter [Best Practices für Express-zu-GenStudio-Vorlagen](#express-to-genstudio-template-best-practices).
>>
Erfahren Sie mehr über die Grundlagen von Vorlagenelementen und -verfahren in [Arbeiten mit Vorlagen](use-templates.md).Unter [Anpassen einer Vorlage](customize-template.md) erhalten Sie spezifische Anweisungen für die Verwendung in Ihrer nächsten Kampagne.

## Verwenden der richtigen Vorlagenelemente

Jeder Vorlagentyp verwendet verschiedene Elemente, um eine Struktur für die kanalspezifische Inhaltserstellung zu erstellen.[Machen Sie sich mit den Teilen einer Vorlage vertraut](use-templates.md#template-elements) und fügen Sie die besten Elemente für Ihre Inhalte und den jeweiligen Vorlagentyp hinzu.

Verwenden Sie beim Anpassen Ihrer Vorlage die Feldnamen anstelle dieser Elemente, wenn GenStudio for Performance Marketing Inhalte generieren muss.

Siehe [Vorlagenelemente](use-templates.md#template-elements).

## Verwenden von Platzhaltertext in Vorlagen

Platzhaltertext kann dazu beitragen, Syntax oder Struktur für Inhalte zu definieren, die später in einer Vorlage von einem Benutzer bzw. einer Benutzerin ausgefüllt werden.Beispiel: {first_name}.{last_name}@email.etc, um eine E-Mail-Adresse zu definieren.Einige gängige Trennzeichen sind jedoch bereits für andere Bedeutungen in GenStudio for Performance Marketing reserviert:

❌ `< >` – Wird für HTML-Tags verwendet.
❌ `{{ }}` – Wird für Handlebar-Ausdrücke verwendet.

Verwenden Sie für Platzhaltertext einfache Klammern (gerade oder geschweift), um Verwechslungen mit vorhandenen Tags zu vermeiden.

✅ `{first_name}` – Platzhalter für den Vornamen.

## Konfigurieren von Kanalrichtlinien

Die Definition klarer Kanalrichtlinien ist wichtig, um sicherzustellen, dass Ihre generierten Inhalte mit den Anforderungen und Zielen Ihrer Marke übereinstimmen.Mit den Kanalrichtlinien können Sie Regeln für Elemente wie Ton, Länge und Stil festlegen, die in Ihrer Vorlage verwendet werden.Sie können beispielsweise eine maximale Zeichenanzahl für den Text festlegen oder einen bestimmten CTA-Stil vorschreiben.Indem Sie diese Richtlinien im Voraus festlegen, müssen Sie nicht mehr in jedem KI-Prompt detaillierte Anweisungen formulieren. Dadurch wird der Prozess der Inhaltserstellung optimiert und Konsistenz in Ihren E-Mails wird sichergestellt.

Überprüfen und definieren Sie die [Kanalrichtlinien](/help/user-guide/guidelines/brands.md#channel-guidelines) Ihrer Marke für alle Schlüsselfelder in Ihrer Vorlage.Wenn Sie keine Richtlinien definieren, werden die [Standardkanalrichtlinien](/help/user-guide/guidelines/brands.md#default-channel-guidelines) angewendet, die Ihre Markenanforderungen möglicherweise nicht vollständig widerspiegeln.

![Spezifikationen des Hauptteils](/help/assets/channel-email-body.png)

Erfahren Sie, wie die [Richtlinien für Marken, Produkte und Personas](/help/user-guide/guidelines/overview.md) Inhalte beeinflussen und wie Sie diese an Ihre Marketing-Ziele anpassen können.

## Hochladen von Bildern für Vorlagen

Bilder, die in Vorlagen verwendet werden, sollten aus dem Content-Repository stammen und korrekt hochgeladen werden, um sicherzustellen, dass das Bild korrekt angezeigt wird.

Wenn eine Vorlage ein bis zum Rand reichendes Bild (mit vollständigem Anschnitt) aufweist, wird die Größe des ausgewählten Bilds automatisch an die vollständigen Vorlagenabmessungen angepasst.Wenn das Bild jedoch nicht dem Seitenverhältnis der Vorlage entspricht, wird es so zugeschnitten, dass es den Abmessungen der Vorlage entspricht, und wird möglicherweise nicht wie erwartet angezeigt.

Es gibt keine Funktion für die „automatische Anpassung“ von Bildern in Vorlagen.

Um das Zuschneiden von Bildern zu optimieren, müssen Benutzende das Seitenverhältnis des in der Vorlage zu verwendenden Bilds definieren, wenn dieses in das Content-Repository hochgeladen wird.Beim Hochladen einer genehmigten Vorlage:

1. [Führen Sie den Upload-Prozess für die Vorlage durch](/help/user-guide/templates/use-templates.md#add-a-template), bis Sie die Seite **[!UICONTROL Details hinzufügen]** erreichen.

2. Definieren Sie das Seitenverhältnis des in der Vorlage zu verwendenden Bilds unter **[!UICONTROL Anzeigenbreite (px)]** und **[!UICONTROL Anzeigenhöhe (px)]**.Dadurch wird das Bildfenster für den Abschnitt der Vorlage definiert, in dem das Bild angezeigt wird.

3. Wählen Sie im Abschnitt **[!UICONTROL Weitere Details]** das Dropdown-Menü **[!UICONTROL Bildgröße]** aus und wählen Sie _Auf feste Größe zuschneiden_ aus.
   ![Auf eine feste Größe zugeschnitten](images/crop-to-fixed-size.png "Auf eine feste Größe zugeschnitten"){width="80%"}

So bestimmen Sie die Größe und das Seitenverhältnis eines Bilds im Browser:

1. Überprüfen Sie das Bild.
   - Unter Windows/Linux:
      - Drücken Sie F12.
   - Unter macOS:
      - Drücken Sie Befehlstaste+Wahltaste+I.

1. Bewegen Sie den Mauszeiger über das Bild.

1. Beachten Sie das Seitenverhältnis.Verwenden Sie diese Option, um das Seitenverhältnis des Bilds in der Vorlage zu definieren.

Wenn diese Details beim Hochladen nicht angewendet werden, wird davon ausgegangen, dass das Bild das gesamte Seitenverhältnis der Vorlage einnimmt, und Bilder, die nicht genau diesem Seitenverhältnis entsprechen, werden abgeschnitten dargestellt.

![In einer Display-Anzeige zugeschnittenes Bild](images/cropped-display.png "Bildzuschnitt"){width="60%"}

**❌Zugeschnittenes Bild in einer Vorlage für eine Display-Anzeige**

![Bild, das in einer Display-Anzeige angezeigt wird](images/full-fit.png "Bild, das in der Display-Anzeige angezeigt wird"){width="60%"}

**✅Bild vollständig angezeigt**

## Befolgen der Richtlinien für kanalspezifische Vorlagen

Stellen Sie beim Erstellen von Vorlagen sicher, dass diese die spezifischen Anforderungen des jeweiligen Kanals erfüllen.Erstellen Sie Vorlagen, die das Layout und die visuellen Anforderungen für jeden Kanal berücksichtigen.Es gibt allgemeine Richtlinien, die für jede Vorlage gelten, z. B.:

- Verwenden Sie sauberes und responsives HTML sowie Inline-CSS
- Verwenden Sie Adobe- oder Google-Schriftarten
- Verwenden Sie **kein** JavaScript

{{note-css-effects}}

Hier finden Sie weitere Tipps und Einschränkungen zur Arbeit mit den einzelnen Vorlagentypen, um eine optimale Leistung sicherzustellen:

- [E-Mails](/help/user-guide/templates/email-template.md)
- [Display- und Banner-Anzeigen](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta-Anzeigen](/help/user-guide/templates/meta-template.md)

## Best Practices für Express-zu-GenStudio-Vorlagen

Die folgenden Tipps helfen Ihnen dabei, zuverlässige Ergebnisse zu erzielen, wenn Sie Designs aus [!DNL Adobe Express] in Vorlagen für [!DNL GenStudio for Performance Marketing] konvertieren.

### Verwenden von Vorlagen mit mehreren Varianten

In [!DNL Adobe Express] können Seiten in einer Vorlagendatei mehrere Größen- oder Seitenverhältnisvarianten darstellen.
Wenn Sie die Vorlage in [!DNL GenStudio for Performance Marketing] auswählen, werden alle Varianten in der Arbeitsfläche angezeigt.

Dieses Verhalten stellt eine Verbesserung gegenüber HTML-Vorlagen dar, die nur eine Variante pro Datei unterstützen.

### Sperren von Feldern, um zu steuern, was Marketing-Fachleute bearbeiten können

Verwenden Sie Sperren, um die Absicht zu kommunizieren.Sperren Sie beispielsweise einen Haftungsausschluss, damit dieser nicht von KI generiert wird, lassen Sie aber eine Überschrift flexibel, damit sie generiert werden kann.

Klicken Sie mit der rechten Maustaste auf ein beliebiges Element in [!DNL Adobe Express], um das Sperrverhalten festzulegen:

- **[!UICONTROL Vollständige Sperre]** – Das Element ist statisch und KI generiert keine Inhalte dafür.
- **[!UICONTROL Sperren, Bildersetzung zulassen]** – Größe und Position werden gesperrt, Benutzende können aber das Bild austauschen.Diese Option eignet sich gut für Logos.
- **[!UICONTROL Sperren, Textersetzung zulassen]** – Größe und Position werden gesperrt, Benutzende können den Text aber weiterhin bearbeiten.Die KI generiert dafür keine Inhalte automatisch.
- **Vollständig flexibel** (entsperrt) – Benutzende können das Element verschieben und seine Größe ändern. Die KI behandelt es dann als Inhalt, der generiert werden soll.

### Benennen von Ebenen für eine bessere KI-basierte Zuordnung

Wenn Sie ein Design in eine Vorlage konvertieren, scannt die KI das Design und ordnet Felder wie Überschrift, CTA und Textkörper zu.Die KI ordnet einfache Vorlagen häufiger genau zu als hochkomplexe Layouts.

**Best Practice:** Fügen Sie in die Platzhalterkopie den gewünschten Feldtyp ein (z. B. `headline`, `sub-headline` oder `CTA`), damit die KI Felder korrekt zuordnen kann.Durch dieses Verfahren können Zuordnungsfehler reduziert werden.

### In Vorlage konvertieren

1. Klicken Sie in [!DNL Adobe Express] auf **[!UICONTROL Freigeben]** > **[!UICONTROL In Vorlage konvertieren]**.
1. Nur die Registerkarten **[!UICONTROL Info]** und **[!UICONTROL Sperren]** werden in [!DNL GenStudio for Performance Marketing] übernommen.
1. Wählen Sie zum Zeitpunkt der Konvertierung aus, wie das Entsperren funktioniert:
   - **[!UICONTROL Benutzenden ermöglichen, zu entsperren]**
   - **[!UICONTROL Jegliches Entsperren verhindern]**
   - **[!UICONTROL Eine Passphrase festlegen]** – Ein Mittelweg, der spontane Änderungen erschwert, ohne den Zugriff dauerhaft zu sperren.

### Aufbewahren einer Kopie der ursprünglichen Design-Datei

Beim Konvertieren wird eine separate [!DNL Adobe Express]-Vorlagendatei erstellt, die ursprüngliche Design-Datei bleibt jedoch bearbeitbar.

**Tipp:** Behalten Sie das Original bei, damit Sie das Design überarbeiten, Varianten erstellen und später neue Vorlagen generieren können.

### Freigeben, um die Sichtbarkeit zu erhöhen

Nach der Konvertierung ist die Vorlage standardmäßig nur für Sie sichtbar.Sie können sie mit einzelnen Personen oder mit der gesamten Organisation teilen.

**Anforderung:** [!DNL Adobe Express] und [!DNL GenStudio for Performance Marketing] müssen dieselbe IMS-Organisation verwenden, um Vorlagen zu synchronisieren.Vorlagen werden in der Regel fast unmittelbar nach der Konvertierung in [!DNL GenStudio for Performance Marketing] angezeigt.

### Steuern der KI-Feldzuordnung

Nachdem Sie eine Vorlage ausgewählt haben, ordnet KI Felder einmal pro Vorlage zu und weist Labels wie **[!UICONTROL Primärmedien]**, **[!UICONTROL generiert]** oder **[!UICONTROL gesperrt]** zu. Sie können Zuordnungen manuell anpassen, wenn die KI Felder falsch zuweist.

Verwenden Sie den Umschalter **[!UICONTROL Generierung aktivieren]** für jedes Feld, um es vor der Generierung zu aktivieren oder zu deaktivieren.Sie können Zuordnungen manuell anpassen, wenn die KI Felder falsch zuweist.Für eine zukünftige Version sind dauerhafte Korrekturen an den Vorlagenzuordnungen geplant.

### Design in [!DNL Adobe Express], Zusammenstellung in [!DNL GenStudio for Performance Marketing]

Ziehen Sie die folgenden Design-Workflows in Betracht, um jeden Service optimal zu nutzen:

- Führen Sie Design-Arbeiten wie die Festlegung von Farben, Layouts und Grafiken in [!DNL Adobe Express] durch.
- Verwenden Sie [!DNL GenStudio for Performance Marketing], um Inhalte aus diesen Vorlagen zusammenzustellen und zu generieren.
- Verwenden Sie [!DNL Adobe Express]-Marken (Farben, Logos, Schriftarten und Grafiken) für die Design-Governance.
- Verwenden Sie [!DNL GenStudio for Performance Marketing]-Marken für Änderungen der Schriftfarbe nach der Generierung.

### Einschränkungen bei E-Mails

E-Mails werden auf der Horizon-Arbeitsfläche für den [!DNL Adobe Express]-Vorlagen-Workflow **nicht** unterstützt.Für E-Mails wird weiterhin der herkömmliche HTML-Vorlagenprozess verwendet.

### Nutzen benutzerdefinierter Schriftarten

Teams fragen oft, wie benutzerdefinierte Schriftarten mit [!DNL Adobe Express]-Vorlagen funktionieren. Admins müssen möglicherweise das Qualifizierungsangebot für benutzerdefinierte Schriftarten in der Admin Console annehmen, bevor diese Schriftarten verfügbar sind; siehe [Verwenden von  [!DNL Adobe Express] -Vorlagen](express-templates.md).
