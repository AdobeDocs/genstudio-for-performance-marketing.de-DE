---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Nutzung von Versionsquellen (Jira + Confluence MCP)

**Downstream Drafting:** [generate-release-notes](../generate-release-notes/SKILL.md) → optional [Polish-release-notes](../polish-release-notes/SKILL.md)

**Parsing-Referenz:** [reference.md](reference.md)

**Target-Ausgabedatei (nur nachgelagert):** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## Voraussetzungen

- **Jira MCP** (`jira_getIssue`, `jira_searchIssues`) authentifiziert
- **Confluence MCP** (`confluence_getContent`, `confluence_searchContent`) authentifiziert
- Jira-Ticketschlüssel aus Zweigname (`GS-#####`), Benutzereingabe oder Ticketbeschreibung

## Workflow-Checkliste

1. [ ] **Resolve Jira Ticket** — `jira_getIssue` mit `issueKey`. Lesen Sie `description` für die Zeremonie Wiki-Link und Release-Monat.
2. [ ] **Zeremonienseite suchen** — Wiki-URL aus Ticket verwenden; Fallback-CQL: `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`.
3. [ ] **Zeremonienkörper abrufen** — `confluence_getContent` mit `bodyMode: storage` (erforderlich; `text` verliert KT-Links und Tabellenstruktur).
4. [ ] **Funktionsgruppen analysieren** - Zeilen aus **GA-** und **Beta-** extrahieren (siehe [reference.md](reference.md#ceremony-feature-groups)).
5. [ ] **Einschlussfilter anwenden** — pro Benutzerbereich (siehe [reference.md](reference.md#inclusion-filters)); Bestätigung der Beta-Zeilenanzahl (kann null sein).
6. [ ] **KT-Seiten auflösen** — `confluence_searchContent` pro KT-Titel; `confluence_getContent` mit `bodyMode: text`.
7. [ ] **KT-Felder extrahieren** — Beschreibung, Aufzugsplatzierung, Ausgelieferte Funktionen, Problembeschreibung, Veröffentlichungstyp und Datum.
8. [ ] **Beta-Flags festlegen** - `requiresBetaBadge: true` für Beta-Abschnittszeilen oder GA-Tabellenzeilen mit dem Typ `Beta`.
9. [ ] **Übergabe** an [generate-release-notes](../generate-release-notes/SKILL.md) mit strukturierter Zeilenliste (keine Wiki/Jira Refs in ausgelieferter Kopie).

## Beta-Kennzeichnung (Übergabe zur Generierung von Kenntnissen)

Wenn `requiresBetaBadge: true`, muss der nachgelagerte `###` unter der Überschrift unmittelbar Folgendes enthalten:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

Fügen Sie keine Haftungsausschlüsse für die Planung der Kursivformatierung für Beta hinzu. Das Badge ist das unterstützte Muster.

## In den mitgelieferten Versionshinweisen verboten

Interne IDs, Wiki-URLs, Jira-Schlüssel und KT-Zitate verbleiben nur in dieser Aufnahmephase. Fassen Sie die benutzerfreundlichen Ergebnisse auf der öffentlichen Seite pro [Generate-Release-Notes - Verbotene Inhalte](../generate-release-notes/SKILL.md#prohibited-content) zusammen.

## Notfallversorgung

Wenn MCP-Aufrufe fehlschlagen, bitten Sie den Benutzer, Zeremonie und KT-Inhalte einzufügen, und fahren Sie dann mit generate-release-notes mit [reference.md KT-Feldzuordnung](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis) fort.

## Weitere Ressourcen

- [reference.md](reference.md) — Zeremonielles Parsen, CQL, Einschlussfilter, MCP-Parameter
- [generate-release-notes](../generate-release-notes/SKILL.md) — Archiv, Entwurf, Links, Qualitätsprüfungen
- [polish-release-notes](../polish-release-notes/SKILL.md) — Editorial Pass on New `###` under `{#latest}`
