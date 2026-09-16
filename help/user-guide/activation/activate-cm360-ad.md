---
title: Aktivieren einer Google Campaign Manager 360-Anzeige
description: Erfahren Sie, wie Sie Google Campaign Manager 360 aktivieren.
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# Aktivieren einer Google Campaign Manager 360-Anzeige

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von Anzeigen-Erlebnissen in Google Campaign Manager 360.

**Unterstützte Formate**: Statische Anzeige, Videoanzeige, HTML5 Zip-Anzeige.

Die Aktivierung einer Google Campaign Manager 360-Anzeige folgt den [gleichen allgemeinen Schritten](create-activation.md) die für die Aktivierung auf anderen Paid-Ad-Kanälen erforderlich sind. Auf dieser Seite werden die Voraussetzungen und Setup-Felder für Google Campaign Manager 360 beschrieben. Nachdem Sie ein Erlebnis in GenStudio for Performance Marketing aktiviert haben, können Sie mit Google Campaign Manager 360 das Erlebnis überprüfen und die Anzeige starten.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

* Ein Google Campaign Manager 360-Konto mit Zugriff auf den Ziel-Advertiser.
* Admin-Zugriff auf den Advertiser, zum Lesen und Schreiben in Campaign Manager 360.

Campaign Manager 360 organisiert Kampagnen und Anzeigen in verschiedenen Advertisern, wobei jeder Advertiser eine Kreativbibliothek enthält. Der Ziel-Advertiser muss bereits in Campaign Manager 360 vorhanden sein. GenStudio for Performance Marketing veröffentlicht Anzeigenerlebnisse in der Kreativbibliothek dieses Advertisers, erstellt jedoch keine Anzeigen.

## Google Campaign Manager 360-Konto verbinden

Bevor Ihr Unternehmen Assets in einer Kreativbibliothek veröffentlichen kann, muss ein GenStudio-Systemmanager oder -Editor Ihr Google Campaign Manager 360-Konto mit GenStudio for Performance Marketing verbinden. Sie müssen Administratorzugriff auf den Advertiser haben, um in Campaign Manager 360 lesen und schreiben zu können. Siehe [Verbinden bezahlter Medienkonten](/help/user-guide/connectors/connect-channel.md).

Nach Abschluss der Synchronisierung können Sie die hinzugefügten Konten anzeigen.

## Google Campaign Manager 360-Setup-Felder

Genehmigte Assets sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Tracking-ID (wird als Kreativname der Plattform verwendet)
* **Felder für die Plattformeinrichtung**: Advertiser

Nach Abschluss der Aktivierung wird Ihr Kreativerlebnis in der Kreativbibliothek des ausgewählten Werbetreibenden in Google Campaign Manager 360 bereitgestellt.
