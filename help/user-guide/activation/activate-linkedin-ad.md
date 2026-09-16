---
title: Aktivieren einer LinkedIn-Anzeige
description: Erfahren Sie, wie Sie ein LinkedIn-Anzeigen-Erlebnis aktivieren.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# LinkedIn-Anzeige aktivieren

Adobe GenStudio for Performance Marketing unterstützt die Aktivierung von LinkedIn-Anzeigen-Erlebnissen für [LinkedIn-Kampagnenmanager](https://business.linkedin.com/marketing-solutions).

**Unterstützte Formate**: Einzelbild, Einzelvideo.

Sie können [ein LinkedIn-Erlebnis &#x200B;](/help/user-guide/create/create-linkedin.md) GenStudio for Performance Marketing erstellen und es dann zur Aktivierung auswählen.

Die Aktivierung einer LinkedIn-Anzeige erfolgt [&#x200B; den gleichen allgemeinen Schritten](create-activation.md) die für die Aktivierung auf anderen Paid-Ad-Kanälen erforderlich sind. Auf dieser Seite werden die LinkedIn-spezifischen Voraussetzungen und Setup-Felder behandelt. Nachdem Sie ein LinkedIn-Erlebnis in GenStudio for Performance Marketing aktiviert haben, können Sie mit LinkedIn Campaign Manager das Erlebnis überprüfen und die Anzeige starten.

GenStudio-Systemmanager und -Bearbeiter können Anzeigen-Erlebnisse aktivieren.

## Voraussetzungen

* Ein LinkedIn-Kampagnen-Manager-Konto mit voller Berechtigung zum Verwalten von Kampagnen und Anzeigen. Dieses Konto muss vorhandene Kampagnen enthalten.
* LinkedIn-Werbekonten mit vollständiger Berechtigung zum Erstellen von Anzeigen und Posten von Inhalten auf LinkedIn-Seiten.

Die Ziel-LinkedIn-Kampagne und der Anzeigensatz müssen bereits im LinkedIn-Kampagnen-Manager vorhanden sein. GenStudio for Performance Marketing erstellt keine Kampagnen oder Anzeigengruppen.

>[!NOTE]
>
>LinkedIn hat seine Kampagnenhierarchie umbenannt: Was LinkedIn Campaign Manager zuvor **Kampagnengruppe** genannt hat, wird jetzt **Kampagne** und was es zuvor **Kampagne** genannt hat, wird jetzt **Anzeigensatz**. Die **[!UICONTROL LinkedIn-Kampagne]** und **[!UICONTROL LinkedIn-]** in [!DNL Activate] verwenden diese aktuelle Terminologie.

GenStudio for Performance Marketing unterstützt derzeit LinkedIn-Anzeigen mit Einzelbildern und Einzelvideos, die jeweils nur ein Bild oder Video pro Beitrag enthalten. Wenn Ihr Erlebnis mehrere Seitenverhältnisse aufweist, generiert [!DNL Activate] in der Aktivierungstabelle eine separate Zeile pro Verhältnis, sodass jede Zeile als eigene Anzeige ausgeführt werden kann. Löschen Sie alle Zeilen, die Sie nicht benötigen.

## Verknüpfen von LinkedIn-Konten

Bevor Ihr Unternehmen Erlebnisse aktivieren kann, muss ein GenStudio-Systemmanager oder -Editor Ihre LinkedIn-Werbekonten mit GenStudio for Performance Marketing verbinden. Sie müssen über vollständigen Administratorzugriff sowohl auf das Werbekonto als auch auf die LinkedIn-Profilseite verfügen, um eine erfolgreiche Verbindung herstellen zu können. Sie müssen nur einmal ein Werbekonto in **[!UICONTROL Einstellungen]** verbinden. Danach ist sie für jeden verfügbar, der auf diese Instanz zugreifen kann.

Diese Verbindung ermöglicht den Datenfluss zwischen GenStudio for Performance Marketing und LinkedIn und ermöglicht so den Aktivierungsprozess.

Nach Abschluss der Synchronisierung können Sie die hinzugefügten Konten anzeigen. Die Synchronisierung großer Datenmengen dauert länger.

## Setup-Felder für LinkedIn

Genehmigte Assets, Überschriften und Einführungstext sind gesperrt und können während der Aktivierung nicht bearbeitet werden, da sie bereits in [!DNL Content] überprüft und genehmigt wurden. Sie können Folgendes bearbeiten:

* **Textfelder**: Beschreibung, Call-to-action, Ziel-URL, URL-Parameter, Tracking-ID (wird als Anzeigename der Plattform verwendet)
* **Felder für die Plattformeinrichtung**: LinkedIn-Werbekonto, LinkedIn-Kampagne, LinkedIn-Anzeigensatz
