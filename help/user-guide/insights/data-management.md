---
title: Daten-Management
description: Erfahren Sie mehr über Datenaufnahme und -speicherung für Einblicke in GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Daten-Management

GenStudio for Performance Marketing verwendet Adobe Experience Platform (AEP) für die Datenaufnahme und Speicherung der Metriken und Metadaten, die [!DNL Insights] unterstützen. AEP verwendet _Schemata_, um die Datenstrukturen und _Datensätze_ zum Speichern und Verwalten von Datenerfassungen zu definieren.

## Datenverbindungen

GenStudio for Performance Marketing verwendet Customer Journey Analytics (CJA), um mehrere Datenquellen zu aggregieren, indem eine Verbindung zu einem oder mehreren AEP-Datensätzen hergestellt wird. CJA verwendet diese Datenverbindungen, um Datenansichten zur Analyse von Metriken mit [!DNL Insights] zu erstellen.

>[!BEGINSHADEBOX]

**Wichtige Informationen zu Datenverbindungen**

Wenn Sie [Adobe-Systemadministrator](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) sind, verfügen Sie möglicherweise über Berechtigungen, die den Zugriff auf AEP-Sandbox-Verwaltungs- und Data-Lake-Komponenten ermöglichen, die GenStudio for Performance Marketing unterstützen.

>[!WARNING]
>
>Wenn Sie die Produktions-Sandbox in AEP zurücksetzen, werden alle Datenverbindungen gelöscht und [!DNL Insights] nicht mehr funktionieren.

Seien Sie vorsichtig und löschen Sie nicht die folgenden Datenverbindungen, die für einen zuverlässigen Betrieb von GenStudio for Performance Marketing erforderlich sind:

- AEP-Datensätze mit dem Präfix `GS Insights`
- AEP-Schemata, -Klassen und -Feldergruppen mit dem Präfix `GS Insights`
- `timestamp for metadata` der benutzerdefinierten Feldergruppe
- AEP-Verbindungen: Datenflüsse mit dem Präfix `GS Insights`
- AEP-Verbindungen: GS Insights-Konto

Siehe [Auswirkungen löschen](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) im Handbuch _Customer Journey Analytics_, bevor Sie Datenkomponenten in AEP löschen.

>[!ENDSHADEBOX]

## Richtlinie zur Datenaufbewahrung

GenStudio for Performance Marketing bewahrt Kanaldaten 13 Monate lang auf. Diese Aufbewahrungsrichtlinie umfasst die 6 Monate an Daten, die während der ersten Verbindung aufgenommen wurden, um eine umfassende historische Datenanalyse und Berichterstellung sicherzustellen.

Siehe [Verbinden eines Kanal-Werbekontos](/help/user-guide/insights/connect-channel.md).
