---
title: Amazon Ads aktivieren
description: Erfahren Sie, wie Sie Amazon Ads-Erlebnisse aktivieren.
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# Amazon Ads aktivieren

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von Anzeigen-Erlebnissen in Amazon Ads.

**Unterstützte**: Statische Anzeige.

Die Aktivierung eines Amazon Ads-Erlebnisses folgt [denselben allgemeinen Schritten](create-activation.md) die für die Aktivierung auf anderen Paid-Ad-Kanälen erforderlich sind. Auf dieser Seite werden Amazon Ads-spezifische Voraussetzungen und Setup-Felder behandelt. Nachdem Sie ein Erlebnis in GenStudio for Performance Marketing aktiviert haben, überprüfen Sie das Erlebnis mit Amazon Ads und starten Sie die Anzeige.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

* Zugriff auf das Amazon Ads-Zielkonto.
* Administratorzugriff auf dieses Konto, um in Amazon Ads zu lesen und zu schreiben.

Amazon Ads organisiert Kampagnen und Anzeigen in verschiedenen Konten und jedes Konto enthält eine Kreativbibliothek. Das Zielkonto muss bereits in Amazon Ads vorhanden sein. GenStudio for Performance Marketing veröffentlicht Anzeigenerlebnisse in der Kreativbibliothek dieses Kontos, erstellt jedoch keine Konten.

## Verbinden Ihres Amazon Ads-Kontos

Bevor Ihr Unternehmen Assets in einer Kreativbibliothek veröffentlichen kann, muss ein GenStudio-System-Manager Ihr Amazon Ads-Konto mit GenStudio for Performance Marketing verbinden. Sie müssen Administratorzugriff auf dieses Konto haben, um aus Amazon Ads lesen und darauf schreiben zu können. Siehe [Verbinden bezahlter Medienkonten](/help/user-guide/connectors/connect-channel.md).

Nach Abschluss der Synchronisierung können Sie die hinzugefügten Konten anzeigen.

## Amazon Ads-Setup-Felder

Genehmigte Assets sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Tracking-ID (wird als Kreativname der Plattform verwendet)
* **Felder für die Plattformeinrichtung**: Konto

Ihr Kreativerlebnis wird nach Abschluss der Aktivierung in Amazon Ads der Kreativbibliothek des ausgewählten Kontos bereitgestellt.
