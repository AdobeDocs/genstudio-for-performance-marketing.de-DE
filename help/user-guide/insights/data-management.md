---
title: Daten-Management
description: Erfahren Sie mehr über Datenaufnahme und -speicherung für [!DNL Insights] in GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: 'https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y'
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
    internal-label: Integrations
  - id: c5a86ad9-9158-4ab1-a7ea-9e29985087b8
    internal-label: Content lifecycle
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e61505eb-ae0c-4fa0-a6cc-9f95313d4431
    internal-label: Reporting and insights
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
source-git-commit: 4d35c796d2968255c3e1f525215cfe71434f8e23
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 2%
---
# Daten-Management

GenStudio for Performance Marketing verwendet Adobe Experience Platform (AEP) für die Datenaufnahme und Speicherung der Metriken und Metadaten, die [!DNL Insights] unterstützen. AEP verwendet _Schemata_ zum Definieren der Datenstrukturen und _Datensätze_ zum Speichern und Verwalten von Datenerfassungen.

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
- AEP Connections: Datenflüsse mit dem Präfix `GS Insights`
- AEP Connections: GS Insights-Konto

Siehe [Auswirkungen löschen](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) im Handbuch _Customer Journey Analytics_, bevor Sie Datenkomponenten in AEP löschen.

>[!ENDSHADEBOX]

## Richtlinie zur Datenaufbewahrung

GenStudio for Performance Marketing bewahrt Kanaldaten 13 Monate lang auf. Diese Aufbewahrungsrichtlinie umfasst die 6 Monate an Daten, die während der ersten Verbindung aufgenommen wurden, um eine umfassende historische Datenanalyse und Berichterstellung sicherzustellen.

Siehe [Verbinden eines Paid-Media-Kontos](/help/user-guide/connectors/connect-channel.md).
