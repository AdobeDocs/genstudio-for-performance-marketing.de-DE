---
name: generate-release-notes
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


# Versionshinweise zu GenStudio generieren

**Kanonische Zieldatei:** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Vollständige Beispiele:** [Examples.md](examples.md)

**KT/wiki-Feldzuordnung und Dokumentenpfade:** [reference.md](reference.md)

## Bearbeitungsbereich (streng)

Wenn Sie diese Fähigkeit verwenden **(der einzige Ort** können Sie den Inhalt **Versionshinweisen** hinzufügen **oder** bearbeiten), ist der Abschnitt mit der Überschrift **`## … {#latest}`** (der einzelne Block, der den `{#latest}` Anker trägt).

- **Bearbeiten Sie** **frühere Versionshinweise**—keinen `+++Notes from YYYY.MM.DD+++` ausblendbaren Block—oder **irgendeinen** älteren `##` monatlichen Abschnitt, der nicht mehr `{#latest}` hat, selbst wenn das Thema in Beziehung zu stehen scheint, ein Link falsch aussieht oder eine Kopie dort dupliziert oder veraltet erscheint.
- **Bereinigen Sie** vorherigen `###` Unterabschnitte, Aufzählungszeichen, Links oder Formulierungen außerhalb des aktuellen `{#latest}`-Blocks nur, wenn der Benutzer eine **explizite, separate** Anfrage sendet, die von dieser Qualifikation nicht abgedeckt wird.
- **Ausnahme:** [Spätestes Archivieren](#archive-previous-latest) beim Einführen eines **neuen** oberen `{#latest}`: **Verschieben** des gesamten vorherigen `{#latest}`-Abschnitts in einen **neuen**, der unter **früheren Versionshinweisen** wie unten beschrieben ausgeblendet werden kann. Während dieses Durchlaufs dürfen **nicht** neu schreiben oder zu **anderen, älteren** Archivblöcken hinzufügen.

Wenn neue Informationen in das Dokument gehören, platzieren Sie sie unter der aktuellen **`{#latest}`** Überschrift (oder archivieren Sie sie zuerst und fügen Sie sie dann nur unter der neuen `{#latest}` hinzu).

## Workflow-Checkliste

Arbeiten Sie in dieser Reihenfolge. Kopieren Sie die Checkliste und verfolgen Sie den Fortschritt bei mehrstufigen Bearbeitungen.

&#x200B;0. [ ] Wenn **Jira** und **Confluence** MCP verfügbar sind, führen Sie zuerst [consumer-release-sources](../consume-release-sources/SKILL.md) aus, um das Arbeitsticket, das Zeremonie-Wiki (GA- und Beta-Funktionsgruppen) und die KT-Seiten aufzunehmen. Wenn MCP nicht verfügbar ist, verwenden Sie eingefügte KT/Wiki-Inhalte und [reference.md](reference.md#internal-sources-kt-and-release-wikis)-Feldzuordnung.
1. [ ] Öffnen Sie `help/user-guide/release-notes.md` und lesen Sie den aktuellen `## YYYY.MM {#latest}`. Behandeln Sie **früheren Versionshinweise** als **schreibgeschützten**-Kontext, es sei denn, Sie führen den Archivierungsschritt in Schritt 2 aus.
2. [ ] Wenn Sie eine **neue** monatliche Version hinzufügen: archivieren Sie die aktuelle Version (siehe [Archivieren Sie die neueste Version](#archive-previous-latest)).
3. [ ] Fügen Sie **Abschnitt** der obersten `## YYYY.MM {#latest}` hinzu oder bearbeiten Sie ihn (neuer Monat am Anfang der Veröffentlichungsliste).
4. [ ] Wenden Sie für jedes Element [Entscheidungsregeln](#decision-rules) an (Feature `###` vs. **Fehlerbehebungen und**, Beta-Badge oder nicht).
5. [ ] Fügen Sie Dokumentations-Links zum relevantesten Satz hinzu oder überprüfen Sie ihn (siehe [reference.md](reference.md#documentation-linking)).
6. [ ] Führen Sie [Qualitätsprüfungen](#quality-checks) vor dem Abschluss durch.
7. [ ] Beibehalten von [frontmatter](reference.md#frontmatter) auf der Seite, es sei denn, die Aufgabe aktualisiert ausdrücklich Metadaten.

## Entscheidungsregeln

Verwenden Sie diese Wenn/Dann-Regeln, damit Inhalte an der richtigen Stelle landen:

| If | THEN |
|----|------|
| Die Funktion ist neu und in Beta verfügbar | Fügen Sie die Beta-Badge-Zeile direkt unter der Überschrift `###` hinzu (siehe [beispiel.md](examples.md)). |
| Source-Material kennzeichnet den Artikel explizit als **Korrektur** oder **Verbesserung** | Lediglich mit `*` Kugeln unter `### Fixes and enhancements` legen. |
| Das Element ist eine neue Funktion oder Feature Story | Verwenden Sie einen `###` Funktionsabschnitt mit 1-3 Sätzen (nicht der Liste mit Fehlerbehebungen). |
| Sie sind sich nicht sicher, ob es sich um eine Korrektur oder eine Funktion handelt | Der Standardwert ist ein `###` Funktionsabschnitt, es sei denn, die Quelle sagt eindeutig „Beheben/Verbessern“. |

**Regel für den Abschnitt „Fehlerbehebungen“** Fügen Sie keine Aufzählungszeichen zu **Fehlerbehebungen und** hinzu, es sei denn, die Quelle ist explizit als Fehlerbehebung oder Verbesserung gekennzeichnet.

## Archivieren Sie die letzte

Bei der Einführung eines neuen `## YYYY.MM {#latest}`:

1. Schneiden Sie den gesamten vorherigen `## YYYY.MM {#latest}`-Abschnitt aus (von seiner Überschrift bis zum Ende des Inhalts dieser Version, vor dem nächsten `##` oder **früheren Versionshinweisen**).
2. Fügen Sie sie in **frühere Versionshinweise** innerhalb eines **neuen** ausblendbaren Blocks ein.
3. Ersetzen Sie die alte Überschrift durch: `+++Notes from YYYY.MM.DD+++` (verwenden Sie das tatsächliche Veröffentlichungsdatum; Format wie in den vorhandenen Hinweisen in der Datei).
4. Entfernen Sie `{#latest}` aus der archivierten Überschrift. Der neue obere Abschnitt ist der einzige mit `{#latest}`.
5. Die chronologische Reihenfolge innerhalb von **früheren Versionshinweisen** beibehalten (neueste archivierte Blöcke nach oben, sofern die Datei nicht bereits eine andere Reihenfolge verwendet - **mit der vorhandenen Datei**).

Bearbeiten **&#x200B;**&#x200B;während der Durchführung dieses Archivs nicht den **(bereits**) `+++Notes from …+++` - fügen Sie nur den neu archivierten Block ein und behalten Sie die älteren Archive unverändert bei.

## Erforderliche Struktur

### Seitentitel und Einführung

Verwenden Sie nach frontmatter:

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

Wenn die Datei bereits einen etwas anderen Einführungssatz verwendet (z. B. „liefert“ anstelle von „Details„), bleiben Sie konsistent mit dem Rest der Seite.

### Neueste Versionshinweise

- Format: `## YYYY.MM {#latest}` für den neuesten Veröffentlichungsblock.
- Nur ein `{#latest}` auf der Seite.

### Funktionsabschnitte

- Verwenden Sie `###` für die wichtigsten Funktionskategorien.
- Präsenz, 1-3 Sätze, klar, was/warum und Benutzeraktionen waren hilfreich.
- Produktnamen: `[!DNL Create]`, `[!DNL Content]`, `[!DNL Insights]` usw.
- Benutzeroberfläche: `[!UICONTROL Control Name]` sofern zutreffend.
- Hervorhebung: `_italics_` für Benutzeroberflächenbereiche/-abschnitte; `**bold**` für Schlüsselbegriffe sparsam.

### Beta-Badge

Verwenden Sie genau:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### Links zur Dokumentation

- Muster: `[link text](/help/user-guide/section/page.md#anchor)`
- Anker bevorzugen; Link zur Wortgruppe der Benutzer, nicht „hier klicken“.

### Fehlerbehebungen und Verbesserungen

- Aufzählungslinien verwenden `*`.
- Nur Artikel mit der expliziten Beschriftung „Korrigieren/Verbessern“ im Quellmaterial.
- Gleiche Konventionen für Links und Terminologie wie für Funktionen.

## Verbotene Inhalte

- Schließen **nicht** Jira-Schlüssel, interne Problemnummern, interne URLs oder Unternehmens-Wiki-Links in veröffentlichten Versionshinweisen ein.
- Geben **&#x200B;**&#x200B;Dokumente, Tickets oder interne Tools zum Wissenstransfer nicht als Nachweis an. Fassen Sie nur benutzerfreundliche Ergebnisse zusammen.
- Duplizieren **&#x200B;**&#x200B;nicht `{#latest}` in mehreren Abschnitten.

## Qualitätskontrollen

Vor Abschluss der Aufgabe:

- [ ] **Umfang:** Nur der `## … {#latest}` wurde hinzugefügt oder bearbeitet; **frühere Versionshinweise** und ältere Monatsabschnitte wurden nicht geändert, außer dem [Archivieren des vorherigen &#x200B;](#archive-previous-latest) Ausschneiden/Einfügen des vorherigen `{#latest}` in einen **neuen** Archivblock.
- [ ] Alle neuen oder geänderten relativen Links werden nach Möglichkeit in echte Pfade unter `help/` aufgelöst.
- [ ] Beta-Funktionen enthalten bei Bedarf das Beta-Badge-Snippet .
- [ ] Terminologie entspricht den vorhandenen Versionshinweisen (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] Scannen Sie den Entwurf nach versehentlichen internen IDs (`[A-Z]+-\d+`), Wiki-URLs oder der Sprache „siehe Jira“; entfernen Sie sie.
- [ ] **Korrekturen und Verbesserungen** enthält nur explizit beschriftete Korrekturen/Verbesserungen.
- [ ] letzte Abschnitt wurde korrekt archiviert, wenn ein neuer Monat hinzugefügt wurde.

## Inhaltsquellen (Zusammenfassung)

Wenn **Jira/Confluence MCP** verfügbar ist, beginnen Sie mit [consumer-release-sources](../consume-release-sources/SKILL.md) (Zeremonie-Wiki → KT-Seiten → strukturierter Übergabe). Ordnen Sie andernfalls eingefügte Wiki-Felder für den Wissenstransfer oder die Freigabe zu, wie in [reference.md](reference.md#internal-sources-kt-and-release-wikis) beschrieben. Die bereitgestellte Seite muss als eigenständige Benutzerdokumentation lesen.

## Optional: Neue Unterabschnitte polieren

Nachdem Sie neue `###` unter `{#latest}` hinzugefügt haben, führen Sie [Polnische Versionshinweise](../polish-release-notes/SKILL.md) für einen Copyeditor-ähnlichen Pass (Benefit-Forward-Ton, **2-3 Sätze pro Absatz**, keine prozeduralen Anleitungen) **only** auf diesen **neuen** Unterabschnitten aus - **nicht** auf früheren Versionshinweisen oder bereits vorhandenen Text, es sei denn, dies wird ausdrücklich angefordert.

## Weitere Ressourcen

- [Examples.md](examples.md) — Einfügebereite Beispiele (Funktionen, Fehlerbehebungen, Archivierungsblock).
- [reference.md](reference.md) - Frontend-Notizen, Dokumentenpfade, Verknüpfungsstrategie.
- [Polnische Versionshinweise](../polish-release-notes/SKILL.md) — optionale redaktionelle Weitergabe neu hinzugefügter `###` unter `{#latest}`.
