---
title: Überblick über „Aktivieren“
description: Erfahren Sie, wie Sie Inhalte mit Adobe CX Enterprise und Anwendungen von Drittanbietern aktivieren können.
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
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
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: ht
source-wordcount: '413'
ht-degree: 100%
---
# „Aktivieren“ in Adobe GenStudio for Performance Marketing

In GenStudio for Performance Marketing [!DNL Activate] bereiten Sie Anzeigenerlebnisse vor und senden sie an gebührenpflichtige Anzeigenkanäle wie Meta oder LinkedIn. Bei der _Aktivierung_ wird das für einen bestimmten Kanal erforderliche Setup auf ein genehmigtes Anzeigenerlebnis und seine Assets angewendet und dann direkt in einem inaktiven, ausgeschalteten Status auf diesem Kanal bereitgestellt. Danach ist eine abschließende Überprüfung im eigenen Anzeigen-Manager des Kanals möglich, bevor die Anzeige live geschaltet wird.

[!DNL Activate] stellt das Erlebnis direkt auf dem Kanal bereit, sodass Sie keine Dateien exportieren oder sie manuell in den eigenen Anzeigen-Manager des Kanals hochladen müssen.

Eine GenStudio-System-Managerin oder -Editorin bzw. ein GenStudio-System-Manager oder -Editor muss das Anzeigenkonto für jeden gebührenpflichtigen Anzeigenkanal verbinden, bevor Sie ein Anzeigenerlebnis für diesen Kanal aktivieren können.

## Aktivieren von Funktionen

Verwenden Sie [!DNL Activate], um Anzeigenerlebnisse für ihre entsprechenden gebührenpflichtigen Anzeigenkanäle vorzubereiten. Sie können eine [Massenaktivierung von Erlebnissen](create-activation.md) auf mehreren gebührenpflichtigen Anzeigenkanälen in einer einzigen Aktivierungstabelle vornehmen. Danach [verwalten Sie Aktivierungen](manage-activations.md), um den Status und die Details jedes aktivierten Erlebnisses anzuzeigen.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### Aktivieren genehmigter Erlebnisse aus „Content“

Wählen Sie ein oder mehrere genehmigte, veröffentlichte Erlebnisse aus [!DNL Content] aus oder beginnen Sie auf der Landingpage von [!DNL Activate]. Im Gegensatz zu früheren Versionen von [!DNL Activate] kann eine einzelne Aktivierungstabelle Erlebnisse für mehrere gebührenpflichtige Anzeigenkanäle gleichzeitig enthalten, die nach Anzeigenformat und Kanal organisiert sind.

>[!NOTE]
>
>[!DNL Content] bezeichnet ein Ziel wie Meta oder LinkedIn als **Kanal**. [!DNL Activate] bezeichnet dasselbe Ziel als **Plattform** (z. B. in **[!UICONTROL Platform-Setup]**). Beide Begriffe beziehen sich auf dasselbe.

### Konfigurieren von Anzeigen- und Platform-Setup-Details

Jede Zeile in der Aktivierungstabelle stellt eine Anzeige dar. Genehmigte Kreativ-Assets, Überschriften und Textkörper sind gesperrt, da sie bereits überprüft und genehmigt wurden. Sie können die verbleibenden Felder bearbeiten, z. B. den Text des Aktionsaufrufs, die Ziel-URL und die Plattform-Setup-Details wie das Anzeigenkonto, die Kampagne und den Anzeigensatz. Bearbeiten Sie Felder jeweils nur für eine Zeile oder wählen Sie mehrere Zeilen aus, um eine Massenbearbeitung freigegebener Felder durchzuführen.

### Überprüfung der Erlebnisse und Veröffentlichung auf den Anzeigenkanälen

Bestätigen Sie, dass in jeder Zeile der Status [!UICONTROL Bereit zum Aktivieren] angezeigt wird. [!DNL Activate] kennzeichnet fehlende oder ungültige Felder, inkompatible Aktionsaufrufe und doppelte Tracking-IDs mit dem Status [!UICONTROL Erfordert Aufmerksamkeit]. Wenn alle Zeilen bereit sind, klicken Sie auf **[!UICONTROL An Platform senden]**, um alle Anzeigen in der Tabelle zu veröffentlichen. [!DNL Activate] meldet den Status jeder Anzeige nahezu in Echtzeit. Erfolgreich veröffentlichte Anzeigen enthalten einen Deep-Link zur Anzeige im nativen Anzeigen-Manager der Zielplattform. Bei fehlgeschlagenen Anzeigen wird eine Fehlermeldung ausgegeben und es ist ein erneuter Versuch möglich.
