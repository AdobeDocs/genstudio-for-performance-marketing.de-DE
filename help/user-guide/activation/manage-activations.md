---
title: Verwalten von Aktivierungen
description: Erfahren Sie, wie Sie aktivierte Erlebnisse mit Adobe GenStudio for Performance Marketing verwalten.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# Verwalten von Aktivierungen

Ihre Aktivierungstabellen werden auf der [!DNL Activate] Landingpage angezeigt. Jede Tabelle listet ihre Anzeigen zusammen mit ihrem Status auf:

| Status | Bedeutung |
|---|---|
| [!UICONTROL Erfordert Aufmerksamkeit] | Mindestens eine Anzeige in der Aktivierungstabelle enthält ein fehlendes oder ungültiges Feld, z. B. eine inkompatible call to action oder eine doppelte Tracking-ID. |
| [!UICONTROL Bereit zum Aktivieren] | Alle Anzeigen in der Aktivierungstabelle bestehen die Validierung und sind zur Veröffentlichung bereit. |
| [!UICONTROL Ausstehend] | Die gesamte Aktivierungstabelle wurde übermittelt und wird von der Zielplattform verarbeitet. |
| [!UICONTROL Veröffentlicht] | Die gesamte Aktivierungstabelle wurde veröffentlicht. |
| [!UICONTROL fehlgeschlagen] | Die Zielplattform hat mindestens eine der Anzeigen in der Tabelle abgelehnt. Bewegen Sie den Mauszeiger über die Status-QuickInfo, um die Fehlermeldung der Plattform anzuzeigen. |

Sie können fehlgeschlagene Aktivierungen automatisch wiederholen, indem Sie oben rechts **[!UICONTROL Erneut versuchen]** klicken.

Veröffentlichte Zeilen sind von der erneuten Übermittlung ausgeschlossen und enthalten einen Deep-Link zur Anzeige im nativen Anzeigen-Manager der Zielplattform, sodass Sie direkt zur Anzeige springen können, um sie zu überprüfen oder zu starten.

## Detailansicht

Klicken Sie auf eine Anzeigenzeile, um eine fokussierte Ansicht der Aktivierungsdetails zu öffnen. Die schreibgeschützte Detailansicht erfasst die definierenden Details einer aktivierten Anzeige, einschließlich fehlgeschlagener Aktivierungen, mit Informationen, die sowohl von GenStudio for Performance Marketing als auch der Zielplattform abgeleitet werden:

* **Veröffentlichungszeit und -datum**: Zeit und Datum der Veröffentlichung auf der Zielplattform
* **Anzeigen-ID**: ID, die von der Zielplattform zugewiesen und zum Tracking verwendet wird, mit einem Deep-Link zur veröffentlichten Anzeige im nativen Anzeigen-Manager der Plattform
* **Anzeigendetails**: Die für die Anzeige verwendeten genehmigten Assets, Kopien und Metadaten
* **Platform-Setup**: Die Felder für das Konto, die Kampagne und andere Plattformeinstellungen, die zum Aktivieren der Anzeige verwendet werden

Die Detailansicht einer fehlgeschlagenen Aktivierung enthält den Grund für den Fehler.
