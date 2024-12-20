---
title: Arbeiten mit Vorlagen
description: Erfahren Sie, wie Sie Vorlagen effektiv verwenden können, um Ihren Kreativprozess in Adobe GenStudio for Performance Marketing zu optimieren.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: e9c398cc81413fc22746d85abd6444c6bd42efe4
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 1%

---

# Arbeiten mit Vorlagen

GenStudio for Performance Marketing ermöglicht es Inhaltserstellern, konsistente markeninterne Marketing-Inhalte schnell mithilfe von _Vorlagen_ zu erstellen. Eine Vorlage reduziert den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellt, der vorkonfigurierte Layouts und Design-Elemente umfasst.

GenStudio for Performance Marketing unterstützt zwar nicht die direkte Erstellung von Vorlagen innerhalb des Programms, aber Sie können Vorlagen einfach mit gängigen Design-Tools wie Adobe InDesign, Illustrator oder Express entwerfen und vorbereiten. Sobald Ihr Design abgeschlossen ist, können Sie es für die Verwendung in GenStudio for Performance Marketing anpassen. Beginnen Sie mit der Verwendung von Vorlagen, indem Sie die folgenden Schritte ausführen:

1. **Vorlage entwerfen**: Verwenden Sie das bevorzugte Design-Tool, um das visuelle Layout Ihrer [Vorlage mit Elementen](#template-elements) wie Preheader, Überschrift, Textkörper, CTA, Bilder und Fußzeile, zu erstellen.

2. **Codieren Sie Ihre Vorlage**: Konvertieren Sie Ihr Design in HTML und Inline-CSS, um sicherzustellen, dass es auf verschiedenen Geräten sauber und responsiv ist. Beachten Sie die [Richtlinien zur Barrierefreiheit](accessibility-for-templates.md) um Ihre maximal vorgesehene Zielgruppe zu erreichen.

3. **Vorbereiten für GenStudio for Performance Marketing**: Passen Sie Ihre HTML-Vorlage mit der Vorlagensprache Handlebars an. Fügen Sie Platzhalter ein, um anzugeben, wo GenStudio for Performance Marketing Inhalte dynamisch generieren soll. Siehe „Anpassen [ Vorlage](customize-template.md) für GenStudio for Performance Marketing.

Wenn Sie diese Schritte befolgen, können Sie professionelle und effektive Vorlagen erstellen, die für die Verwendung in GenStudio for Performance Marketing bereit sind, sodass Sie Markeninhalte schnell und effizient erstellen können.

## Vorlagenelemente

Eine Vorlage ist ein Satz von Anweisungen, die mit HTML und Inline-CSS definiert werden und zur Erstellung von E-Mails, Social-Media-Anzeigen oder Display-Anzeigen verwendet werden können. Vorlagenelemente stellen die Struktur für die Inhaltserstellung bereit.

Im Folgenden finden Sie eine Liste der in Vorlagen verwendeten Elemente und einige Details zu ihren Eigenschaften:

- **Preheader**

   - Dient als sekundäre Betreffzeile in einer E-Mail und erweitert die Hauptbetreffzeile
   - Zwischen 40 und 50 Zeichen
   - Im Posteingang neben dem Betreff sichtbar, bevor die E-Mail geöffnet wird
   - Wird in E-Mail-Vorlagen verwendet

- **Kopfzeile**

   - Oberer Abschnitt der E-Mail, den der Empfänger beim Öffnen der E-Mail sieht
   - Legt den Ton fest und liefert Kontext für den enthaltenen Inhalt
   - Wird in E-Mail-Vorlagen verwendet

- **Überschrift**

   - Erster Inhalt, den der Empfänger sieht
   - Sollte fesselnd sein, Interesse zu wecken
   - Wird in Meta-Anzeigenvorlagen verwendet

- **body**

   - Hauptinhaltsbereich, in dem die primäre Nachricht übermittelt wird
   - Kann Text, Bilder und andere Medien enthalten
   - Wird in E-Mail- und Meta-Anzeigenvorlagen verwendet

- **CTA (Aktionsaufruf)**

   - Ermuntert den Empfänger, eine bestimmte Aktion auszuführen, z. B. auf einen Link zu klicken oder einen Kauf zu tätigen
   - Wird in E-Mail- und Meta-Anzeigenvorlagen verwendet

- **Bilder**

   - Verbessert die visuelle Attraktivität
   - Text aufteilen
   - Unterstützen der Nachricht
   - Sollte qualitativ hochwertig und auffällig sein
   - Wird in E-Mail- und Meta-Anzeigenvorlagen verwendet

- **Fußzeile**

   - Unterer Abschnitt, der zusätzliche Inhalte wie Kontaktdaten, Social-Media-Links, Haftungsausschlüsse und Abmeldeoptionen enthält
   - Wird in E-Mail-Vorlagen verwendet

- **Textüberlagerung**

   - Text auf einem Bild
   - Verwenden Sie , um Überschrift und Hauptteil zu unterstützen und zu verbessern
   - Wird in Meta-Anzeigenvorlagen verwendet

>[!TIP]
>
>Siehe die [erkannten Feldnamen](customize-template.md#recognized-field-names) die GenStudio for Performance Marketing für Vorlagen jedes Kanaltyps unterstützt.

## Vorlage anpassen

Sie [Ihre Vorlage](customize-template.md) zur Verwendung in GenStudio for Performance Marketing anpassen, indem Sie Platzhalter oder Felder für Inhalte einfügen, die die generative KI zum Einfügen von Inhalten verwendet. GenStudio for Performance Marketing erkennt bestimmte Felder, z. B. das `body`, und hält sich an die für die jeweilige Marke konfigurierten Kanalrichtlinien.

>[!TIP]
>
>Befolgen Sie [Richtlinien für ](accessibility-for-templates.md) Barrierefreiheit[ und „Best ](/help/user-guide/content/best-practices-for-templates.md)&quot;, damit Sie mehr Ihrer Audience erreichen und ein optimales Erlebnis bieten können.

## Vorlagen verwalten

Der [!DNL Templates] zeigt Ihr Inventar von Vorlagen an, die für die Generierung von Erlebnissen in GenStudio for Performance Marketing angepasst wurden. Sie können Vorlagen nach Kanaltyp filtern, z. B. E-Mail-, Display-Anzeigen- und Meta-Anzeigen.

![Liste der Inhaltsvorlagen](/help/assets/content-templates.png){width="650" zoomable="yes"}

### Vorlage hinzufügen

Bevor Sie eine Vorlage hochladen, stellen Sie sicher, dass sie vollständig vorbereitet und für die Verwendung in GenStudio for Performance Marketing bereit ist, indem Sie die Anleitung [Anpassen von Vorlagen](customize-template.md) befolgen.

**So fügen Sie eine Vorlage**:

1. Wählen Sie _[!DNL Content]_den Abschnitt **[!UICONTROL Vorlagen]**aus.

1. Klicken Sie **[!UICONTROL Vorlage hinzufügen]**.

1. Suchen Sie im Bereich _[!UICONTROL Genehmigte Vorlage hinzufügen]_ nach der HTML-Vorlagendatei oder ziehen Sie die HTML-Vorlagendatei in den Ablagebereich. Klicken Sie auf **[!UICONTROL Weiter]**.

1. Überprüfen Sie _[!UICONTROL Bereich „Erkannte]_ überprüfen“ die erkannten Felder. Vergewissern Sie sich, dass Sie die richtige Vorlage verwenden und dass alle Details erwartungsgemäß sind. Klicken Sie auf **[!UICONTROL Weiter]**.

   Beispielvorschau für eine E-Mail-Vorlage:

   ![Vorschau der Felder erkannt](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Wenn die Vorlage nicht korrekt ist, klicken Sie auf **[!UICONTROL Zurück]** und kehren Sie zum vorherigen Schritt zurück. Laden Sie die korrigierte Vorlagendatei hoch.

1. Benennen _[!UICONTROL im Bereich „Vorlagendetails angeben und hochladen]_ Ihre Vorlage und wählen Sie einen **[!UICONTROL Kanal]** Typ aus.

   Vorlagenname und Kanaltyp sind erforderlich. Zusätzliche Anforderungen können Folgendes umfassen:

   - **Meta**: erfordert Seitenverhältnis
   - **Anzeigen anzeigen**: erfordert Dimensionen

1. Fügen Sie so viele Details wie möglich hinzu, um die Vorlagenidentifizierung bei Suchen und Filtern zu verbessern.

1. Klicken Sie auf **[!UICONTROL Fertig]**.

### Vorlage aktualisieren

Vorlagen können statische Dateien wie Symbole oder Logos enthalten. Verwenden Sie „Aktualisieren“, um die Vorlagenvorschau mit den neuesten Versionen dieser Assets zu aktualisieren.

**Aktualisieren der Vorlage**:

1. Wählen Sie _[!DNL Content]_den Abschnitt **[!UICONTROL Vorlagen]**aus.

1. Klicken Sie auf eine Vorlage, um eine vollständige Ansicht und eine Liste der Details anzuzeigen.

1. Klicken **[!UICONTROL oben rechts auf]** Aktualisieren“ (kreisende Pfeile), um eine Aktualisierung aller in der Vorlage verwendeten Assets durchzuführen.

### Erstellen eines Erlebnisses mit einer Vorlage

Suchen und verwenden Sie eine vorhandene Vorlage in GenStudio for Performance Marketing, um weitere Erlebnisse zu erstellen.

**So erstellen Sie ein Erlebnis mit einer Vorlage**:

1. Wählen Sie _[!DNL Content]_den Abschnitt **[!UICONTROL Vorlagen]**aus.

1. Klicken Sie auf eine Vorlage, um eine vollständige Ansicht und eine Liste der Details anzuzeigen.

1. Klicken **[!UICONTROL oben rechts auf Erlebnis]** Pinsel erstellen), um die Vorlage zu verwenden.

1. Fahren Sie mit [Erstellen](/help/user-guide/create/overview.md) fort.
