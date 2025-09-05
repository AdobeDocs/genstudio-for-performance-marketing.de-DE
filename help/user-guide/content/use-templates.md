---
title: Arbeiten mit Vorlagen
description: Erfahren Sie, wie Sie Vorlagen effektiv verwenden können, um Ihren Kreativprozess in Adobe GenStudio for Performance Marketing zu optimieren.
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 2f15dc05f65ec216c7d242ffb3e14a83c76f3000
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 1%

---

# Arbeiten mit Vorlagen

GenStudio for Performance Marketing ermöglicht es Inhaltserstellern, konsistente markeninterne Marketing-Inhalte schnell mithilfe von _Vorlagen_ zu erstellen. Eine Vorlage reduziert den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellt, der vorkonfigurierte Layouts und Design-Elemente umfasst. Laden Sie zunächst eine benutzerdefinierte Vorlage in [!DNL Content] hoch oder verwenden Sie eine erste Vorlage in [!DNL Create]. [Einstiegsvorlagen](/help/user-guide/templates/starter-templates.md) bieten eine schnelle Möglichkeit, mit einem Standarddesign zu beginnen, während eine benutzerdefinierte Vorlage es Ihnen ermöglicht, Ihre einzigartigen Designs und Layouts zu verwenden.

GenStudio for Performance Marketing unterstützt zwar nicht die direkte Erstellung von Vorlagen innerhalb des Programms, aber Sie können Vorlagen einfach mit gängigen Design-Tools wie Adobe InDesign, Illustrator oder Express entwerfen und vorbereiten. Sobald Ihr Design abgeschlossen ist, können Sie es für die Verwendung in GenStudio for Performance Marketing anpassen. Beginnen Sie mit der Verwendung von Vorlagen, indem Sie die folgenden Schritte ausführen:

1. **Vorlage entwerfen**: Verwenden Sie das bevorzugte Design-Tool, um das visuelle Layout Ihrer [Vorlage mit Elementen](#template-elements) wie Preheader, Überschrift, Textkörper, CTA, Bilder und Fußzeile, zu erstellen.

2. **Codieren Sie Ihre Vorlage**: Konvertieren Sie Ihr Design in HTML und Inline-CSS, um sicherzustellen, dass es auf verschiedenen Geräten sauber und responsiv ist. Beachten Sie die [Richtlinien zur Barrierefreiheit](accessibility-for-templates.md) um Ihre maximal vorgesehene Zielgruppe zu erreichen.

3. **Vorbereiten für GenStudio for Performance Marketing**: Passen Sie Ihre HTML-Vorlage mithilfe der Handlebars-Vorlagensprache an. Fügen Sie Platzhalter ein, um anzugeben, wo GenStudio for Performance Marketing Inhalte dynamisch generieren soll. Siehe „Anpassen [ Vorlage](customize-template.md) für GenStudio for Performance Marketing.

Wenn Sie diese Schritte befolgen, können Sie professionelle und effektive Vorlagen erstellen, die für die Verwendung in GenStudio for Performance Marketing bereit sind, sodass Sie Markeninhalte schnell und effizient erstellen können.

## Vorlagenelemente

Eine Vorlage ist ein Satz von Anweisungen, die mit HTML und Inline-CSS definiert werden und zur Erstellung von E-Mails, Social-Media-Anzeigen oder Display-Anzeigen verwendet werden können. Vorlagenelemente stellen die Struktur für die Inhaltserstellung bereit.

Im Folgenden finden Sie eine Liste der in Vorlagen verwendeten Elemente und einige Details zu ihren Eigenschaften:

| **Element** | **Kanal** | **Beschreibung** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Preheader** | E-Mail | Eine sekundäre Betreffzeile in einer E-Mail, die normalerweise zwischen 40 und 50 Zeichen umfasst, wodurch die Haupt-Betreffzeile erweitert wird. Er wird im Posteingang neben dem Betreff angezeigt, bevor die E-Mail geöffnet wird. |
| **Kopfzeile** | E-Mail | Der obere Abschnitt der E-Mail, den der Empfänger beim Öffnen der E-Mail sieht, gibt den Ton an und liefert Kontext für den enthaltenen Inhalt. |
| **Überschrift** | Meta-, Banner- und Display-Anzeigen, LinkedIn | Der erste Inhalt, den der Empfänger sieht, sollte verlockend sein, um Interesse zu wecken. |
| **Unterüberschrift** | E-Mail-, Banner- und Display-Anzeigen | Ein zweites Textelement, das die Überschrift unterstützt. Er ist in der Regel kurz gehalten und so konzipiert, dass er die Hauptüberschrift ergänzt und die Aufmerksamkeit des Lesers weiter in den Inhalt lenkt. |
| **Einführungstext** | LinkedIn | Die primäre Nachricht übermittelt die Kernnachricht, ähnlich der Textkörper-Kopie. Es kann bis zu 150 Zeichen verwenden, einschließlich Leerzeichen, maximal vier Emojis und Satzzeichen. |
| **Text** | E-Mail-, Meta-, Banner- und Display-Anzeigen | Der Haupttext der Anzeige vermittelt die Kernbotschaft. Es sollte ansprechend, informativ und überzeugend sein, um die gewünschte Aktion aus dem Publikum zu fördern. |
| **Aktionsaufforderung** | E-Mail-, Meta-, Banner- und Display-Anzeigen, LinkedIn | Bei einer call-to-action-Schaltfläche werden eine Phrase und ein Link verwendet, um den Empfänger zu einer bestimmten Aktion zu ermutigen, z. B. zum Klicken auf einen Link oder zum Tätigen eines Kaufs. |
| **Bilder** | E-Mail-, Meta-, Banner- und Display-Anzeigen, LinkedIn | Verbessern Sie die visuelle Attraktivität, teilen Sie Text auf und unterstützen Sie die Botschaft. Bilder sollten von hoher Qualität und auffällig sein. |
| **Fußzeile** | E-Mail | Der untere Abschnitt der E-Mail enthält zusätzliche Inhalte wie Kontaktdaten, Social-Media-Links, Haftungsausschlüsse und Abmeldeoptionen. |
| **Textüberlagerung** | Meta-Anzeige | Text, der auf einem Bild platziert wird, um die Überschrift und den Hauptteil des Inhalts zu unterstützen und zu verbessern. |

>[!TIP]
>
>Siehe die [erkannten Feldnamen](customize-template.md#recognized-field-names) die GenStudio for Performance Marketing für Vorlagen jedes Kanaltyps unterstützt.

## Vorlage anpassen

Sie [Ihre Vorlage](customize-template.md) zur Verwendung in GenStudio for Performance Marketing anpassen, indem Sie Platzhalter oder Felder für Inhalte einfügen, die die generative KI zum Einfügen von Inhalten verwendet. GenStudio for Performance Marketing erkennt bestimmte Felder, z. B. das `body`, und hält sich an die für die jeweilige Marke konfigurierten Kanalrichtlinien.

>[!TIP]
>
>Befolgen Sie [Richtlinien für ](accessibility-for-templates.md) Barrierefreiheit[ und „Best ](/help/user-guide/content/best-practices-for-templates.md)&quot;, damit Sie mehr Ihrer Audience erreichen und ein optimales Erlebnis bieten können.

## Vorlagen verwalten

Der _[!DNL Templates]_&#x200B;zeigt Ihr Inventar von Vorlagen an, die für die Generierung von Erlebnissen in GenStudio for Performance Marketing angepasst wurden.

### Vorlagen suchen

Jede [!DNL Content] bietet Filteroptionen, mit denen Sie Ihre Suche nach dem idealen Asset, Erlebnis oder einer Vorlage eingrenzen können. Es gibt Filter, die auf [Richtlinien](/help/user-guide/guidelines/overview.md), [Schlüsselwörtern](asset-details.md#user-defined-metadata) und [Attributkategorien](/help/user-guide/insights/attributes.md#categories) basieren, um Suchergebnisse einzugrenzen.

Beispielsweise können Sie eine Vorlage eines bestimmten Kanaltyps oder Seitenverhältnisses suchen, der von Ihnen erstellt wurde:

- **[!UICONTROL Erstellt von]**: begrenzt die Liste _[!UICONTROL Vorlagen]_ so, dass nur die von Ihnen oder einer bestimmten Person erstellten Vorlagen angezeigt werden.
- **[!UICONTROL Seitenverhältnis]**: Begrenzt die Liste _[!UICONTROL Vorlagen]_, um Vorlagen anzuzeigen, die für ein bestimmtes Seitenverhältnis entwickelt wurden.

Im folgenden Beispiel werden Filter nach Kanaltyp angezeigt, z. B. E-Mail, Display-Anzeigen, Meta-Anzeigen und LinkedIn-Anzeigen.

![Inhaltsvorlagenliste](/help/assets/content-templates-filter.png "Durchsuchen der LinkedIn-Vorlagen"){width="650"}

Die Vorlagensuchfunktion ist bei der Auswahl [!UICONTROL &#x200B; Vorlage für eigene oder bezahlte &#x200B;] während der Erstellung verfügbar. Wenn bestimmte Filteroptionen nicht sichtbar sind, bedeutet dies, dass keine Vorlagen im Repository den entsprechenden Metadatenkriterien entsprechen. Stellen Sie sicher, dass Vorlagen ordnungsgemäß mit Metadaten getaggt sind, damit sie über diese Filter auffindbar sind.

### Vorlage hinzufügen

Bevor Sie eine Vorlage hochladen, stellen Sie sicher, dass sie vollständig vorbereitet und für die Verwendung in GenStudio for Performance Marketing bereit ist, indem Sie die Anleitung in [Anpassen von Vorlagen](customize-template.md) befolgen.

**So fügen Sie eine Vorlage**:

1. Wählen Sie _[!DNL Content]_&#x200B;den Abschnitt **[!UICONTROL Vorlagen]**&#x200B;aus.

2. Klicken Sie **[!UICONTROL Vorlage hinzufügen]**.

3. Suchen Sie im Bereich _[!UICONTROL Genehmigte Vorlage hinzufügen]_ die HTML-Vorlagendatei oder ziehen Sie die HTML-Vorlagendatei in den Ablagebereich. Klicken Sie auf **[!UICONTROL Weiter]**.

4. Überprüfen Sie _[!UICONTROL Bereich „Erkannte]_ überprüfen“ die Felder. Vergewissern Sie sich, dass Sie die richtige Vorlage verwenden und dass alle Details erwartungsgemäß sind.

   Beispielvorschau für eine E-Mail-Vorlage:

   ![Vorschau der Felder erkannt](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Wenn die Vorlage nicht korrekt ist, klicken Sie auf **[!UICONTROL Zurück]** und kehren Sie zum vorherigen Schritt zurück. Laden Sie die korrigierte Vorlagendatei hoch. Oder verwenden Sie den [Vorlagen-Code](/help/user-guide/content/code-editor.md)Editor, um einfache Korrekturen vorzunehmen.

5. Klicken Sie **[!UICONTROL Weiter]** wenn Sie mit der Vorlagenvorschau zufrieden sind.

6. Benennen _[!UICONTROL unter „Vorlagendetails angeben und hochladen]_ Ihre Vorlage und wählen Sie einen **[!UICONTROL Kanal]** Typ aus.

   Vorlagenname und Kanaltyp sind erforderlich. Zusätzliche Anforderungen können Folgendes umfassen:

   - **Meta**: erfordert Seitenverhältnis
   - **Banner- und Display-Anzeige**: Erfordert Dimensionen

7. Fügen Sie so viele Details wie möglich hinzu, um die Vorlagenidentifizierung bei Suchen und Filtern zu verbessern.

8. Klicken Sie auf **[!UICONTROL Fertig]**.

### Vorlage aktualisieren

Vorlagen können statische Dateien wie Symbole oder Logos enthalten. [Statischer Inhalt](/help/user-guide/content/customize-template.md#static-content) wird nach der Erstellung der Vorlagenvorschau nicht gespeichert. GenStudio for Performance Marketing verweist weiterhin auf den in der Vorlage bereitgestellten Quell-Link. Verwenden Sie „Aktualisieren“, um die Vorlagenvorschau mit den neuesten Versionen dieser Assets zu aktualisieren.

**Aktualisieren der Vorlage**:

1. Wählen Sie _[!DNL Content]_&#x200B;den Abschnitt **[!UICONTROL Vorlagen]**&#x200B;aus.

2. Klicken Sie auf eine Vorlage, um eine vollständige Ansicht und eine Liste der Details anzuzeigen.

3. Klicken **[!UICONTROL oben rechts auf]** Aktualisieren“ (kreisende Pfeile), um eine Aktualisierung aller in der Vorlage verwendeten Assets durchzuführen.

### Erstellen eines Erlebnisses mit einer Vorlage

Suchen und verwenden Sie eine vorhandene Vorlage in GenStudio for Performance Marketing, um weitere Erlebnisse zu erstellen.

**So erstellen Sie ein Erlebnis mit einer Vorlage**:

1. Wählen Sie _[!DNL Content]_&#x200B;den Abschnitt **[!UICONTROL Vorlagen]**&#x200B;aus.

2. Klicken Sie auf eine Vorlage, um eine vollständige Ansicht und eine Liste der Details anzuzeigen.

3. Klicken **[!UICONTROL oben rechts auf Erlebnis]** Pinsel erstellen), um die Vorlage zu verwenden.

4. Fahren Sie mit [Erstellen](/help/user-guide/create/overview.md#create-use-cases) fort.

## Vorlagen aus AJO und Marketo

Sie können eine Vorlage hochladen, die Sie in Adobe Journey Optimizer (AJO) oder Marketo erstellt haben. GenStudio for Performance Marketing erkennt anwendungsspezifische Muster und ignoriert sie, wobei das Originalformular für die weitere Verwendung in AJO oder Marketo beibehalten wird. Sie müssen keine Änderungen an der ursprünglichen AJO- oder Marketo-Syntax vornehmen.

Zu den erkannten Anwendungsmustern gehören:

- **AJO**: `{{profile.*}}`, `{{context.*}}`
- **Marketo**: `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Voraussetzungen**

- Die Anwendung (AJO, Marketo) und GenStudio for Performance Marketing müssen zur Integration derselben IMS-Organisation angehören
- Benutzer müssen die Rolle „Mitarbeiter“ (die niedrigste Ebene) oder höher haben

>[!ENDSHADEBOX]

Passen Sie [ Ihre Vorlage mit ](/help/user-guide/content/customize-template.md) an, um anzugeben, wo GenStudio for Performance Marketing Inhalte für Sie generieren soll. [Vorlage hinzufügen](#add-a-template) zum [!DNL Content]-Repository hinzufügen und die Vorlage validieren. Nehmen Sie mit dem Code-Editor kleinere Korrekturen vor.
