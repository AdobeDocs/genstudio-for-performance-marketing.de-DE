---
title: Aktivieren einer Meta-Anzeige
description: Erfahren Sie, wie Sie ein Meta Ad-Erlebnis aktivieren.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# Aktivieren einer Meta-Anzeige

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von Meta-Anzeigen-Erlebnissen auf Instagram und Facebook.

**Unterstützte**: Bild, Video, Karussell.

[Erstellen eines Meta-Erlebnisses](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing, und wählen Sie es dann zur Aktivierung aus.

Die Aktivierung einer Meta-Anzeige erfolgt in [&#x200B; gleichen allgemeinen Schritten](create-activation.md) die für die Aktivierung auf anderen Paid-Ad-Kanälen erforderlich sind. Auf dieser Seite werden Meta-spezifische Voraussetzungen und Setup-Felder behandelt. Nachdem Sie ein Meta-Erlebnis in GenStudio for Performance Marketing aktiviert haben, verwenden Sie [Meta Ads Manager](https://adsmanager.facebook.com/), um das Erlebnis zu überprüfen und die Anzeige zu starten.

Im Gegensatz zu anderen Kanälen kann eine Meta-Anzeige mehrere Seitenverhältnisse in einer Anzeige enthalten. Wenn Ihr Erlebnis mehrere Seitenverhältnisse hat, generiert [!DNL Activate] dennoch nur eine Zeile dafür, nicht eine Zeile pro Seitenverhältnis.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

Vergewissern Sie sich, dass Ihre verbundenen Meta-Werbekonten über die vollständige Berechtigung zum Verwalten von Anzeigen in diesen Komponenten der Meta-Werbeplattform verfügen:

* Meta-Werbekonto
* Facebook-Seite
* Meta Campaign
* Meta-Anzeigensatz
* Instagram-Profil (optional)

Die Meta-Zielkampagne und der Anzeigensatz müssen bereits in Meta Ads Manager vorhanden sein. GenStudio for Performance Marketing erstellt derzeit keine Kampagnen oder Anzeigengruppen.

## Meta-Konten verbinden

Bevor Ihr Unternehmen Erlebnisse aktivieren kann, muss ein GenStudio-Systemmanager Ihre Meta-Konten mit GenStudio for Performance Marketing verbinden. Diese Verbindung ermöglicht den Datenfluss zwischen GenStudio for Performance Marketing und Meta und ermöglicht so den Aktivierungsprozess. Siehe [Verbindung zu Meta Ads herstellen](/help/user-guide/connectors/meta-ads.md).

Um ein Instagram-Konto auszuwählen, stellen Sie in Meta Business Manager sicher, dass [das Instagram-Konto, das Sie verwenden möchten, mit demselben Werbekonto verbunden ist](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account) das beim Onboarding ausgewählt wurde. Wenn diese Verbindung fehlt, wird das Instagram-Konto während der Aktivierung möglicherweise nicht **[!UICONTROL Dropdown]** Menü „Instagram-Profil“ angezeigt.

Nach Abschluss der Synchronisierung können Sie die hinzugefügten Konten anzeigen. Die Synchronisierung großer Datenmengen dauert länger.

## Meta-Setup-Felder

Genehmigte Assets, Überschriften und Textkörper sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Beschreibung, Call-to-action, Ziel-URL, URL-Parameter, Tracking-ID (als Name der Meta-Anzeige verwendet)
* **Felder für die Plattformeinrichtung**: Werbekonto, Facebook-Seite, Instagram-Profil, Meta-Kampagne, Meta-Anzeigensatz
