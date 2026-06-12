---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# Referenz: Consumer Release Sources (MCP)

## Erkennung der Zeremonieseite

| Muster | Beispiel |
|---------|---------|
| Titel | `YYYY/MM Release Ceremony` in **GenStudio** Bereich |
| Aus Jira | Wiki-Link im Ticket `description` (bevorzugt) |
| CQL-Fallback | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## Funktionsgruppen der Zeremonie

Wikis für die Veröffentlichungszeremonie enthalten bis zu **2** Funktionstabellen. Analysieren Sie beide aus **Speicher** HTML.

### Funktionen der GA-Version

- Abschnittsüberschrift: `GA Release Features` (`<h2>`)
- Unterposition: `Feature Group:` mit optionalem Floodgate-Link
- Tabellenspalten umfassen **Typ** (`GA`, `Limited`, `EA`, `Beta` oder leer)
- **KT-Dokumentation** Spalte: `<ac:link><ri:page ri:content-title="..."/></ac:link>`

Extraktion pro Zeile:

| Feld | Quelle |
|-------|--------|
| `featureDescription` | Erste `<td>` in Datenzeile |
| `type` | Zellentext für Spalte eingeben |
| `ktPageTitle` | `ri:content-title` in KT-Spalte |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key` (nur intern) |
| `releaseTier` | `ga`, wenn Typ `GA` ist; Typ für andere GA-Tabellenwerte übernehmen |

### Beta-Versionsfunktionen

- Abschnittsüberschrift: `Beta Release Features` (kann **fehlen** in einigen Monaten)
- Zweite Tabelle; **keine Typspalte** — jede Zeile ist Beta
- KT- und Jira-Extraktion wie GA-Tabelle
- `releaseTier: beta` und `requiresBetaBadge: true` in jeder Beta-Abschnittszeile festlegen

Wenn der Abschnitt &quot;Beta&quot; fehlt, protokollieren Sie null Beta-Zeilen und fahren Sie fort.

### Speicher-HTML-Muster

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## Verwendung von MCP-Tools

| Schritt | Tool | Parameter |
|------|------|------------|
| Eintrittskarte | `jira_getIssue` | `issueKey`, optionale `expand: renderedFields` |
| Zeremonie | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| KT-Suche | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| KT-Textkörper | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**Verwenden Sie** Analyse von KT-Links `bodyMode: text` für Zeremonienseiten.

## KT-Feldzuordnung (Zeicheneingaben)

Ordnen Sie dies generieren-release-notes zu; fügen Sie dies nicht wörtlich in die öffentlichen Versionshinweise ein.

| KT-Strecke | Verwenden |
|------------|-----|
| Beschreibung | Kernfunktionen |
| Höhenverstellung | Wertvorschlag |
| Bereitgestellte Funktionen | Konkretes Verhalten |
| Problembeschreibung | Benutzerprobleme (nur Kontext) |
| Veröffentlichungstyp und Datum | GA/Beta/Limited (intern); Entscheidung über Laufwerkskennzeichen |

## Einschlussfilter

Bestätigen Sie den Umfang mit dem Benutzer, wenn Sie Unklarheiten haben. Allgemeine Voreinstellungen:

| Voreinstellung | Beinhaltet |
|--------|----------|
| `ga_only` | GA-Tabellenzeilen, bei denen Typ = `GA` |
| `ga_and_beta` | **Empfohlener Standard für zukünftige Monate** — GA-Zeilen mit Typ = `GA` **plus alle** Tabellenzeilen zu Beta-Versionsfunktionen |
| `ga_plus_empty` | GA-Tabelle: Typ = `GA` oder leerer Typ |
| `all_except_pilot` | GA-Tabellenzeilen außer `Limited`; plus Beta-Abschnitt bei Verwendung von `ga_and_beta` |
| `all_with_badges` | Alle Tabellenzeilen; Beta-Abschnittszeilen erhalten immer das Beta-Badge |

## Übergabe des Beta-Badges

| Bedingung | `requiresBetaBadge` |
|-----------|---------------------|
| Zeile aus der Tabelle mit den **Beta** Versionsfunktionen | `true` |
| GA-Tabellenzeile mit Typ = `Beta` | `true` |
| GA-Tabellenzeile mit Typ = `GA` | `false` |

Downstream: [generate-release-notes-decision rules](../generate-release-notes/SKILL.md#decision-rules) und [Beta-Badge-Snippet](../generate-release-notes/SKILL.md#beta-badge).

## Übergabe-Payload (informell)

Übergeben Sie an generate-release-notes als Liste von Elementen:

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
