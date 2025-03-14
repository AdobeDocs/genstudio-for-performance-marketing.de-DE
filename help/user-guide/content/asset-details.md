---
title: Asset-Details
description: Adobe GenStudio for Performance Marketing speichert genehmigte Inhalte mit Rich-Metadaten, um die Suche und die Leistung zu verfolgen.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: f401f93e7dd08db4837b8709e28acec5571052f7
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 1%

---

# Asset-Details

Adobe GenStudio for Performance Marketing speichert genehmigte Inhalte mit Rich-Metadaten für die Auffindbarkeit und das Performance-Tracking.

Jedes Asset (einschließlich Erlebnissen und Vorlagen) verfügt über zugehörige _Details_ (Metadaten), die dabei helfen, die Content-Performance zu identifizieren, zu verfolgen, zu verwenden und aus ihr zu lernen.

**Anzeigen von Asset-Details**:

1. Wählen Sie _[!DNL Content]_ein Asset, ein Erlebnis oder eine Vorlage aus. Durch Klicken auf ein Asset wird eine zielgerichtete Ansicht des Assets geöffnet.

1. Gehen Sie in der Asset-Ansicht zum Abschnitt _[!UICONTROL Details]_ auf der rechten Seite.

1. Wenn der Abschnitt _[!UICONTROL Details]_ nicht sichtbar ist, klicken Sie auf das Symbol **[!UICONTROL Information]** (i).

Asset-Details enthalten Metadaten, die während des Erstellungs- oder Upload-Prozesses angewendet wurden. Asset-Metadatentypen umfassen [Systemmetadaten](#system-metadata) und [benutzerdefinierte Metadaten](#user-defined-metadata).

Das folgende Bild-Asset enthält Systemmetadaten, die den Dateityp, die Größe und andere Eigenschaften beschreiben, ein benutzerdefiniertes Keyword und mehrere von KI erkannte Attribute und Farben.

![Details eines Assets mit mehreren Tags](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets aus AEM-Repositorys zeigt verschiedene Metadaten an. Unter [Asset-Sichtbarkeit konfigurieren](connect-aem-repo.md#step-4-configure-asset-visibility) erfahren Sie, wie Sie [!DNL AEM Assets Content Hub] Asset-Details konfigurieren.

## Systemmetadaten

Einige Asset-Metadaten werden beim Hochladen eines Assets automatisch erfasst, z. B. Dateityp, Größe, Abmessungen, Quelle usw. Mit Ausnahme des Dateinamens können Sie keine standardmäßigen Systemmetadaten bearbeiten.

### Erzeugte Tags

Wenn Sie ein genehmigtes Asset in [!DNL Content] speichern, verwendet GenStudio for Performance Marketing die KI- und maschinellen Lernfunktionen von Adobe, um das Asset zu untersuchen und Tags basierend auf den Asset-Funktionen anzuwenden. Beispielsweise kann ein Bild einer Katze zu Attribut-Tags wie `pet photography` oder `cat` und Farb-Tags führen, die dominante Farben im Bild identifizieren. Sie können Tags, die erkannt und automatisch angewendet werden, nicht bearbeiten.

Siehe [!DNL Insights] [Attributkategorien](/help/user-guide/insights/attributes.md#categories) für detaillierte Listen mit Bild-, Video- und Textfunktionen.

### Erzeugte Inhaltsmetadaten

Die Informationen, die zum Generieren eines neuen Assets oder Erlebnisses verwendet werden, werden zu Metadaten, wie z. B. die Eingabeaufforderung, die verwendet wurde. Sie können die Eingabeaufforderung nach der Genehmigung des Inhalts nicht mehr bearbeiten, sondern sie als Ausgangspunkt für die Erstellung neuer Inhalte verwenden.

## Benutzerdefinierte Metadaten

Benutzerdefinierte Metadaten fügen dem Inhalt des Assets Marketing-Kontext hinzu, sodass Marketing-Fachleute verstehen können, wie das Asset verwendet und mit ihm interagiert wird.

Beim [Hochladen eines Assets](/help/user-guide/content/manage-assets.md#add-assets) können Sie eine Reihe optionaler Asset-Details definieren, die in GenStudio for Performance Marketing als Metadaten vorhanden sind. Das Einschließen weiterer Details kann die Asset-Identifizierung bei Suchen und Filtern verbessern.

**So bearbeiten Sie die benutzerdefinierten Metadaten**:

1. Wählen Sie _[!DNL Content]_ein Asset, ein Erlebnis oder eine Vorlage aus. Durch Klicken auf ein Asset wird eine zielgerichtete Ansicht des Assets geöffnet.

1. Gehen Sie in der Asset-Ansicht zum Abschnitt _[!UICONTROL Details]_ auf der rechten Seite.

1. Klicken Sie **[!UICONTROL Details bearbeiten]** (Bleistift), um Asset-, Erlebnis- oder Vorlagenmetadaten zu bearbeiten.

   Je mehr Details Sie angeben, desto zuverlässiger werden die Funktionen von GenStudio for Performance Marketing. Wählen Sie ein oder mehrere Details aus der Liste aus oder geben Sie gegebenenfalls ein neues ein, z. B. mit Schlüsselwörtern. Jedes hinzugefügte Detail wird unter der Liste angezeigt. Klicken Sie auf **`x`** , um ein Detail zu entfernen.

### Metadatendetails

In der folgenden Tabelle sind die Metadaten (Asset-Details) aufgeführt, die Sie beim Erstellen eines Assets definieren können.

| Feld | Beschreibung |
| -------------- | ----------- |
| Titel | Name des Assets; der Standardtitel kann der ursprüngliche Dateiname sein |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) enthalten Werbeinhalte mit konsistentem Messaging, um ein Geschäftsziel zu erreichen. Durch <br> auf einen Kampagnen-Link gelangen Sie zur Übersichtsseite der Kampagne |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) wurde zu GenStudio for Performance Marketing hinzugefügt und zur Verwendung veröffentlicht |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) zur Verwendung zu GenStudio for Performance Marketing hinzugefügt |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) zur Verwendung zu GenStudio for Performance Marketing hinzugefügt |
| Kanäle | Plattformen für die Verteilung bestimmter Inhaltstypen wie E-Mail und Banner und Display-Anzeige |
| [!UICONTROL Zeitraum] | Zeitrahmen, für den das Asset verwendet wird, z. B. Quartal, Saison, Jahr usw. Beispiel: `Winter 2023` |
| Region | Regionen, für die das Asset verwendet wird. Beispiele: `North America`, `APAC`, `Italy` |
| Sprache | Sprachen, für die das Asset verwendet wird. Beispiel: `Spanish` |
| Keywords | Benutzerdefinierte Keywords werden zur weiteren Identifizierung von Asset-Merkmalen und -Zweck verwendet |

>[!TIP]
>
>Klicken Sie auf **[!UICONTROL Details bearbeiten]** (Bleistift), um Asset-Metadaten zu bearbeiten. Sie können beispielsweise den Asset-Namen ändern oder Schlüsselwörter hinzufügen oder entfernen.

## Erzeugungskontext

Der Abschnitt [!UICONTROL Generativer Kontext] zeigt, welche Informationen zum Generieren des Erlebnisses verwendet wurden, z. B. die während des [!DNL Create] verwendeten `Prompt`. Diese Einblicke können Ihnen helfen, noch erfolgreichere Varianten zu erstellen.

Die Informationen können Folgendes umfassen:

- `Brand`-, `Product`- und `Persona`, die während des [!DNL Create] ausgewählt wurden
- `Subject line` und `Preheader` für E-Mail-Erlebnisse
- `Headline` und `Body` für Meta-Anzeigen

## Verlauf

Erweitern Sie den _[!UICONTROL Verlauf]_ in einem Erlebnis, um eine Zeitleiste mit Genehmigungen und Aktivitäten anzuzeigen. Beispiel: Ein genehmigtes Erlebnis zeigt das Genehmigungsdatum, die Genehmigungszeit und die genehmigende Person an:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
