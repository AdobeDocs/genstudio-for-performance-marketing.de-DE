---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---
## Zweck

Helfen Sie den KI-Kodierungs-Assistenten, kleine, sichere Änderungen am GenStudio for Performance Marketing-Dokumentations-Repository vorzunehmen.

## Hochrangige Architektur (kurz)
- Dieses Repository ist eine Dokumentations-Site, die aus Markdown unter `help/` mit freigegebenen Einschlüssen in `help/_includes/` und kuratierten Bildern unter `help/_includes/assets/` besteht.
- Versionshinweise, Benutzerhandbuch und Erweiterbarkeitsinhalte live unter `help/`. Große Inhaltsänderungen sollten die Frontend- und vorhandene Überschriftenstruktur beibehalten.
- Die Site wird mit Jekyll erstellt und auf GitHub-Seiten gehostet. Der Build-Prozess verwendet standardmäßige Jekyll-Konventionen mit einigen benutzerdefinierten Plug-ins.

## Projektspezifische Konventionen
- Cursor-Regeln: Benutzerdefinierte Automatisierung und Anleitung lebt in `.cursor/rules/*.mdc`. Beispiele: `.cursor/rules/docs-lint.mdc` (Lint-Prozess), `.cursor/rules/generate-release-notes.mdc` (verweist beim Bearbeiten von `help/user-guide/release-notes.md` auf die Kenntnis zu Versionshinweisen ). Führen Sie diese Schritte aus, um automatisierte Aufgaben durchzuführen.
- Agent-Fähigkeiten: Aufgaben-Workflows sind unter `.cursor/skills/<name>/SKILL.md` verfügbar. Beispiel: `.cursor/skills/generate-release-notes/SKILL.md` (vollständiges Verfahren mit Versionshinweisen zu GenStudio; verwenden Sie mit `examples.md` und `reference.md` im selben Ordner).
- Dateinamen und Schriftart:
   - Versionshinweise: Beibehalten vorhandener Experience League-Schriftarten auf `help/user-guide/release-notes.md` (siehe `.cursor/skills/generate-release-notes/reference.md#frontmatter`); die Thin-Regel `.cursor/rules/generate-release-notes.mdc` automatisch angehängt, wenn diese Datei bearbeitet wird.
   - Verwenden Sie den kebab-case für Regeldateien und `.mdc`.
- Formatierungskonventionen: Dokumente verwenden GitHub-Markdown. Überschriften folgen im Allgemeinen auf Groß- und Kleinschreibung und kurze Absätze. `*` Aufzählungszeichen sollten Sie für Listen in den Versionshinweisen und `###` für Funktionsabschnitte bevorzugen.

## Stilrichtlinien für die Dokumentation
- Befolgen Sie das Handbuch für den Schreibstil von [Microsoft](https://learn.microsoft.com/en-us/style-guide/) für die technische Dokumentation mit Best Practices:
   - Schreiben Sie klare, knappe Sätze, die sich auf Benutzeraktionen konzentrieren
   - Aktive Stimme und Präsenz verwenden
   - Text in kurze, scannbare Blöcke unterteilen
   - Behalten Sie einen warmen, direkten Ton bei und bewahren Sie gleichzeitig die technische Genauigkeit
- Markdown-Authoring:
   - Verwendung von Großbuchstaben für Überschriften (nur erstes Wort großschreiben)
   - Absätze aus Gründen der Lesbarkeit kurz halten (2-3 Sätze)
   - Leere Zeilen vor und nach Überschriften und Listen hinzufügen
   - Verwenden von Backticks für Benutzeroberflächenelemente, Dateipfade und Code
   - Alternativtext für alle Bilder einschließen
   - Verknüpfen mit bestimmten Abschnitten mithilfe von beschreibendem Text

## Sicherheitsregeln für Bearbeitungen (Was KI tun sollte)
- Fügen Sie niemals Jira-IDs, interne Links oder rein betriebliche Verweise auf öffentliche Dokumente hinzu. Siehe `.cursor/skills/generate-release-notes/SKILL.md` (Abschnitt **Verbotene Inhalte**)
- Bewahren Sie die Frontend-YAML genau bei der Bearbeitung von Dateien auf, die sie enthalten. Viele Vorlagen und Versionshinweise basieren auf festen Schlüsseln (Titel, Beschreibung, Rolle, exl-id).
- Für die Fehlerbehebung sollten Sie automatisierte, idempotente Bearbeitungen aus `.cursor/rules/docs-lint.mdc` bevorzugen (entfernen Sie nachfolgende Leerzeichen, stellen Sie den endgültigen Zeilenumbruch sicher). Von Menschen verwendete Beispielbefehle:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Beispiele (was zu ändern ist und wie)
- Fehlerbehebungen für kleine Kopien: Aktualisieren Sie Text in `help/` Markdown-Dateien, ohne die Überschriften und Anker zu verändern.
- Bildaktualisierungen: Referenzbilder unter `help/_includes/assets/`. Verschieben oder benennen Sie Bilder nicht um, ohne alle Verweise zu aktualisieren.

## Wo zuerst gesucht werden soll
- `help/_includes/` - Freigegebene Fragmente und Bilder.
- `.cursor/rules/` - Anleitung zur Automatisierung und Verknüpfung; verwenden Sie diese als maßgebliche Regeln für Formatierung und Prozesse.
- `markdownlint_custom.json` - Überschreibungen des lokalen Markdownlint.
- `.github/pull_request_template.md` — PR-Erwartungen.

## Wann man den Menschen fragen sollte
- Wenn eine Änderung das Ausführen oder Ändern von Docker-basierten Tools erfordert (die Link-Regel erwähnt Docker) oder sich auf Site-Build-Pipelines auswirkt.
- Wenn eine Datei auf eine unbekannte externe Konfiguration verweist (z. B. fehlt `markdownlint.json`) - fragen Sie, ob Sie sie erstellen oder ignorieren möchten.

## Minimale Befehle für Menschen

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

&#x200B;---
Wenn Sie möchten, kann ich dies in `.github/copilot-instructions.md` im Repository zusammenführen (oder Wortlaut/Länge anpassen). Was sollte ich ändern oder hinzufügen?
