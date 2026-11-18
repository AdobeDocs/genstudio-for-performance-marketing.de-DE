---
title: KI-Assistent - Tools-Referenz
description: Erfahren Sie mehr über die Tools Insights, Erstellen, Planen, Aktivieren und Feedback, die ein KI-Assistent mit [!DNL GenStudio for Performance Marketing] verwenden kann.
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# Referenz zu KI-Assistenten-Tools

In dieser Referenz werden die Tools beschrieben, die ein Connected AI-Assistent mit [!DNL GenStudio for Performance Marketing] verwenden kann. Die Liste der verfügbaren Tools hängt von der Konfiguration Ihres Unternehmens ab.

Fragen Sie Ihren KI-Assistenten, auf welche Tools er zugreifen kann, bevor Sie einen Workflow starten.

## Funktionsbereiche

| Bereich | Zweck | Verhalten |
|---|---|---|
| Insights | Fragen Sie die Leistung von bezahlten Medien und E-Mails ab und rufen Sie kreative Empfehlungen ab. | Schreibgeschützt. |
| Erstellen | Suchen Sie nach Assets, stellen Sie Entwürfe aus Express-Vorlagen oder Insights-Empfehlungen zusammen und verwalten Sie dann die Überprüfung. | Lesen und Schreiben. Erstellt Dokumente in Creative Cloud. |
| Plan | Extrahieren Sie Kampagnendetails aus einer Zusammenfassung und speichern Sie sie in Workfront Planning. | Das Extrahieren ist schreibgeschützt. Beim Speichern werden Datensätze in Workfront Planning erstellt und können nicht automatisch zurückgesetzt werden. |
| Aktivieren | Beheben Sie ein Veröffentlichungsziel und senden Sie ein genehmigtes Erlebnis an die Plattform. | Schreiben. Anzeigen werden an die Plattform gesendet und im Status „Aus“ veröffentlicht. Man schaltet sie separat ein. Durch diese Tools nicht umkehrbar. |
| Feedback | Senden Sie Produkt-Feedback an das [!DNL GenStudio for Performance Marketing]-Team. | Schreiben. |

Die meisten Insights-Tools umfassen `meta`, `linkedin` und `innovid`. Werkzeuge für Metrikwerte decken `meta` und `linkedin` ab. Das Reporting über E-Mail-Kampagnen umfasst Adobe Journey Optimizer (`ajo`) und Adobe Campaign (`acc`).

Create unterstützt `meta`, `linkedin`, `display`, `tiktok` und `youtube`. Activate unterstützt `META`, `LINKEDIN` und `GOOGLECM360`.

## Insights-Tools

### GET_INSIGHTS_CAPABILITIES

Gibt die für Ihre Organisation aktivierten Insights-Kanäle und Reporting-Vorgänge aus. Verwenden Sie dieses Tool zuerst, wenn die Verfügbarkeit unklar ist. Die unterstützten Kanäle sind `meta`, `linkedin`, `innovid`, `ajo` und `acc`.

Dieses Tool gibt Funktionsmetadaten zurück, nicht Kampagnen-, Anzeigen- oder Metrikwerte. Verwenden Sie `list_connected_channels_and_metrics`, um die benutzerdefinierten Metrikschlüssel Ihres Unternehmens zu finden.

### list_connected_channels_and_metrics

Gibt die aktiven Meta-, LinkedIn- und Google Campaign Manager 360-Verbindungen Ihres Unternehmens, die unterstützten Insights-Kanäle und -Vorgänge und die konfigurierten benutzerdefinierten Konversionsmetriken zurück. Verwenden Sie sie, um Metrikschlüssel zu finden, bevor Sie `get_insights_metric_values` aufrufen.

Dieses Tool gibt Metrikschlüssel, Beschriftungen und Formate zurück, nicht Metrikwerte. Eine Verbindung garantiert nicht, dass historische Berichtsdaten verfügbar sind.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. Lassen Sie beide aus, um den vollständigen Katalog zurückzugeben. |

### get_insights_summary

Gibt allgemeine Leistungsmetriken und Trends für einen Kanal über einen ausgewählten Datumsbereich zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `startDate` | Nein | Startdatum im `YYYY-MM-DD`. Der Standardwert ist „vor 30 Tagen“. |
| `endDate` | Nein | Enddatum im `YYYY-MM-DD`. Die Standardeinstellung ist „Heute“. |
| `metrics` | Nein | Diagrammmetriken: `spend`, `ctr`, `cpc`, `cpm`, `cpa`, `impressions`, `clicks`, `conversions`, `videoPlays`, `engagement`, `likes`, `comments` oder `shares`. Der Standardwert lautet `spend`, `ctr`, `cpc` und `cpm`. |

### list_insights_campaigns

Gibt eine sortierbare Tabelle mit Kampagnenleistungsmetriken und eine Zeile mit Gesamtsummen zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. Der Standardwert ist die letzten 30 Tage. |
| `search` | Nein | Filter für Kampagnennamen. |
| `sortBy` | Nein | Sortierfeld: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` oder `name`. Der Standardwert lautet `spend`. Die Ergebnisse werden immer absteigend sortiert. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. Die Standardseitengröße ist 20. |

### list_insights_email_campaigns

Gibt eine sortierbare Tabelle mit E-Mail-Kampagnen mit Versand- und Interaktionsmetriken für Adobe Journey Optimizer und Adobe Campaign zurück. Verwenden Sie für Werbekampagnen `list_insights_campaigns`.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `ajo` oder `acc`. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. Der Standardwert ist die letzten 30 Tage vor dem Enddatum. |
| `search` | Nein | Filter für Kampagnennamen. |
| `sortBy` | Nein | Sortierfeld: `campaignName`, `emailsNumber`, `emailsDelivered`, `totalClicks`, `openRate`, `ctr`, `ctor`, `bounceRate`, `unsubscribeRate` oder `spamComplaintRate`. Der Standardwert lautet `emailsDelivered`. Die Ergebnisse werden immer absteigend sortiert. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

### list_insights_ads

Gibt die Leistung auf Anzeigenebene zurück. Verwenden Sie den standardmäßigen Durchsuchen-Modus für eine sortierbare Tabelle oder einen Stufenmodus für Anzeigen mit hoher und niedriger Leistung.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `meta`, `linkedin` oder `innovid`. |
| `tier` | Nein | `all`, `high` oder `low`. Der Standardwert lautet `all`. |
| `mainMetric` | Nein | Rangfolgemetrik für den `high`- oder `low`: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` oder `clicks`. Im Durchsuchen-Modus ignoriert. |
| `metrics` | Nein | Zusätzliche Metriken, die für jede Anzeige im Ebenenmodus gemeldet werden. |
| `campaigns` | Nein | Zur Begrenzung des Ergebnisses verwendete Kampagnen, bis zu 50. Jede Kampagne umfasst `channel`, `accountId` und `campaignId`. |
| `search` | Nein | Anzeigennamenfilter. |
| `sortBy` | Nein | Sortierfeld „Durchsuchen-Modus“: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` oder `name`. Der Standardwert lautet `spend`. Die Ergebnisse werden immer absteigend sortiert. |
| `spendMin`, `spendMax` | Nein | Gesamtausgabengrenzen für jede Anzeige. Nur Stufenmodus. |
| `includeUnsupported` | Nein | Enthält Anzeigen, deren Kreative nicht gerendert werden können. Der Standardwert lautet `false`. |
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
| `ads` | Ja | Eine bis 200 Anzeigen zu erklären. Jede Anzeige enthält `channel`, `accountId`, `campaignId` und `adId` sowie optional `adGroupId` und `performanceTier` (`high` oder `low`). Verwenden Sie die von `list_insights_ads` im Stufenmodus zurückgegebenen Kennungen. |
| `mainMetric` | Ja | Die für die Rangfolge der Anzeigen verwendete Metrik: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` oder `clicks`. |
| `campaigns` | Nein | Zur Definition der Vergleichspopulation verwendete Kampagnen, bis zu 50. Jede Kampagne umfasst `channel`, `accountId` und `campaignId`. |
| `spendMin`, `spendMax` | Nein | Ausgabengrenzen für die Vergleichspopulation. |
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
| `tagSource` | Nein | `ad_tags` oder `campaign_tags`. Der Standardwert lautet `ad_tags`. |
| `sortBy` | Nein | Sortierfeld: `adsCount`, `spend`, `impressions`, `clicks`, `conversionCount`, `ctr`, `cpc`, `cpm` oder `cpa`. Der Standardwert lautet `adsCount`. |
| `search` | Nein | Tag-Wert-Filter. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

### get_insights_metric_values

Gibt die Werte und Trends für die verfolgten Metriken Ihres Unternehmens zurück, z. B. Interessenten, Anmeldungen oder Rendite auf Werbeausgaben für Meta und LinkedIn.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channels` | Nein | `meta`, `linkedin` oder beides. |
| `metrics` | Nein | Bis zu 20 Metrikschlüssel von `list_connected_channels_and_metrics` zurückgegeben. Der Standardwert ist der standardmäßige sichtbare Satz Ihres Unternehmens. |
| `campaigns` | Nein | Zur Begrenzung des Ergebnisses verwendete Kampagnen, bis zu 50. Jede Kampagne umfasst `channel`, `accountId` und `campaignId`. |
| `startDate`, `endDate` | Nein | Datumsbereich im `YYYY-MM-DD`. Der Standardwert ist die letzten 30 Tage. |

### get_insights_recommendations

Gibt vorgeschlagene kreative Änderungen zurück, die auf den Leistungsdaten Ihres Unternehmens basieren. Eine Anfrage kann keine Empfehlungen zurückgeben, wenn der ausgewählte Umfang keine geeigneten Anzeigen enthält.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channels` | Ja | Eine oder mehrere `meta`, `linkedin` oder `innovid`. |
| `campaigns` | Nein | Zur Begrenzung des Ergebnisses verwendete Kampagnen, bis zu 50. Jede Kampagne umfasst `channel`, `accountId` und `campaignId`. |
| `search` | Nein | Filter für Kampagnennamen. |
| `recommendationId` | Nein | Die `adUid` einer Empfehlung, die zum detaillierten Abrufen verwendet wird. |
| `onlyWithPreview` | Nein | Schließt Recommendations aus, die keine beispielhafte kreative Vorschau haben. Der Standardwert lautet `true`. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

## Erstellen von Tools

Erstellen Sie Tools, suchen Sie Assets, stellen Sie Entwürfe aus Adobe Express-Vorlagen zusammen und verwalten Sie die Überprüfung, bevor ein Erlebnis zur Aktivierung bereit ist.

### list_express_templates

Listet die verfügbaren Express-Vorlagen mit Filtern und Facettenzahlen auf.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Nein | `meta`, `display`, `linkedin`, `tiktok`, `youtube` oder `__unspecified__`. |
| `query` | Nein | Suchbegriff für Vorlagen. |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | Nein | Facettenfilter für Vorlagen. |
| `sortBy` | Nein | `modified` oder `created`. Der Standardwert lautet `modified`. |
| `order` | Nein | `asc` oder `desc`. Der Standardwert lautet `desc`. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

### describe_express_template

Gibt die bearbeitbaren Textfelder und Bildplatzierungen in einer Vorlage zurück.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `templateId` | Ja | Express-Vorlagenkennung. |

### list_cta_options

Gibt die zulässigen call-to-action-Werte für einen Kanal zurück. Die Anzeige gibt eine leere Liste zurück, da sie Freiformtext akzeptiert.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `linkedin`, `meta`, `display`, `tiktok` oder `youtube`. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. Lassen Sie beide weg, um jede Option zurückzugeben. |

### search_assets

Durchsucht die Bilder und Videos in Ihren GenStudio-Inhalten. Verwenden Sie sie, um vorhandene Assets für einen Entwurf auszuwählen. Abgeleitete, externe und abgelaufene Assets werden ausgeschlossen. Dieses Tool kann keine Assets hochladen, bearbeiten, löschen oder generieren und erfordert eine Berechtigung für GenStudio-Inhalte.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `query` | Nein | Suche nach Keywords oder natürlicher Sprache in Asset-Metadaten. |
| `mediaTypes` | Nein | `image`, `video` oder beides. Die Standardeinstellung enthält beide. |
| `aspectRatios` | Nein | Seitenverhältnisse wie `1:1` oder `16:9`. Wenn ein Verhältnis nicht verfügbar ist, gibt das Tool die verfügbaren Auswahlmöglichkeiten zurück. |
| `brands`, `campaigns`, `products`, `personas`, `channels` | Nein | Filtert nach Namen. |
| `customMetadata` | Nein | Bis zu 5 Metadatenfelder mit jeweils einem oder mehreren Werten. |
| `uploadedBy` | Nein | `me` oder eine Uploader-E-Mail-Adresse. |
| `createdAtFrom`, `createdAtTo` | Nein | Erstellungszeitgrenzen im ISO 8601-Format. |
| `aiGenerated` | Nein | Filtert nach dem Status der KI-Generierung. |
| `contentCredentials` | Nein | Filtert nach dem Content Credentials-Status. |
| `limit`, `offset` | Nein | Seitengröße und Paging-Versatz. |

Das Ergebnis enthält stabile Asset-Verweise für `create_draft` und kurzlebige signierte URLs.

### create_draft

Erstellt einen bearbeitbaren Entwurf aus einer Express-Vorlage mit einem oder mehreren Erlebnissen. Jeder Aufruf erstellt einen neuen Entwurf.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `templateId` | Ja | Express-Vorlagenkennung. |
| `prompt` | Ja | Creative-Kurzanweisungen und -Kopieranweisungen, die mit dem Entwurf gespeichert sind. |
| `experiences` | Ja | Ein oder mehrere Erlebnisse. Siehe folgende Tabelle. |
| `name` | Nein | Dokumentname. |
| `allowAssetReuse` | Nein | Ermöglicht die Wiederverwendung eines ausgewählten Assets für mehrere Erlebnisse. Der Standardwert lautet `false`. |

Jedes Erlebnis unterstützt diese Felder:

| Feld | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Ja | `linkedin`, `meta`, `display`, `tiktok` oder `youtube`. |
| `title` | Nein | Erlebnis-Titel. Der Standardwert lautet „Konzept *n*&quot;. |
| `headline` | Meta und LinkedIn | Primäre Überschrift. |
| `body` | Meta, LinkedIn und TikTok | Textkörper-Kopie. Für LinkedIn ist dies der Einführungstext. Bei TikTok ist dies der Primärtext. |
| `description` | YouTube | Anzeigenbeschreibung. Optional für Meta und LinkedIn. |
| `display_url` | Meta und LinkedIn | Anzeige-URL in der Anzeige. |
| `destination_url` | Nein | URL, auf die die Anzeige verweist. |
| `cta` | Nein | Call-to-action-Text aus `list_cta_options`. |
| `templateFields` | Nein | Überschreibungen für benannte Vorlagenelemente aus `describe_express_template`. Jede Überschreibung setzt Text, eine Bild-URL mit Abmessungen oder eine Video-URL. |
| `assetTemplateFields` | Nein | Inhalts-Assets aus `search_assets` für Bild- oder Videofelder in der Vorlage. |

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
| `emails` | Ja | Eine bis 20 E-Mail-Adressen von Mitwirkenden. |
| `role` | Ja | `editor` oder `viewer`. |
| `message` | Nein | Einladungsnachricht. |

### request_draft_approval

Sendet einen Entwurf zur Genehmigung an eine oder mehrere Personen.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `draftId` | Ja | Kennung des Entwurfs-Assets. |
| `emails` | Ja | Eine bis 20 E-Mail-Adressen der Prüfer. |

### list_experiences

Gibt genehmigte, veröffentlichte Erlebnisse zurück, die aktiviert werden können. Entwürfe sind nicht enthalten.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `channel` | Nein | `email`, `meta`, `meta_organic`, `display`, `ctv`, `linkedin`, `linkedin_organic`, `tiktok`, `chatgpt` oder `youtube`. |
| `createdByMe` | Nein | Beschränkt Ergebnisse auf Erlebnisse, die vom aktuellen Benutzer erstellt wurden. |
| `campaignNames` | Nein | Bis zu 5 exakte Filter für Kampagnennamen. |
| `creatorEmail` | Nein | E-Mail-Filter des Erstellers. |
| `createdAtFrom`, `createdAtTo` | Nein | Datumsgrenzen für die Erstellung. |
| `language` | Nein | BCP 47-Sprach-Tag. |
| `limit`, `cursor` | Nein | Seitengröße (1-50, Standard 20) und Paginierungscursor. |

## Planungs-Tools

Planungs-Tools wandeln eine Kampagnenbeschreibung in einen überprüfbaren Kampagnenentwurf um und speichern sie in Workfront Planning.

### extract_campaign_from_brief

Extrahiert einen überprüfbaren Kampagnenentwurf aus einer eingefügten Marketing-Zusammenfassung. Dieses Tool speichert keine Datensätze. Fehlende Fakten und Daten werden nicht abgeleitet.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `briefText` | Ja | Vollständiger Text einer Kampagnenbeschreibung mit bis zu 100.000 Zeichen. Dateien und Links werden nicht unterstützt. |

Das Ergebnis enthält einen Kampagnenentwurf, Ergebnisse mit unterstützenden Anführungszeichen, empfohlene Zielgruppen und Warnungen.

### create_workfront_campaign

Erstellt eine Workfront Planning-Kampagne mit verknüpften Produkten und Rollen aus einem Entwurf, den Sie geprüft und genehmigt haben. Dieses Tool ist nicht idempotent und Datensätze können nicht automatisch zurückgesetzt werden. Überprüfen Sie Workfront, bevor Sie einen Schreibvorgang wiederholen, der möglicherweise erfolgreich war.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `campaignDraft` | Ja | Der genehmigte Entwurf. Erfordert `name`. Optionale Felder sind `description`, `objective`, `keyMessaging`, `startDate`, `endDate` (`YYYY-MM-DD`), `status`, `channels`, `products` und `personas`. |
| `channelSelections` | Nein | Genehmigte Auswahlmöglichkeiten für mehrdeutige Kanalnamen. |
| `entitySelections` | Nein | Bestehende Produkt- und Persona-Einträge genehmigt. Verwenden Sie `null` , um einen neuen Datensatz anzufordern. |
| `createMissingEntities` | Nein | Erstellt die Produkte und Rollen, die Sie als neu ausgewählt haben. Der Standardwert lautet `false`. |

Wenn ein Produkt, eine Rolle oder ein Kanal mehrdeutig ist, gibt das Tool zur Bestätigung Auswahlmöglichkeiten zurück und nimmt keine Änderungen vor.

## Tools aktivieren

Aktivierungs-Tools lösen eine Paid-Media-Zielgruppe und senden ein genehmigtes Erlebnis an die Plattform. Anzeigen werden im ausgeschalteten Zustand veröffentlicht (Meta angehalten, LinkedIn-Entwurf, Campaign Manager 360 inaktiv), sodass sie separat aktiviert werden müssen, bevor sie gesendet werden. Das Senden von Anzeigen an die Plattform kann mit diesen Tools nicht rückgängig gemacht werden.

### configure_activation_target

Löst das Paid-Media-Konto, die Kampagne, das Anzeigen-Set und die Facebook-Seite auf und validiert sie, falls erforderlich.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `platform` | Ja | `META`, `LINKEDIN` oder `GOOGLECM360`. |
| `platformAccountId` | Nein | Kennung des Paid-Media-Kontos. Lassen Sie es aus, um Konten zu ermitteln. |
| `campaignId` | Nein | Kampagnenkennung für Meta oder LinkedIn. Wird nicht für Campaign Manager 360 verwendet. |
| `adsetId` | Nein | Meta-Anzeigensatz oder LinkedIn-Kampagnenkennung. Wird nicht für Campaign Manager 360 verwendet. |
| `pageId` | Nein | Facebook-Seitenkennung für Meta. |

Für Campaign Manager 360 ist nur das Werbekonto erforderlich.

### create_activation

Sendet ein genehmigtes Erlebnis als Werbung an die Plattform unter Verwendung einer validierten Zielgruppe. Die Anzeigen werden im ausgeschalteten Zustand veröffentlicht. Meta erstellt für jedes Seitenverhältnis eine Anzeige mit dem ersten Bild. LinkedIn und Campaign Manager 360 erstellen für jedes aufgelöste Bild eine Anzeige.

| Parameter | Erforderlich | Beschreibung |
|---|---|---|
| `platform` | Ja | `META`, `LINKEDIN` oder `GOOGLECM360`. |
| `targetId` | Ja | Validierte Zielgruppe von `configure_activation_target` zurückgegeben. |
| `experienceId` | Ja | Von `list_experiences` zurückgegebene genehmigte Erlebnis-ID. |
| `name` | Nein | Anzeigename der Anzeigenplatzierung. Der Standardwert ist der Anzeigentitel des Erlebnisses. |

Das Ergebnis listet die Anzahl der erstellten, in die Warteschlange gestellten und übersprungenen Anzeigen mit dem ursprünglichen Status jeder Anzeige und einem Link dazu in [!DNL GenStudio for Performance Marketing] auf. Der Status `PENDING` bedeutet, dass der Auftrag in die Warteschlange gestellt wird und nicht, dass die Anzeige gesendet wird.

Wenn Sie `create_activation` zweimal aufrufen, werden zusätzliche Anzeigen erstellt, anstatt die ersten Anzeigen zu aktualisieren.

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
- **Getrackte Metriken überprüfen:** Rufen Sie `list_connected_channels_and_metrics` auf und rufen Sie dann `get_insights_metric_values` mit den zurückgegebenen Metrikschlüsseln auf.
- **Umwandeln einer Empfehlung in einen Entwurf:** Anruf `get_insights_recommendations`, dann Anruf `create_draft_from_recommendation`.
- **Erstellen aus einer Vorlage:** Rufen Sie `list_express_templates`, `describe_express_template` und `list_cta_options` auf und rufen Sie dann `create_draft` auf.
- **Aus vorhandenen Assets erstellen:** Rufen Sie `search_assets` auf und übergeben Sie dann die zurückgegebenen Asset-Verweise an `create_draft` in `assetTemplateFields`.
- **Kampagnenkürzel in Workfront speichern** Anruf `extract_campaign_from_brief`, Entwurf überprüfen und dann `create_workfront_campaign` anrufen.
- **Senden eines genehmigten Erlebnisses an eine Plattform:** Rufen Sie `list_experiences` auf und rufen Sie dann `configure_activation_target` und `create_activation` auf.

## Verwandte Funktionen

- [Übersicht über KI-Assistenten](overview.md)
- [KI-Assistenten verbinden](connect-ai-assistants.md)
- [Verwenden von KI-Assistenten](use-ai-assistants.md)
