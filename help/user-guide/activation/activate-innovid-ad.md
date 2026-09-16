---
title: Aktivieren einer Innovid-Anzeige
description: Erfahren Sie, wie Sie ein Innovid-Erlebnis aktivieren.
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# Aktivieren einer Innovid-Anzeige

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von Anzeigen-Erlebnissen für Innovid.

**Unterstützte Formate**: Statische Anzeige, HTML5 Zip-Anzeige.

Die Aktivierung eines Innovid-Erlebnisses folgt den [gleichen allgemeinen Schritten](create-activation.md) die für die Aktivierung auf anderen Paid-Ad-Kanälen erforderlich sind. Auf dieser Seite werden Innovid-spezifische Voraussetzungen und Setup-Felder behandelt. Nachdem Sie ein Erlebnis in GenStudio for Performance Marketing aktiviert haben, überprüfen Sie das Erlebnis mit Innovid und starten Sie die Anzeige.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

* Zugriff auf das Innovid-Zielkonto.
* Administratorzugriff auf dieses Konto, um aus Innovid zu lesen und darauf zu schreiben.

Innovid organisiert Kampagnen und Anzeigen in verschiedenen Accounts, und jedes Account verfügt über eine Kreativbibliothek. Die Ziel-Kreativbibliothek muss bereits in Innovid vorhanden sein. GenStudio for Performance Marketing veröffentlicht Anzeigen-Erlebnisse in dieser Kreativbibliothek, erstellt jedoch keine Konten oder Kreativbibliotheken.

## Verbinden Ihres Innovid-Kontos

Bevor Ihr Unternehmen Assets in einer Kreativbibliothek veröffentlichen kann, muss ein GenStudio-Systemmanager Ihr Innovid-Konto mit GenStudio for Performance Marketing verbinden. Sie müssen Administratorzugriff auf dieses Konto haben, um aus Innovid lesen und schreiben zu können. Siehe [Verbinden bezahlter Medienkonten](/help/user-guide/connectors/connect-channel.md).

Nach Abschluss der Synchronisierung können Sie die hinzugefügten Konten anzeigen.

## Ungültige Setup-Felder

Genehmigte Assets sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Tracking-ID (wird als Kreativname der Plattform verwendet)
* **Felder für die Platform**-Einrichtung: Konto, Creative-Bibliothek, Konzeptname

Nach Abschluss der Aktivierung wird Ihr Kreativerlebnis in der ausgewählten Kreativbibliothek in Innovid bereitgestellt.
