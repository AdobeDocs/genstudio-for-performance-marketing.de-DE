---
title: Aktivieren einer ChatGPT-Anzeige
description: Erfahren Sie, wie Sie ein ChatGPT-Anzeigen-Erlebnis aktivieren.
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
source-wordcount: '272'
ht-degree: 0%
---
# Aktivieren einer ChatGPT-Anzeige

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von ChatGPT-Anzeigen-Erlebnissen.

**Unterstützte Formate**: Chat-Karten.

Sie können [ein ChatGPT-Erlebnis &#x200B;](/help/user-guide/create/create-chatgpt-ad.md) GenStudio for Performance Marketing erstellen und es dann zur Aktivierung auswählen.

Die Aktivierung einer ChatGPT-Anzeige folgt [denselben allgemeinen Schritten](create-activation.md) die für die Aktivierung auf anderen Paid-Ad-Kanälen erforderlich sind. Auf dieser Seite werden die ChatGPT-spezifischen Voraussetzungen und Setup-Felder behandelt. Nachdem Sie ein ChatGPT-Erlebnis in GenStudio for Performance Marketing aktiviert haben, führen Sie mit OpenAI Ads Manager abschließende Prüfungen durch und starten Sie die Anzeige.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

* Ein OpenAI Ads-Konto und ein API-Schlüssel aus diesem Konto.
* Die Ziel-ChatGPT-Kampagne und -Anzeigengruppe muss bereits in OpenAI Ads Manager vorhanden sein. GenStudio for Performance Marketing erstellt keine neuen Kampagnen oder Anzeigengruppen.

## Verbinden Ihres ChatGPT-Kontos

Bevor Ihr Unternehmen Erlebnisse aktivieren kann, muss ein GenStudio-Systemmanager Ihr OpenAI Ads-Konto mit GenStudio for Performance Marketing verbinden:

1. Navigieren Sie in OpenAI Ads Manager zu **[!UICONTROL Einstellungen]** > **[!UICONTROL API-Schlüssel]** > **[!UICONTROL Neuen Schlüssel erstellen]**.
1. Gehen Sie in GenStudio for Performance Marketing zu **[!UICONTROL Mehr]** > **[!UICONTROL Einstellungen]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Verbinden]** > **[!UICONTROL Konto hinzufügen]**.
1. Geben Sie den Namen Ihres OpenAI Ads-Kontos ein, fügen Sie Ihren API-Schlüssel ein und klicken Sie dann auf **[!UICONTROL Konto hinzufügen]**.

## ChatGPT-Setup-Felder

Genehmigte Assets, Überschriften (Titel) und Textkörper sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Ziel-URL, Tracking-ID (wird als Anzeigename der Plattform verwendet)
* **Felder für die Platform**: OpenAI Ads-Konto, OpenAI-Kampagne, OpenAI-Anzeigengruppe

Die Ziel-URL muss ein gültiges `https://`-Format verwenden, z. B. `https://www.example.com`.
