---
title: Aktivieren einer Anzeige beim Trade Desk
description: Erfahren Sie, wie Sie ein statisches Display und Erlebnis für The Trade Desk aktivieren.
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%
---
# Aktivieren einer Anzeige für das Trade Desk

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von Anzeigen-Erlebnissen im Trade Desk.

**Unterstützte Formate**: Statische Anzeige (nur ein Asset).

Die Aktivierung einer Anzeige für The Trade Desk folgt den [gleichen allgemeinen Schritten](create-activation.md) die für die Aktivierung für andere Paid-Ad-Kanäle erforderlich sind, mit einem Unterschied. Der Trade Desk ist ein verwalteter Unternehmensservice und keine Self-Service-Anzeigenplattform, sodass der Kontozugriff anders funktioniert als für andere Kanäle. Auf dieser Seite werden diese Unterschiede zusammen mit den Voraussetzungen und Setup-Feldern für The Trade Desk behandelt.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

* Ein bestehendes Live-Trade-Desk-Konto. Richten Sie dies direkt beim Trade Desk ein, bevor Sie es mit GenStudio for Performance Marketing verbinden.
* API-Zugriff durch Ihr The Trade Desk-Konto-Team aktiviert. Bei The Trade Desk ermöglicht Ihr Konto-Team diesen Zugriff in Ihrem Namen mithilfe eines API-Tokens und nicht mithilfe der OAuth-Anmeldung, die von anderen Paid-Ad-Kanälen verwendet wird.
* Der richtige Advertiser, der richtige Platz und die richtigen Berechtigungen, die vom Trade Desk für die GenStudio for Performance Marketing-Integration aktiviert wurden.
* Ein API-Token oder Anmeldedaten von Ihrem The Trade Desk-Konto-Team mit Berechtigungen zum Veröffentlichen von Kreativen im Ziel-Advertiser-Konto.
* Eine Zielkampagne, die bereits im Trade Desk vorhanden ist. GenStudio for Performance Marketing aktiviert Anzeigen für diese bestehende Kampagne.

## Verbinden Ihres The Trade Desk-Kontos

Bevor Ihr Unternehmen Erlebnisse aktivieren kann, wenden Sie sich an Ihr Trade Desk-Accountteam, um den API-Zugriff zu aktivieren. Anschließend verbindet ein GenStudio-Systemmanager das Account mit GenStudio for Performance Marketing:

1. Wenden Sie sich an Ihr Trade Desk-Accountteam und fordern Sie Zugriff auf die Veröffentlichung von Kreativen aus GenStudio for Performance Marketing in Ihrem The Trade Desk-Account an. Bestätigen Sie, welche Advertiser-ID, welcher Sitz oder welche Partnerdetails für die Aktivierung verwendet werden sollen.
1. Beschaffen Sie sich das API-Token oder die Anmeldeinformationen von Ihrem The Trade Desk-Konto-Team und bestätigen Sie, dass das Token kreative Veröffentlichungsberechtigungen für das Ziel-Advertiser-Konto unterstützt.
1. Navigieren Sie in GenStudio for Performance Marketing zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Kanäle]** und klicken Sie dann auf **[!UICONTROL Verbinden]** auf der Kachel **[!UICONTROL The Trade Desk]**. Geben Sie den Kontonamen, die Advertiser-ID und das API-Token oder die Anmeldedaten ein und speichern Sie dann die Verbindung.

Wenn die Verbindung fehlschlägt, bestätigen Sie mit Ihrem The Trade Desk-Konto-Team, dass der API-Zugriff aktiviert wurde und das Token über die richtigen Advertiser- und Sitzberechtigungen verfügt.

## Die Trade Desk-Setup-Felder

Genehmigte Assets sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Tracking-ID (wird als Kreativname der Plattform verwendet)
* **Felder für die Plattformeinrichtung**: Konto, Kampagne

Derzeit unterstützt die Aktivierung von The Trade Desk nur statische Anzeigen für einzelne Assets.
