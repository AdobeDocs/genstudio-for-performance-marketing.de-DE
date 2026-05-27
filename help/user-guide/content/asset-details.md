---
title: Asset-Details
description: Adobe GenStudio for Performance Marketing speichert genehmigte Inhalte mit Rich-Metadaten, um die Suche und die Leistung zu verfolgen.
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
TQID: https://experienceleague.adobe.com/Hm7qcrP6VcXf6IqZ2pYybduNyjjV8kdWj571gcRpglI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f321b88b-6bb7-49cc-a16a-ae2b665ebd32id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a8b28c00-da6e-4d27-8667-80f790ad8972id: a98e0185-3180-4e8c-8f31-f72af4cc21a2id: b03d2162-d906-40a0-9cbd-001391e22d4aid: dd48f9df-f2e2-49fe-a918-332a8e240ffeid: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 732
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
Assets aus AEM-Repositorys zeigt verschiedene Metadaten an. Unter [Asset-Sichtbarkeit konfigurieren](connect-aem-repo.md#step-4-configure-asset-visibility) erfahren Sie, wie Sie [!DNL AEM Assets Content Hub] Asset-Details konfigurieren.

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
| Suchbegriffe | Benutzerdefinierte Keywords werden zur weiteren Identifizierung von Asset-Merkmalen und -Zweck verwendet |

>[!TIP]
>
Klicken Sie auf **[!UICONTROL Details bearbeiten]** (Bleistift), um Asset-Metadaten zu bearbeiten. Sie können beispielsweise den Asset-Namen ändern oder Schlüsselwörter hinzufügen oder entfernen.

## Erzeugungskontext

Der Abschnitt [!UICONTROL Generativer Kontext] zeigt, welche Informationen zum Generieren des Erlebnisses verwendet wurden, z. B. die während des [!DNL Create] verwendeten `Prompt`. Diese insight kann Ihnen dabei helfen, noch erfolgreichere Varianten zu erstellen.

Die Informationen können Folgendes umfassen:

- `Brand`-, `Product`- und `Persona`, die während des [!DNL Create] ausgewählt wurden
- `Subject line` und `Preheader` für E-Mail-Erlebnisse
- `Headline` und `Body` für Meta Ads

## Verlauf

Erweitern Sie den _[!UICONTROL Verlauf]_ in einem Erlebnis, um eine Zeitleiste mit Genehmigungen und Aktivitäten anzuzeigen. Beispiel: Ein genehmigtes Erlebnis zeigt das Genehmigungsdatum, die Genehmigungszeit und die genehmigende Person an:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
