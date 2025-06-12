---
title: Adobe GenStudio for Performance Marketing-Kampagnen
description: Erfahren Sie, wie Sie digitale Marketing-Kampagnen erstellen und verwalten, die Assets und Erlebnisse mit generativer KI nutzen.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Diese Funktion befindet sich derzeit in Beta, sodass einige Funktionen möglicherweise eingeschränkt sind oder geändert werden können."
exl-id: b7c4194f-fa61-4739-acd6-7acbdd98e9b2
source-git-commit: 5279caaf4651ed81c3cf3d8a4de2f17c3f151ec8
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Erstellen einer Kampagne

Eine GenStudio for Performance Marketing-Kampagne definiert wichtige Eigenschaften digitaler Kampagnen und entwickelt sich entsprechend der Bereitstellung und Bewertung der Stadien. GenStudio for Performance Marketing unterstützt den dynamischen Prozess des Kampagnenstarts, der Leistungsnachverfolgung einzelner Kampagnenkomponenten und der Neuausrichtung von Anzeigenerlebnissen auf der Grundlage von Leistungsmetriken.

Die Schlüsselelemente Ihrer Kampagne werden in einem Kampagnenobjekt gespeichert, wodurch ein gemeinsamer Kontext für alle Assets und Erlebnisse erstellt wird, die mit demselben eindeutigen Kampagnennamen gekennzeichnet sind. Dieser Titel identifiziert die Kampagne in GenStudio for Performance Marketing.

GenStudio-Systemmanager und GenStudio-Bearbeiter können Kampagnen erstellen.

## Definieren von Kampagnendetails

{{$include /help/_includes/campaign-details.md}}

**Kampagnendetails eingeben**:

1. Klicken Sie in [!DNL Campaigns] auf **[!UICONTROL Kampagne hinzufügen]**. Die _„Kampagne erstellen_ wird geöffnet.

   Details umfassen sowohl optionale als auch obligatorische Felder, die Ihre Kampagne definieren. Diese Details werden in [!DNL Campaigns] als Metadatenattribute der Kampagne gespeichert.

1. Doppelklicken Sie auf die Kopfzeile _Neue Kampagne_ und geben Sie einen aussagekräftigen, eindeutigen Namen ein.

   GenStudio for Performance Marketing Dieser Name wird in _zu einer_-Bezeichnung, mit der Sie Assets oder Erlebnisse während des Hochladens und der Erstellung mit der Kampagne verknüpfen können.

1. Geben Sie Werte in die Felder _Details_ ein, die Ihre Kampagne beschreiben. Definitionen _Kampagnenfunktionen finden Sie in der_ Kampagnendetails“.

## Zuweisen von Kanälen und Regionen

Die Kanal- und Regionseinstellungen bestimmen, wo die Kampagne bereitgestellt wird, sowie ihre Verteilungskanäle.

GenStudio for Performance Marketing verwendet vordefinierte Vorlagen _Datensätze_ zur Darstellung der wichtigsten Kampagnenkomponenten, z. B. Kanäle, Regionen, Rollen und Produkte. Beim Erstellen einer Kampagne verknüpfen Sie diese mit den entsprechenden Datensätzen für jede dieser Komponenten.

* **Kanaleinstellungen** Definiert die öffentlichen Verteilungskanäle für Ihre Kampagne, einschließlich Paid-Media-Konten, E-Mail-Marketing-Services und Display-Anzeigennetzwerke. Daten zur Leistung von Kampagnen, Assets und Erlebnissen in diesen Kanälen werden zur kanalspezifischen Analyse in [[!DNL Insights]](/help/user-guide/insights/overview.md) eingespeist.

* **Regionseinstellungen** - Gibt die geografischen Bereiche an, in denen Sie Ihre Kampagne bereitstellen. Durch die Verbindung mit regionalen Datenquellen kann GenStudio for Performance Marketing Inhalte und Strategien an die Präferenzen der lokalen Zielgruppe anpassen. Dies ermöglicht eine genauere Zielgruppenbestimmung und Leistungsanalyse auf der Grundlage regionaler Metriken.

**So wählen Sie Vertriebskanäle für Ihre Kampagne aus**:

1. Klicken Sie auf das Pluszeichen (**[!UICONTROL Datensätze verbinden +]**) neben **[!UICONTROL Kanäle]**.

   Das _Kanäle auswählen_ Popup wird geöffnet.

1. Auswählen der Kanäle, auf denen die Kampagne bereitgestellt wird. Gültige Werte sind `Email`, `Paid media`, `Web` und `Display ads`.

   Wählen Sie optional **[!UICONTROL Alle anzeigen]**, um eine Ansicht aller unterstützten Kanäle zu öffnen.

**So weisen Sie Ihrer Kampagne Regionen zu**:

1. Klicken Sie auf das Pluszeichen (**[!UICONTROL Datensätze verbinden +]**) neben **[!UICONTROL Regionen]**.

   Das _Regionen auswählen_ Popup wird geöffnet. Sie können nach einer bestimmten unterstützten Region suchen.

1. Wählen Sie die Regionen aus, eine oder mehrere Zielregionen für Ihre Kampagne. Gültige Regionen sind `AMER`, `LATAM`, `EMEA`, `APAC` und `Japan`.

   Wählen Sie optional **[!UICONTROL Alle anzeigen]**, um eine Ansicht aller unterstützten Bereiche zu öffnen.

## Zuweisen von Personas und Produkten

[Personas](/help/user-guide/guidelines/personas.md) und [products](/help/user-guide/guidelines/products.md) werden als Datensätze gespeichert. Ein Personendatensatz definiert die Merkmale eines bestimmten Kundensegments (Ihrer Zielgruppe für generierte Inhalte). Dies kann demografische Details und einen Verlauf der Kundeninteraktionen umfassen.

Produktdatensätze definieren wichtige Produktspezifikationen und -attribute im Kontext Ihrer Markenrichtlinien. Zu den Attributen können Funktionen, zugehörige Bilder und die Produktpositionierung innerhalb Ihrer Marke gehören.

Die Optionen in den _Personas_ und _Products_ Dropdown-Menüs werden auf Organisationsebene definiert. Bei der Erstellung einer Kampagne wählen Sie aus diesen vordefinierten Datensätzen aus, um eine konsistente Produktdarstellung zu gewährleisten und eine genaue Zielgruppenbestimmung, Messaging und Leistungsverfolgung zu unterstützen.

**So weisen Sie Ihrer Kampagne Personas zu**:

1. Klicken Sie auf das Pluszeichen (**[!UICONTROL Datensätze verbinden +]**) neben **[!UICONTROL Personas]**.

   Das _Rollen auswählen_ Popup wird geöffnet. Sie können nach bestimmten unterstützten Personas suchen.

1. Wählen Sie die Personas aus, auf die Ihre Kampagne abzielt. Gültige Personas werden von Ihrer Organisation während der Erstellung [ Richtlinien ](/help/user-guide/guidelines/personas.md).

   Wählen Sie optional **[!UICONTROL Alle anzeigen]**, um eine Ansicht aller verfügbaren Personas zu öffnen.

**So weisen Sie Ihrer Kampagne Produkte zu**:

1. Klicken Sie auf das Pluszeichen (**[!UICONTROL Datensätze verbinden +]**) neben **[!UICONTROL Produkte]**.

   Das _Produkte auswählen_ Popup wird geöffnet. Sie können nach einem bestimmten unterstützten Produkt suchen.

1. Ein oder mehrere Produkte auswählen. Produkte werden von Ihrer Organisation während der Erstellung [ Richtlinien ](/help/user-guide/guidelines/products.md).

   Wählen Sie optional **[!UICONTROL Alle anzeigen]**, um eine Ansicht aller verfügbaren Produkte zu öffnen.

## Abschließen der Kampagnenerstellung

Klicken Sie **[!UICONTROL Erstellen]**, um die eingegebenen Werte zu speichern und die Kampagne zu erstellen.

Der neue Kampagnenname ist jetzt als Kampagnentitel in [!DNL Content] und [!DNL Create] verfügbar. Sie können Ihrer Kampagne genehmigte Assets und Erlebnisse über [!DNL Content] hinzufügen oder während der Inhaltserstellung ein Asset und ein Erlebnis zu einer Kampagne zuweisen.

## Hinzufügen von Inhalten zu einer Kampagne

GenStudio for Performance Marketing verknüpft Inhalte mithilfe von Kampagnenkennzeichnungen, die in [!DNL Content] Metadaten gespeichert sind, mit Kampagnen. Ein einzelnes Inhaltselement kann mehreren Kampagnen zugeordnet werden.

Kampagnentitel identifizieren die Kampagne und ihre Attribute. Wenn Sie einem Asset oder Erlebnis einen Titel zuweisen, wird das Asset oder Erlebnis mit der entsprechenden Kampagne verbunden.

**Hinzufügen von Assets und Erlebnissen aus[!DNL Content]**:

1. Wählen Sie in der [!DNL Content] _Erlebnisse_ oder _Assets_-Galerie das genehmigte Erlebnis oder Asset aus.

1. Wählen Sie in _Ansicht_ Details“ den Namen der Kampagne aus dem Dropdown-Menü _Kampagnen_ aus.

**Hinzufügen von Assets und Erlebnissen während der Inhaltserstellung**:

Bei der Inhaltserstellung können Sie das neu erstellte Asset oder Erlebnis in [!DNL Content] veröffentlichen.

1. Wählen _im Popup Details für genehmigte Inhalte bestätigen_ eine Kampagne aus dem Dropdown-Menü _Kampagnen_ aus.

1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

Diese Kampagne ist jetzt im Dashboard _Kampagnen_ verfügbar.
