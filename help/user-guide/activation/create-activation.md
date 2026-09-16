---
title: Aktivierungs-Workflow
description: Erfahren Sie mehr über den Aktivierungs-Workflow für Werbeanzeigen.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 6cb428b368f75e0b646cfa4e6536a4728fdf40e2
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 1%
---
# Aktivierungs-Workflow

[!DNL Activate] aktiviert veröffentlichte Erlebnisse für ihre Paid-Ad-Kanäle. Ein GenStudio for Performance Marketing-Erlebnis ist eine Marketing-Kampagnenkomponente (z. B. eine Anzeige), die für eine bestimmte Zielgruppe in einem gebührenpflichtigen Anzeigenkanal vorbereitet wird. Die zu aktivierenden Erlebnisse umfassen drei Hauptkomponenten:

* **Medien-Assets**: Bilder oder Videos, die in Ihrem Anzeigenerlebnis enthalten sind. Unterstützte Dateitypen und Seitenverhältnisse variieren je nach Kanal und Format.

* **Text**: Alle in Ihrer Anzeige enthaltenen Formen von Kopien, einschließlich Überschriften, Textkörper und call-to-action-Elemente.

* **Metadaten**: Benutzerdefinierte Attribute zur Verbesserung von Leistungsanalyse, Filterung und Tracking. Metadaten sind für die endgültige Anzeigenzielgruppe in der Regel nicht sichtbar.

Sie bereiten diese Komponenten vor der Aktivierung in [!DNL Content] vor und genehmigen sie. [!DNL Activate] erstellt oder bearbeitet keine genehmigten Assets, Überschriften oder Textkörper. Es wird nur das für jeden Kanal erforderliche Setup angewendet und dann das Erlebnis veröffentlicht.

Eine einzelne Aktivierungstabelle kann Erlebnisse für mehrere Paid-Ad-Kanäle und Anzeigenformate gleichzeitig enthalten.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## Kanalkonten verbinden

Ein GenStudio-Systemmanager oder -Editor muss die Werbekonten für jeden gebührenpflichtigen Anzeigenkanal verbinden, bevor Sie ein Erlebnis für diesen Kanal aktivieren können. Die Schritte für diesen Prozess finden Sie unter [Paid-Media-Konten verbinden](/help/user-guide/connectors/connect-channel.md).

## Starten einer Aktivierung

Starten einer Aktivierung von einem von zwei Einstiegspunkten aus:

* **Von[!DNL Content]**: Filtern Sie nach Erlebnissen, wählen Sie ein oder mehrere veröffentlichte Erlebnisse aus und klicken Sie dann **[!UICONTROL der oberen Aktionsleiste]** Aktivieren“.
* **Von[!DNL Activate]**: Klicken Sie auf der [!DNL Activate] Landingpage auf **[!UICONTROL + Neue Aktivierung]**. Dadurch wird die Erlebnisgalerie geöffnet, in der Sie Erlebnisse zur Aktivierung auswählen.

Suchen Sie in beiden Fällen nach Erlebnisnamen oder filtern Sie nach mehreren Kanälen, um die gewünschten Erlebnisse zu finden.

Wenn Sie Erlebnisse im Anzeigeformat auswählen, geben Sie an, welche Anzeigeplattform verwendet werden soll: Google Campaign Manager 360, Innovid, Amazon Ads oder The Trade Desk. Klicken Sie dann auf **[!UICONTROL Aktivierung starten]**. Für andere Formate wie Meta, LinkedIn, TikTok, YouTube und ChatGPT leitet [!DNL Activate] die Plattform aus dem Kanal des Erlebnisses ab und überspringt diesen Schritt.

[!DNL Activate] generiert eine Aktivierungstabelle, in der alle ausgewählten Erlebnisse aufgelistet sind. Die Tabelle ist nach Anzeigenformat und Kanal in Untertabellen unterteilt, z. B. Einzelbild von Meta oder Einzelbild von LinkedIn. Jede Zeile stellt eine Anzeige dar. Bei den meisten Kanälen, z. B. LinkedIn, TikTok und Anzeigekanälen, generiert ein Erlebnis mit mehreren Seitenverhältnissen eine Zeile pro Seitenverhältnis. Löschen Sie alle Zeilen, die Sie nicht benötigen. Meta bildet die Ausnahme. Eine Meta-Anzeige kann mehrere Seitenverhältnisse in einer einzigen Anzeige enthalten, sodass ein Meta-Erlebnis mit mehreren Seitenverhältnissen immer noch nur eine Zeile generiert.

Ihre Aktivierungstabelle wird beim Öffnen automatisch als Entwurf gespeichert. Sie können den Entwurf jederzeit vor der Veröffentlichung verlassen und fortsetzen.

Um einer bereits geöffneten Aktivierungstabelle weitere Erlebnisse hinzuzufügen, klicken Sie **[!UICONTROL oben rechts in der Tabelle auf]** Weitere Erlebnisse hinzufügen“. Dadurch wird die Erlebnisgalerie erneut geöffnet, sodass Sie zusätzliche Erlebnisse auswählen können, die [!DNL Activate] zur vorhandenen Tabelle hinzufügt.

**[!UICONTROL Weitere Erlebnisse hinzufügen]** ermöglicht auch die Aktivierung auf mehr als einer Anzeigeplattform in derselben Tabelle. Bei Erlebnissen im Anzeigeformat müssen Sie zunächst eine einzelne Anzeigeplattform auswählen, aber Sie können auf **[!UICONTROL Weitere Erlebnisse hinzufügen]** klicken, weitere Erlebnisse im Anzeigeformat auswählen und eine andere Anzeigeplattform auswählen, als die, die sich bereits in Ihrer Tabelle befindet. Sie können beispielsweise The Trade Desk-Anzeigen zu einer Tabelle hinzufügen, die bereits Innovid-Anzeigen enthält.

## Konfigurieren von Anzeigen- und Platform-Setup-Details

Genehmigte Assets, Überschriften und Textkörper sind gesperrt und können in der Aktivierungstabelle nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Die verbleibenden Felder können bearbeitet werden und variieren je nach Kanal:

>[!NOTE]
>
>[!DNL Content] ruft ein Ziel wie Meta oder LinkedIn in einem **channel** auf. [!DNL Activate] ruft dasselbe Ziel auf wie **Plattform** (z. B. in **[!UICONTROL Platform-]**) und in der Spalte **Bearbeitbare Plattformeinstellungen** unten). Die beiden Begriffe beziehen sich auf dasselbe.

Sie müssen die Felder Ihres Kanals nicht vorab nachschlagen. [!DNL Activate] zeigt nur die Spalten an, die für die ausgewählten Kanäle und Formate relevant sind. Verwenden Sie die nachstehende Tabelle als Referenz für das, was pro Kanal bearbeitet werden kann.

**Bearbeitbare Felder nach Kanal**

| Kanal | Unterstützte Formate | Gesperrte Kopie | Bearbeitbare Textfelder | Bearbeitbare Felder für die Plattformeinrichtung |
|---|---|---|---|---|
| Meta | Bild, Video, Karussell | Überschrift, Textkörper | Beschreibung, Call-to-action, Ziel-URL, URL-Parameter, Tracking-ID | Werbekonto, Facebook-Seite, Instagram-Profil, Meta-Kampagne, Meta-Anzeigensatz |
| LinkedIn | Einzelbild, einzelnes Video | Überschrift, Einführungstext | Beschreibung, Call-to-action, Ziel-URL, URL-Parameter, Tracking-ID | Werbekonto, Kampagne, Anzeigensatz |
| Google Campaign Manager 360 | Statische Anzeige, Videoanzeige, HTML5 ZIP-Anzeige | k. A. | Tracking-ID | Inserentin |
| Amazon Ads | Statische Anzeige | k. A. | Tracking-ID | Konto |
| Innovid | Statische Anzeige, HTML5 ZIP-Anzeige | k. A. | Tracking-ID | Account, Creative Library, Concept Name |
| TikTok | In-Feed-Videoanzeigen | Primärer Text | Call-to-action, Ziel-URL, Tracking-ID | Werbekonto, Kampagne, Anzeigengruppe |
| YouTube | Shorts in Google Ads Demand Gen-Kampagnen | Beschreibung | Call-to-action, Geschäftsname, Ziel-URL, URL-Parameter, Tracking-ID | Konto, Kampagne, Anzeigengruppe, Logo |
| ChatGPT | Chat-Karten | Titel, Textkörper | Ziel-URL, Tracking-ID | OpenAI-Anzeigenkonto, OpenAI-Kampagne, OpenAI-Anzeigengruppe |
| The Trade Desk | Statische Anzeige | k. A. | Tracking-ID | Konto, Kampagne |

Eine **Tracking-ID** ist eine eindeutige Beschriftung, die Sie einer Anzeigenzeile zuweisen. Sie werden als Anzeige- oder Kreativname an die Zielplattform übergeben. Verwenden Sie sie also, um diese Anzeige zum Reporting und zur Fehlerbehebung zu identifizieren.

Bearbeiten Sie die Felder inline pro Zeile oder wählen Sie mehrere Zeilen innerhalb derselben Formattabelle aus und klicken Sie auf **[!UICONTROL Details bearbeiten]** auf der Symbolleiste, die angezeigt wird, um diese Felder gleichzeitig in großen Mengen zu bearbeiten. Um die Felder der Plattformeinrichtung für eine Gruppe von Anzeigenformaten zu konfigurieren, klicken Sie auf **[!UICONTROL Plattformeinstellungen verwalten]** und bearbeiten Sie die Felder im daraufhin angezeigten Dialogfeld.

Um schneller zwischen **[!UICONTROL Tracking-ID]**-Feldern zu wechseln, verwenden Sie diese Tastaturbefehle:

* Drücken Sie **Eingabetaste**, um das Bearbeitungsfeld für die ausgewählte **[!UICONTROL Tracking-ID]** zu öffnen.
* Drücken Sie die **Nach** oder **Nach-unten**-Taste, um zum vorherigen oder nächsten Feld **[!UICONTROL Tracking-ID]** in dieser Spalte zu wechseln.
* Drücken Sie **Eingabetaste** erneut, um die Bearbeitung zu speichern.

## Überprüfen und veröffentlichen Sie Ihre Erlebnisse auf ihren Anzeigenkanälen

Bestätigen Sie, dass in jeder Zeile [!UICONTROL Bereit zur Aktivierung] angezeigt wird. [!DNL Activate] kennzeichnet fehlende oder ungültige Felder, inkompatible Aktionsaufrufe und doppelte Tracking-IDs als [!UICONTROL erfordert Aufmerksamkeit]. Wenn jede Zeile fertig ist, klicken Sie auf **[!UICONTROL An Platform senden]** und bestätigen Sie dies im Dialogfeld „Veröffentlichen“.

[!DNL Activate] zeigt den Status jeder Anzeige nahezu in Echtzeit an: Ausstehend, dann Veröffentlicht oder Fehlgeschlagen. Wenn eine Anzeige fehlschlägt, bewegen Sie den Mauszeiger über ihren Status, um den Fehler der Plattform anzuzeigen. Sie können jede fehlgeschlagene Anzeige in der Tabelle auf einmal wiederholen, indem Sie auf **[!UICONTROL Erneut versuchen]** klicken, anstatt jede Anzeige einzeln erneut zu versuchen. Veröffentlichte Zeilen sind von der erneuten Übermittlung ausgeschlossen und enthalten einen Deep-Link zur Anzeige im nativen Anzeigen-Manager der Zielplattform. Ihre abschließende Prüfung vor der Veröffentlichung und das Starten von Anzeigen erfolgt im eigenen Anzeigenmanager des Zielkanals: [!DNL Activate] stellt Anzeigen immer in einem inaktiven Status bereit.

Ihre Aktivierungstabellen werden auf der [!DNL Activate] Landingpage angezeigt.

## Unterstützte Kanäle

Jeder bezahlte Anzeigenkanal verfügt über kanalspezifische Setup-Felder und Voraussetzungen. Wählen Sie den Kanal der gebührenpflichtigen Anzeige für Aktivierungsrichtlinien:

* [Meta](activate-meta-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
* [Amazon-Anzeigen](activate-amazon-ad.md)
* [Innovid](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [ChatGPT](activate-chatgpt-ad.md)
* [The Trade Desk](activate-trade-desk-ad.md)
