---
title: Figma Plugin für Adobe GenStudio for Performance Marketing
description: Erfahren Sie, wie Sie das Figma-Plug-in für GenStudio for Performance Marketing konfigurieren und verwenden.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: c6080555812fa82a7b71eee7e2deb963a881d9f4
workflow-type: tm+mt
source-wordcount: '2124'
ht-degree: 0%

---

# Figma-Plug-in für GenStudio for Performance Marketing

Das GenStudio for Performance Marketing Figma-Plug-in fügt dem Figma-Programm ein neues Bedienfeld hinzu, mit dem Sie markeninterne Inhalte generieren können.

Auf dieser Seite wird beschrieben, wie Sie das Plug-in konfigurieren und verwenden.

Zu den Funktionen dieses Plug-ins gehören:

* Ordnen Sie Figma-Textelemente GenStudio for Performance Marketing-Feldern zu, z. B. `headline`, `body`, `on_image_text` und mehr.
* Erstellen Sie neue markeninterne Meta-, LinkedIn- oder Display-[!DNL Experiences] basierend auf einer Marken-, Personen-, Produkt- und Textaufforderung.
* Erstellen Sie [!DNL Experiences] direkt im Figma-Dokument, indem Sie den Text in den zugeordneten Figma-Elementen durch die von GenStudio for Performance Marketing generierten Werte ersetzen.
* Vorhandene Inhalte je nach Aufforderung umformulieren, verkürzen, verlängern oder übersetzen.
* Generierte [!DNL Experiences] in mehrere Sprachen übersetzen.
* Exportieren Sie generierte [!DNL Experiences] als reduzierte Bilder in eine lokale Quelle.
* Exportieren Sie generierte [!DNL Experiences] nach GenStudio for Performance Marketing.
* Verwenden Sie Plug-in-Optionen, die sich an die ausgewählten Elemente auf der Figma-Arbeitsfläche anpassen.

>[!VIDEO](https://video.tv.adobe.com/v/3478809?learn=on)

## Erstellen einer Vorlage

Das Plug-in erfordert die ersten beiden Ebenen Ihres Figma-Dokuments, um dieser Konvention zu folgen:

* **Abschnitt** - Stellt das übergeordnete Projekt dar, das mehrere Vorlagen enthalten kann.
* **Frame** - Stellt eine Vorlage in einem Projekt dar. Die Vorlage kann mit Text, Bildern, Komponenten und anderen Elementen gefüllt werden.

### Meta-Vorlagen

Diese Vorlagengrößen werden unterstützt:

Für Instagram- oder Facebook-Posts:

* Breite: 1080 px (fest)
* Höhe: 1080 px oder 1350 px

Für Instagram- oder Facebook-Stories:

* Breite: 1080 px (fest)
* Höhe: 1920 px

Das -Plug-in bestimmt das Chrom des generierten Erlebnisses anhand der Höhe der Vorlage.

### Vorlagen anzeigen

Es gibt keine Anforderung für eine feste Größe. Anzeigevorlagen unterstützen jede Größe.

### LinkedIn-Vorlagen

* Breite: 1200 px (fest)
* Höhe: 1200 px, 628 px, 2292 px, 1800 px oder 1500 px

### Zuordnung der Feldrolle

Das Plug-in muss die verschiedenen Elemente Ihrer Vorlage verstehen, z. B. Überschrift, Haupttext oder Bild.

So weisen Sie Elementrollen zu:

1. Wählen Sie ein Element in Ihrer Vorlage aus (Text, Bild usw.)
1. Verwenden Sie das Dropdown-Menü, um eine Rolle zuzuweisen.

Das -Plug-in speichert diese Zuordnungen, um sie für generierte Inhalte zu verwenden. Ein Feld „role“ kann mehreren Vorlagenelementen zugeordnet werden.

![Zuordnung von Feldrollen](./field-role-mapping.png){width="600"}

### Ausnahmen bei der Feldzuordnung

{{$include /help/_includes/field-mapping-exceptions.md}}

## Neuen Inhalt generieren

Verwenden Sie GenStudio for Performance Marketing AI, um Elemente in Figma-Vorlagen zu generieren oder zu variieren.

1. Wenn Sie das GenStudio Plug-in Playground oder bereits vorbereitete Vorlagen verwenden, wählen Sie den Abschnittsknoten aus, der Ihre Anzeigenvorlagen enthält. Sie können dies über das Bedienfeld **Ebenen** oder durch direktes Klicken auf den Bereich auf der Arbeitsfläche tun.
   ![Abschnitt oder Varianten auswählen](./plugin-playground.png){width="500" zoomable="yes"}
1. Geben Sie im Plug-in-Fenster einen Projektnamen für die Varianten ein, wählen Sie eine Plattform für den Inhalt aus und füllen Sie die anderen erforderlichen Informationen aus. Klicken Sie anschließend auf **[!UICONTROL Setup beenden]**.
   ![Projektfenster einrichten](./setup-project.png){width="300" zoomable="yes"}
1. Wählen Sie die [!DNL Brand], [!DNL Persona] und [!DNL Product] aus, die für die Inhaltserstellung verwendet werden sollen.
1. Wählen Sie die Anzahl der zu erstellenden Varianten aus (bis zu acht).
1. Verwenden Sie die Schaltfläche unter **[!UICONTROL Inhalt auswählen]**, um Bilder aus Ihren Assets zu suchen und auszuwählen. Die 40 zuletzt hinzugefügten Assets werden zuerst angezeigt, und Sie können nach anderen Assets suchen. Die Größe der ausgewählten Bilder wird automatisch an die Vorlagen angepasst.
1. Geben Sie eine Textaufforderung ein. Für jedes Feld in der **[!UICONTROL Felder]**-Liste ist die Option **[!UICONTROL Aktion]** auf **[!UICONTROL Generieren]** für neue Inhalte festgelegt.
1. Ordnen Sie alle Feldrollen zu. Siehe [Zuordnung von Feldrollen](#field-role-mapping).
1. Klicken Sie auf die **[!UICONTROL Generieren]**-Schaltfläche.

## Übersetzen oder Erstellen und Kopieren von Varianten aus vorhandenen Inhalten

Verwenden Sie GenStudio for Performance Marketing AI, um Anzeigenkopien von Varianten zu generieren oder Figma-Vorlagen zu übersetzen.

1. Wählen Sie den Abschnittsknoten aus, der Ihre Anzeigenvorlagen enthält. Sie können dies über das Bedienfeld **Ebenen** oder durch direktes Klicken auf den Bereich auf der Arbeitsfläche tun.
   ![Abschnitt oder Varianten auswählen](./plugin-playground.png){width="500" zoomable="yes"}
1. Geben Sie im Plug-in-Fenster einen Projektnamen für die Varianten ein und wählen Sie eine Plattform für den Inhalt aus.
1. In **[!UICONTROL Was ist das Ziel?Wählen Sie]** **[!UICONTROL Varianten erstellen]** oder **[!UICONTROL Übersetzen]** und klicken Sie dann auf die Schaltfläche **[!UICONTROL Setup beenden]**.
   ![Projektfenster einrichten](./setup-project.png){width="300" zoomable="yes"}
1. Wählen Sie die [!DNL Brand], [!DNL Persona] und [!DNL Product] aus, die für die Inhaltserstellung verwendet werden sollen.
1. Wählen Sie die Anzahl der zu erstellenden Varianten aus.
1. Verwenden Sie die Schaltfläche unter **[!UICONTROL Inhalt auswählen]**, um Bilder aus Ihren Assets zu suchen und auszuwählen. Die 40 zuletzt hinzugefügten Assets werden zuerst angezeigt, und Sie können nach anderen Assets suchen. Die Größe der ausgewählten Bilder wird automatisch an die Vorlagen angepasst.
1. Geben Sie eine Textaufforderung ein. Für jedes Feld in der **[!UICONTROL Felder]**-Liste ist die Option **[!UICONTROL Aktion]** auf **[!UICONTROL Generieren]** für neue Inhalte festgelegt.
1. Ordnen Sie alle Feldrollen zu. Siehe [Zuordnung von Feldrollen](#field-role-mapping).
1. Wählen Sie jeden Feldtyp aus, um Varianten zu generieren oder zu übersetzen im Bedienfeld auf der linken Seite des Plug-ins und fügen Sie den anfänglichen Inhalt in jedes Feld **[!UICONTROL Anfänglicher Inhalt]** ein.
   ![Beispieltext im Feld Anfänglicher Inhalt](./initial-content-box.png){width="60%" zoomable="yes"}
1. Klicken Sie auf die **[!UICONTROL Generieren]**-Schaltfläche.

## Inhalte nach der Erstellung übersetzen

1. Wählen Sie eine Generation aus, die Sie übersetzen möchten.
   ![Generierung auswählen](./select-generation.png){width="200" zoomable="yes"}
1. Wählen Sie **[!UICONTROL Übersetzung]** aus und klicken Sie dann auf **[!UICONTROL Übersetzen]**.
1. Wählen Sie Ihre Zielsprache(n) aus.
1. Klicken Sie auf **[!UICONTROL Auswählen]**.

Zu den Übersetzungsergebnissen gehören:

* Es wird eine neue Seite mit übersetzten Inhalten angezeigt.
* Jede Übersetzung zeigt die Zielsprache oder das Gebietsschema an.
* Der ursprüngliche Inhalt bleibt auf der Originalseite unverändert.

![Ergebnisse der Übersetzung](./translation-results.png){width="60%" zoomable="yes"}

## Andere Aktionen für Inhaltsfelder nach der Generierung

Wenn Sie vorhandene Inhalte in einem Feld bearbeiten, werden im Plug-in-Bedienfeld nützliche Optionen angezeigt.

![Optionen für Plug-in-Aktionen](./figma-other-actions.png){width="300" zoomable="yes"}

Sie haben unter anderem folgende Möglichkeiten:

* Ändern Sie den **[!UICONTROL Wert]**, um Text direkt zu ändern. Das Ändern dieses Inhalts gilt automatisch für alle ausgewählten Varianten.
* Die KI kann viele Optionen **[!UICONTROL Aktion]** ausführen, darunter:

| Aktion | Beschreibung |
| --- | --- |
| **[!UICONTROL Generieren]** | Erzeugt eine neue Variante des Textes. |
| **[!UICONTROL Umformulierung]** | Erzeugt eine neue Variante des Textes. |
| **[!UICONTROL kürzen]** | Erzeugt eine kürzere Variante des Textes. |
| **[!UICONTROL Längen]** | Erzeugt eine längere Variante des Textes. |

Nachdem Sie eine **[!UICONTROL Aktion]**-Option ausgewählt haben, generieren Sie den Inhalt mit der Schaltfläche **[!UICONTROL Regenerieren]** neu.

## Bild erzeugen

Generieren von Bildern, die in Ihren Vorlagen über eine Textaufforderung verwendet werden sollen

1. Wählen Sie **[!UICONTROL Bild generieren]** aus.
1. Wählen Sie ein Modell aus dem Dropdown-Menü aus. Sie können auch alle benutzerdefinierten Modelle auswählen, die Sie erstellt haben.
1. Wählen Sie das Einstellungssymbol aus, um die Erzeugungseinstellungen anzupassen.
1. Optional: Wählen Sie ein Seitenverhältnis aus.
1. Optional: Passen Sie den Stil des Bildes an, indem Sie einen der folgenden Schritte ausführen:
   * Laden Sie ein Referenzbild von Ihrem Gerät oder AEM hoch, indem Sie **[!UICONTROL Bild hochladen]** auswählen.
   * Wählen Sie eines der Stock-Bilder von Adobe aus, indem Sie **[!UICONTROL Galerie durchsuchen]** auswählen.
   * Wählen Sie mithilfe des Schiebereglers einen Wert für die Stärke aus. Die Stärke passt an, wie streng sich Firefly an den von Ihnen angegebenen Stil hält.
1. Klicken Sie auf die Schaltfläche **&lt;**.
1. Eingabeaufforderung eingeben.
1. Klicken Sie auf das Symbol Generieren . Bilder werden im Plug-in-Bedienfeld angezeigt.
1. Bilder mithilfe einer der folgenden Methoden auf die Arbeitsfläche bringen:
   * Ziehen Sie ein Bild per Drag-and-Drop auf die Arbeitsfläche.
   * Wählen Sie einen Rahmen auf der Figma-Arbeitsfläche und wählen Sie ein Bild im Plugin-Fenster, um es in den Rahmen einzufügen.
   * Wählen Sie das Upload-Symbol aus, um ein Bild auf die Arbeitsfläche hochzuladen.
   * Wählen Sie die 3 Punkte und **[!UICONTROL Alles auf Figma herunterladen]**.
1. Optional: Wählen Sie die drei Punkte aus, um weitere Aktionen durchzuführen:
   * Wählen Sie **[!UICONTROL Weitere generieren]** aus, um die Eingabeaufforderung erneut auszuführen.
   * Wählen Sie **[!UICONTROL Eingabeaufforderung kopieren]**, um die Eingabeaufforderung zu kopieren.
1. Optional: Wählen Sie das Stiftsymbol aus, um das generative Ausfüllen und ähnliche Aktionen für ein einzelnes Bild zu generieren.

## Erzeugen ähnlicher Bilder

Einen Satz ähnlicher Bilder erzeugen

1. Wählen Sie die Karte **[!UICONTROL Ähnliche erstellen]** aus.
1. Wählen Sie ein Bild als Referenz aus, indem Sie einen der folgenden Schritte ausführen:
   * Wählen Sie ein Bild auf der Figma-Arbeitsfläche aus.
   * Wählen **[!UICONTROL Bild hochladen]**, um es von Ihrem Gerät hochzuladen.
   * Wählen Sie **[!UICONTROL AEM-Assets durchsuchen]** aus, um sie von AEM hochzuladen.
1. Klicken Sie auf das Symbol Generieren . Varianten werden im Plug-in-Bedienfeld angezeigt.
1. Bilder mithilfe einer der folgenden Methoden auf die Arbeitsfläche bringen:
   * Ziehen Sie ein Bild per Drag-and-Drop auf die Arbeitsfläche.
   * Wählen Sie einen Rahmen auf der Figma-Arbeitsfläche und wählen Sie ein Bild im Plugin-Fenster, um es in den Rahmen einzufügen.
   * Wählen Sie das Upload-Symbol aus, um ein Bild auf die Arbeitsfläche hochzuladen.
   * Wählen Sie die 3 Punkte und **[!UICONTROL Alles auf Figma herunterladen]**.
1. Optional: Wählen Sie die drei Punkte aus, um weitere Aktionen durchzuführen:
   * Wählen Sie **[!UICONTROL Weitere generieren]** aus, um die Eingabeaufforderung erneut auszuführen.
1. Optional: Wählen Sie das Stiftsymbol aus, um das generative Ausfüllen und ähnliche Aktionen für ein einzelnes Bild zu generieren.

## Entfernen des Hintergrunds

Entfernen des Hintergrunds eines Bildes.

1. Wählen Sie die Karte **[!UICONTROL Hintergrund entfernen]**.
1. Wählen Sie ein Bild als Referenz aus, indem Sie einen der folgenden Schritte ausführen:
   * Wählen Sie ein Bild auf der Figma-Arbeitsfläche aus.
   * Wählen **[!UICONTROL Bild hochladen]**, um es von Ihrem Gerät hochzuladen.
   * Wählen Sie **[!UICONTROL AEM-Assets durchsuchen]** aus, um sie von AEM hochzuladen.
1. Wählen Sie **[!UICONTROL Entfernen]** aus. Wenn das Bild auf der Arbeitsfläche ausgewählt wurde, wird das Bild auf der Figma-Arbeitsfläche ersetzt. Wenn das Bild auf einem Gerät oder in AEM ausgewählt wurde, können Sie es per Drag-and-Drop auf die Arbeitsfläche ziehen oder **[!UICONTROL Bild einfügen]** auswählen, um es auf der Arbeitsfläche zu platzieren.

## Generative Füllung

Wenden Sie generative Füllungen für einen Bereich eines Bildes an.

1. Wählen Sie die Karte **[!UICONTROL Generative]**) aus.
1. Wählen Sie ein Bild als Referenz aus, indem Sie einen der folgenden Schritte ausführen:
   * Wählen Sie ein Bild auf der Figma-Arbeitsfläche aus.
   * Wählen **[!UICONTROL Bild hochladen]**, um es von Ihrem Gerät hochzuladen.
   * Wählen Sie **[!UICONTROL AEM-Assets durchsuchen]** aus, um sie von AEM hochzuladen.
1. Wählen Sie das Pinselwerkzeug aus und erstellen Sie eine Maske.
1. Optional: Wählen Sie das Dropdown-Caret und passen Sie die Pinselgröße an.
1. Klicken Sie auf die Schaltfläche Zurücksetzen , um die Maske zu entfernen.
1. Wählen Sie optional das Symbol Hintergrund entfernen aus, um den Hintergrund zu entfernen.
1. Geben Sie eine Eingabeaufforderung ein, um die Generierung für die ausgewählte Maske zu leiten, und wählen Sie die Schaltfläche **[!UICONTROL Generieren]**.
1. Bilder mithilfe einer der folgenden Methoden auf die Arbeitsfläche bringen:
   * Ziehen Sie ein Bild per Drag-and-Drop auf die Arbeitsfläche.
   * Wählen Sie einen Rahmen auf der Figma-Arbeitsfläche und wählen Sie ein Bild im Plugin-Fenster, um es in den Rahmen einzufügen.
   * Wählen Sie das Upload-Symbol aus, um ein Bild auf die Arbeitsfläche hochzuladen.
   * Wählen Sie die 3 Punkte und **[!UICONTROL Alles auf Figma herunterladen]**.
1. Optional: Wählen Sie die drei Punkte aus, um weitere Aktionen durchzuführen:
   * Wählen Sie **[!UICONTROL Eingabeaufforderung kopieren]**, um die Eingabeaufforderung zu kopieren.
1. Optional: Wählen Sie das Stiftsymbol aus, um das generative Ausfüllen und ähnliche Aktionen für ein einzelnes Bild zu generieren.

## Eingabeaufforderung zur Bearbeitung

Bearbeiten Sie den Inhalt eines Bildes über eine Textanforderung.

1. Wählen Sie die Karte **[!UICONTROL Aufforderung zur Bearbeitung]** aus.
1. Wählen Sie ein Bild als Referenz aus, indem Sie einen der folgenden Schritte ausführen:
   * Wählen Sie ein Bild auf der Figma-Arbeitsfläche aus.
   * Wählen **[!UICONTROL Bild hochladen]**, um es von Ihrem Gerät hochzuladen.
   * Wählen Sie **[!UICONTROL AEM-Assets durchsuchen]** aus, um sie von AEM hochzuladen.
1. Wählen Sie das Einstellungssymbol aus, um die Erzeugungseinstellungen anzupassen.
1. Optional: Wählen Sie ein Seitenverhältnis aus und klicken Sie auf die Schaltfläche **&lt;**.
1. Geben Sie eine Eingabeaufforderung ein, um die Generierung zu leiten, und wählen Sie die Schaltfläche **[!UICONTROL Generieren]**.
1. Bilder mithilfe einer der folgenden Methoden auf die Arbeitsfläche bringen:
   * Ziehen Sie ein Bild per Drag-and-Drop auf die Arbeitsfläche.
   * Wählen Sie einen Rahmen auf der Figma-Arbeitsfläche und wählen Sie ein Bild im Plugin-Fenster, um es in den Rahmen einzufügen.
   * Wählen Sie das Upload-Symbol aus, um ein Bild auf die Arbeitsfläche hochzuladen.
   * Wählen Sie die 3 Punkte und **[!UICONTROL Alles auf Figma herunterladen]**.
1. Optional: Wählen Sie die drei Punkte aus, um weitere Aktionen durchzuführen:
   * Wählen Sie **[!UICONTROL Weitere generieren]** aus, um die Eingabeaufforderung erneut auszuführen.
   * Wählen Sie **[!UICONTROL Eingabeaufforderung kopieren]**, um die Eingabeaufforderung zu kopieren.
1. Optional: Wählen Sie das Stiftsymbol aus, um das generative Ausfüllen und ähnliche Aktionen für ein einzelnes Bild zu generieren.

## Generative Erweiterung

Erweitern Sie die Dimensionen Ihrer Bilder und fügen Sie generative Inhalte mit Generative expand hinzu. Mit Generative Expand können Sie schlecht passende Bilder in das am besten geeignete Seitenverhältnis für Banner, Meta-Anzeigen, LinkedIn-Anzeigen oder Display-Anzeigenvorlagen umwandeln.

1. Wählen Sie die Karte **[!UICONTROL Generatives]**&quot;.
1. Ein Bild auf der Arbeitsfläche auswählen.
1. Ändern Sie die Größe des Generierungsrahmens, um den temporären Rahmen auf die gewünschten neuen Abmessungen zu erweitern.
1. Optional: Verschieben Sie das Bild an eine beliebige Stelle innerhalb des Rahmens.
1. Geben Sie eine Eingabeaufforderung ein, um die Generierung zu leiten, und wählen Sie die Schaltfläche **[!UICONTROL Generieren]**.
1. Wählen Sie ein Bild auf der Arbeitsfläche aus, um Ihr Originalbild durch das generierte Ergebnis zu ersetzen.

## Exportieren von Erlebnissen

Varianten können aus Figma als GenStudio for Performance Marketing [!DNL Experiences] exportiert werden.

1. Wählen Sie den Inhalt aus, der in die Figma-Arbeitsfläche exportiert werden soll, indem Sie einen der folgenden Schritte ausführen:
   * Wählen Sie den Abschnitt Erstellung auf der Arbeitsfläche aus und klicken Sie dann **[!UICONTROL Plug-in]**&#x200B;Bedienfeld auf Alle für Export markieren .
     ![Generierungsabschnitt auswählen](./select-generation-section.png){width="200" zoomable="yes"}
   * Wählen Sie eine einzelne Generierung auf der Arbeitsfläche aus und klicken Sie dann im Plug **[!UICONTROL in-Bedienfeld]**&#x200B;Für Export markieren“.
     ![Individuelle Generierung auswählen](./select-generation.png){width="200" zoomable="yes"}
1. Wählen Sie im Seitenleistenmenü die Option Exportieren aus.
   ![Die Schaltfläche „Für Export markieren“ wird für eine Meta-Anzeige angezeigt](./mark-for-export.png){width="60%" zoomable="yes"}
1. Auswählen eines Ziels.
1. Klicken Sie **[!UICONTROL Exportieren]**, um den Inhalt zu exportieren.

Im Plug-in-Bedienfeld wird eine ZIP-Datei erstellt oder es wird ein Link zu **[!UICONTROL In GenStudio öffnen]** angezeigt. Verwenden Sie den ZIP-Link, um auszuwählen, wo die Datei gespeichert werden soll, oder wählen Sie **[!UICONTROL In GenStudio öffnen]**.

## Generationsverlauf

Das Plug-in verwaltet für jedes Feld einen Änderungsverlauf. Wählen Sie auf der Vorlagenseite in der Seitenleiste des Plug **[!UICONTROL ins &quot;]**&quot; aus.

![Option „Generierungsverlauf“ für eine Meta-Anzeige angezeigt](./generation-history.png){width="80%" zoomable="yes"}

## Fehlerbehebung

Beachten Sie die folgenden Best Practices und Tipps, wenn Text oder Bilder in generierten Varianten nicht ersetzt werden.

### Zugeordnete Felder

Wenn Text oder Bilder nicht ersetzt werden, überprüfen Sie, ob die Felder in der Plug-in-Benutzeroberfläche den GenStudio-Felderrollen zugeordnet wurden. Siehe [Zuordnung von Feldrollen](#field-role-mapping).

### Bestätigen der Verfügbarkeit von Schriftarten

Die Schriftart eines Textfelds muss auf Ihrem Computer verfügbar sein, damit sie während der Generierung ersetzt wird. Vergewissern Sie sich, dass alle in der Datei verwendeten Schriftarten auf Ihrem Computer verfügbar sind, insbesondere wenn die Datei auf dem Computer eines anderen Benutzers erstellt wurde.

### Unterstützung für Felderrollen in Erwägung ziehen

Bestimmte Kanäle unterstützen nur die Ersetzung in bestimmten Feldern. Beachten Sie Ausnahmen für die [Feldrollenzuordnung](#field-role-mapping).
