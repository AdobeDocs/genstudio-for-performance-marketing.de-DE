---
title: Daten-Management
description: Erfahren Sie mehr über Datenaufnahme und -speicherung für  [!DNL Insights]  in GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 0%

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

Siehe [Auswirkungen löschen](https://experienceleague.adobe.com/de/docs/analytics-platform/using/technotes/deletion) im Handbuch _Customer Journey Analytics_, bevor Sie Datenkomponenten in AEP löschen.

>[!ENDSHADEBOX]

## Richtlinie zur Datenaufbewahrung

GenStudio for Performance Marketing bewahrt Kanaldaten 13 Monate lang auf. Diese Aufbewahrungsrichtlinie umfasst die 6 Monate an Daten, die während der ersten Verbindung aufgenommen wurden, um eine umfassende historische Datenanalyse und Berichterstellung sicherzustellen.

Siehe [Verbinden von Paid Media-Konten](/help/user-guide/connectors/connect-channel.md).
