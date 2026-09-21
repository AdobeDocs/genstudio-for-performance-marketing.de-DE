---
title: KI-Assistent - Tools-Referenz
description: Erfahren Sie mehr über die Tools „Insights“, „Erstellen“, „Aktivieren“ und „Feedback“, die ein KI-Assistent mit [!DNL GenStudio for Performance Marketing] verwenden kann.
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# Referenz zu KI-Assistenten-Tools

In dieser Referenz werden die Tools beschrieben, die ein Connected AI-Assistent mit [!DNL GenStudio for Performance Marketing] verwenden kann. Die Liste der verfügbaren Tools hängt von der Konfiguration Ihres Unternehmens ab.

Fragen Sie Ihren KI-Assistenten, auf welche Tools er zugreifen kann, bevor Sie einen Workflow starten.

## Funktionsbereiche

| Bereich | Zweck | Verhalten |
|---|---|---|
| Insights | Fragen Sie die Paid-Media-Leistung ab und rufen Sie kreative Empfehlungen ab. | Schreibgeschützt. |
| Erstellen | Stellen Sie Entwürfe aus Express-Vorlagen oder Insights-Empfehlungen zusammen und verwalten Sie dann die Überprüfung. | Lesen und Schreiben. Erstellt Dokumente in Creative Cloud. |
| Aktivieren | Beheben Sie ein Veröffentlichungsziel und veröffentlichen Sie ein genehmigtes Erlebnis. | Schreiben und zerstören. Kann eine Live-Anzeige veröffentlichen und Ausgaben verursachen. |
| Feedback | Senden Sie Produkt-Feedback an das [!DNL GenStudio for Performance Marketing]-Team. | Schreiben. |

Die meisten Insights-Tools umfassen `meta`, `linkedin` und `innovid`. Tools für Konversionsmetriken decken `meta` und `linkedin` ab.

Create unterstützt `meta`, `linkedin`, `display`, `tiktok` und `youtube`. Activate unterstützt `META`, `LINKEDIN` und `GOOGLECM360`.

## Insights-Tools

### GET_INSIGHTS_CAPABILITIES

Gibt die Insights-Kanäle, -Vorgänge und benutzerdefinierten Konversionsmetriken zurück, die für Ihre Organisation aktiviert sind. Verwenden Sie dieses Tool zuerst, wenn die Verfügbarkeit unklar ist.

Dieses Tool gibt Funktionsmetadaten zurück, nicht Kampagnen-, Anzeigen- oder Metrikwerte.

### get_insights_summary

Gibt allgemeine Leistungsmetriken und Trends für einen Kanal über einen ausgewählten Datumsbereich zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `startDate` | Nein | Startdatum im `YYYY-MM-DD`. Der Standardwert ist „vor 30 Tagen“. |
| `endDate` | Nein | Enddatum im `YYYY-MM-DD`. Die Standardeinstellung ist „Heute“. |
| `metrics` | Nein | Diagrammmetriken wie `spend`, `ctr`, `cpc`, `cpm`, `impressions`, `clicks` oder `conversions`. |

### list_insights_campaigns

Gibt eine sortierbare Tabelle mit Kampagnenleistungsmetriken und eine Zeile mit Gesamtsummen zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. Der Standardwert ist die letzten 30 Tage. |
| `search` | Nein | Filter für Kampagnennamen. |
| `sortBy` | Nein | Sortierfeld, z. B. `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` oder `name`. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

### list_insights_ads

Gibt die Leistung auf Anzeigenebene zurück. Verwenden Sie den standardmäßigen Durchsuchen-Modus für eine sortierbare Tabelle oder einen Stufenmodus für Anzeigen mit hoher und niedriger Leistung.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `tier` | Nein | `all`, `high` oder `low`. Der Standardwert lautet `all`. |
| `mainMetric` | bedingt | Rangfolgemetrik ist für `high` oder `low` erforderlich. |
| `campaigns` | Nein | Zur Ergebnisbegrenzung verwendete Kampagnenkennungen. |
| `search` | Nein | Anzeigennamenfilter. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

Der Stufenmodus gibt die von `get_insights_ad_attributes` benötigten Anzeigenkennungen zurück.

### get_insights_ad_details

Gibt kreative Metadaten für eine Anzeige zurück, einschließlich Kopie, call to action, Assets und Platzierungen. Es werden keine Leistungsmetriken zurückgegeben.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `accountId` | Ja | Kennung des Paid-Media-Kontos. |
| `campaignId` | Ja | Kampagnenkennung. |
| `adId` | Ja | Anzeigenkennung. |
| `adgroupId` | Nein | Anzeigengruppenkennung, wenn der Kanal Anzeigengruppen verwendet. |

### get_insights_ad_attributes

Vergleicht kreative Eigenschaften für ausgewählte Anzeigen mit dem Kanaldurchschnitt. Verwenden Sie sie, nachdem `list_insights_ads` Anzeigen mit hoher oder niedriger Leistung identifiziert hat.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `ads` | Ja | Zu erläuternde Anzeigen, einschließlich der von `list_insights_ads` zurückgegebenen Kennungen. |
| `mainMetric` | Ja | Die für die Platzierung der Werbeanzeigen verwendete Metrik. |
| `campaigns` | Nein | Kampagnenkennungen, die zur Definition der Vergleichspopulation verwendet werden. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. |

### get_insights_tag_categories

Gibt die Tag-Kategorien zurück, die für Ihre Organisation im angeforderten Zeitraum verfügbar sind. Es werden Kategorienamen, nicht Leistungsmetriken zurückgegeben.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channels` | Ja | Ein oder mehrere unterstützte Kanäle. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. |

### get_insights_ad_tags

Gibt die Leistung nach Tag-Wert innerhalb einer Kategorie zurück, z. B. Produkt, Region oder kreatives Design.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `tagCategory` | Ja | Eine von `get_insights_tag_categories` zurückgegebene Kategorie. |
| `tagSource` | Nein | `ad_tags` oder `campaign_tags`. |
| `sortBy` | Nein | Metrik zum Sortieren des Ergebnisses. |
| `search` | Nein | Tag-Wert-Filter. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. |

### get_insights_custom_metrics

Gibt die für Ihre Organisation konfigurierten benutzerdefinierten Konversionsmetriken aus. Vor dem `get_insights_conversion_metrics` verwenden.

Dieses Tool gibt Metrikkennungen zurück, keine Metrikwerte.

### get_insights_conversion_metrics

Gibt konfigurierte Werte und Trends für die Konversionsmetrik für Meta und LinkedIn zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channels` | Nein | Unterstützter Konvertierungskanal. Der Standardwert lautet `meta`. |
| `metrics` | Nein | Von `get_insights_custom_metrics` zurückgegebene Metrikkennungen. |
| `campaigns` | Nein | Zur Ergebnisbegrenzung verwendete Kampagnenkennungen. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. |

### get_insights_recommendations

Gibt vorgeschlagene kreative Änderungen zurück, die auf den Leistungsdaten Ihres Unternehmens basieren. Eine Anfrage kann keine Empfehlungen zurückgeben, wenn der ausgewählte Umfang keine geeigneten Anzeigen enthält.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channels` | Ja | Ein oder mehrere unterstützte Kanäle. |
| `campaigns` | Nein | Zur Ergebnisbegrenzung verwendete Kampagnenkennungen. |
| `search` | Nein | Filter für Kampagnennamen. |
| `recommendationId` | Nein | Kennung, die zum Abrufen einer einzelnen Empfehlung verwendet wird. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

## Erstellen von Tools

Erstellen Sie Tools, stellen Sie Entwürfe aus Adobe Express-Vorlagen zusammen und verwalten Sie Überprüfungen, bevor ein Erlebnis bereit zur Aktivierung ist.

### list_express_templates

Listet die verfügbaren Express-Vorlagen mit Filtern und Facettenzahlen auf.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Nein | `meta`, `display`, `linkedin`, `tiktok`, `youtube` oder `__unspecified__`. |
| `query` | Nein | Suchbegriff für Vorlagen. |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | Nein | Facettenfilter für Vorlagen. |
| `sortBy`, `order` | Nein | Sortierfeld und -reihenfolge |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

### describe_express_template

Gibt die bearbeitbaren Textfelder und Bildplatzierungen in einer Vorlage zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `templateId` | Ja | Express-Vorlagenkennung. |

### list_cta_options

Gibt die zulässigen call-to-action-Werte für einen Kanal zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `linkedin`, `meta`, `display`, `tiktok` oder `youtube`. |

### create_draft

Erstellt einen bearbeitbaren Entwurf aus einer Express-Vorlage mit einem oder mehreren Erlebnissen.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `templateId` | Ja | Express-Vorlagenkennung. |
| `prompt` | Ja | Creative-Kurzanweisungen und -Kopieranweisungen, die mit dem Entwurf gespeichert sind. |
| `experiences` | Ja | Kanal-, Inhaltsfelder und optionale Vorlagenfelder überschreiben für jedes Erlebnis. |
| `name` | Nein | Dokumentname. |

Verwenden Sie `list_cta_options` , bevor Sie einen Entwurf für einen Kanal mit festen call-to-action-Werten erstellen.

### create_draft_from_recommendation

Erstellt einen bearbeitbaren Entwurf aus einer bestimmten Insights-Empfehlung.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta` oder `linkedin`. |
| `adUid` | Ja | Von `get_insights_recommendations` zurückgegebene Empfehlungskennung. |
| `prompt` | Ja | Creative Brief basierend auf der Empfehlung. |
| `name` | Nein | Dokumentname. |

### list_recent_drafts

Listet die aktuellen Express-Vorlagenentwürfe mit ihrem Status und ihren Links auf.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

### get_draft_metadata

Gibt den Namen, die Kanäle, den Genehmigungsstatus, die Ergebnisse der Validierungsverantwortlichen und den Zugriff auf Mitwirkende eines Entwurfs zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `draftId` | Ja | Kennung des Entwurfs-Assets. |

### share_draft

Ermöglicht Mitwirkenden das Anzeigen oder Bearbeiten eines Entwurfs, ohne dessen Genehmigung anzufordern.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `draftId` | Ja | Kennung des Entwurfs-Assets. |
| `emails` | Ja | Eine oder mehrere E-Mail-Adressen von Mitwirkenden. |
| `role` | Ja | `editor` oder `viewer`. |
| `message` | Nein | Einladungsnachricht. |

### request_draft_approval

Sendet einen Entwurf zur Genehmigung an eine oder mehrere Personen.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `draftId` | Ja | Kennung des Entwurfs-Assets. |
| `emails` | Ja | Eine oder mehrere E-Mail-Adressen von Prüfern. |

### list_experiences

Gibt genehmigte, veröffentlichte Erlebnisse zurück, die aktiviert werden können. Entwürfe sind nicht enthalten.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Nein | Erlebniskanalfilter. |
| `createdByMe` | Nein | Beschränkt Ergebnisse auf Erlebnisse, die vom aktuellen Benutzer erstellt wurden. |
| `campaignNames` | Nein | Exakte Filter für Kampagnennamen. |
| `creatorEmail` | Nein | E-Mail-Filter des Erstellers. |
| `createdAtFrom`, `createdAtTo` | Nein | Datumsgrenzen für die Erstellung. |
| `language` | Nein | BCP 47-Sprach-Tag. |
| `limit`, `cursor` | Nein | Seitengröße und Paginierungscursor. |

## Tools aktivieren

Aktivierungs-Tools lösen eine Paid-Media-Zielgruppe und veröffentlichen ein genehmigtes Erlebnis. Die Veröffentlichung kann mit diesen Tools nicht rückgängig gemacht werden und kann Kosten verursachen.

### configure_activation_target

Löst das Paid-Media-Konto, die Kampagne, das Anzeigen-Set und die Facebook-Seite auf und validiert sie, falls erforderlich.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `platform` | Ja | `META`, `LINKEDIN` oder `GOOGLECM360`. |
| `platformAccountId` | Nein | Kennung des Paid-Media-Kontos. Lassen Sie es aus, um Konten zu ermitteln. |
| `campaignId` | Nein | Kampagnenkennung für Meta oder LinkedIn. |
| `adsetId` | Nein | Meta-Anzeigensatz oder LinkedIn-Kampagnenkennung. |
| `pageId` | Nein | Facebook-Seitenkennung für Meta. |

### create_activation

Veröffentlicht eine Live-Anzeige mit einem Bild aus einem genehmigten Erlebnis und validierten Ziel.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `platform` | Ja | `META`, `LINKEDIN` oder `GOOGLECM360`. |
| `targetId` | Ja | Validierte Zielgruppe von `configure_activation_target` zurückgegeben. |
| `experienceId` | Ja | Von `list_experiences` zurückgegebene genehmigte Erlebnis-ID. |
| `assetId` | Nein | Variantenkennung für ein Erlebnis mit mehreren geeigneten Varianten. |
| `name` | Nein | Anzeigename der Anzeigenplatzierung. |

Wenn Sie `create_activation` zweimal aufrufen, werden zwei separate Anzeigen erstellt, anstatt die erste Anzeige zu aktualisieren.

## Feedback-Tool

### submit_mcp_feedback

Sendet Feedback zu einem Tool oder Workflow an das [!DNL GenStudio for Performance Marketing].

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `category` | Ja | `bug`, `feature_request` oder `workflow_friction`. |
| `comment` | Ja | Eine kurze Beschreibung des Feedbacks. |
| `tags` | Nein | Tags, die zur Kategorisierung des Feedbacks verwendet werden |
| `tool_name` | Nein | Das mit dem Feedback verknüpfte Tool. |

## Allgemeine Workflows

Verwenden Sie diese Sequenzen, wenn ein Tool Kennungen oder Konfigurationen für ein anderes bereitstellt:

- **Diagnose einer Anzeige:** Rufen Sie `list_insights_ads` im `high`- oder `low`-Modus auf und rufen Sie dann `get_insights_ad_attributes` mit derselben Rangfolgenmetrik auf.
- **Analysieren nach Tag:** Rufen Sie `get_insights_tag_categories` auf und rufen Sie dann `get_insights_ad_tags` mit einer zurückgegebenen Kategorie auf.
- **Konversionsmetriken überprüfen:** Rufen Sie `get_insights_custom_metrics` auf und rufen Sie dann `get_insights_conversion_metrics` mit den zurückgegebenen Metrikkennungen auf.
- **Umwandeln einer Empfehlung in einen Entwurf:** Anruf `get_insights_recommendations`, dann Anruf `create_draft_from_recommendation`.
- **Erstellen aus einer Vorlage:** Rufen Sie `list_express_templates`, `describe_express_template` und `list_cta_options` auf und rufen Sie dann `create_draft` auf.
- **Genehmigte Erlebnisse veröffentlichen:**-Aufruf `list_experiences`, dann `configure_activation_target` und `create_activation` aufrufen.

## Verwandte Funktionen

- [Übersicht über KI-Assistenten](overview.md)
- [KI-Assistenten verbinden](connect-ai-assistants.md)
- [Verwenden von KI-Assistenten](use-ai-assistants.md)
