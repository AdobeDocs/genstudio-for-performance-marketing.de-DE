---
name: polish-release-notes
description: ""
notes: refines only newly added
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---


# Versionshinweise zu GenStudio in Polen

**Kanonische Zieldatei:** [help/user-guide/release-notes.md](../../../help/user-guide/release-notes.md)

**Examples:** [Examples.md](examples.md)

**Drafting-Workflow (Upstream):** [generate-release-notes](../generate-release-notes/SKILL.md)

## Umfang (erforderlich)

Nur **polnische**, die der Benutzer als &quot;**hinzugefügt“** dieser Runde kennzeichnet:

- **In Datei:** `###` Unterabschnitte unter der einzelnen Überschrift `## YYYY.MM {#latest}` in `help/user-guide/release-notes.md`.
- **Bearbeiten Sie** Seitentitel, den Einführungsabsatz, die Frontanschrift oder Text unter **Frühere Versionshinweise** (ausblendbare `+++`).
- **Bearbeiten Sie** vorherigen `##` monatlichen Blöcke oder bereits vorhandenen `###` im selben `{#latest}`-Abschnitt, es sei denn, der Benutzer **ausdrücklich**.
- Wenn unklar ist, welche `###` neu sind, **Sie** oder verwenden Sie **git diff** / edit context, bevor Sie die Prosa ändern.
- **Eingefügter Inhalt:** Der Benutzer fügt Markdown nur dann ein, wenn er bestätigt, dass er mit diesen **gleichen** neuen Unterabschnitten übereinstimmt (nicht verwandte Paste als im Umfang enthalten behandeln).

Unterschiede beibehalten **minimal**: Nur Formulierungs- und Absatzumbrüche - keine Drive-by-Refaktoren an anderer Stelle in der Datei.

## Stimme und Ton

- Schreiben Sie als **Werbetexter** für Produktversionshinweise: **kurz**, **überschaubar** und **angeregt** über **neuen Wert** - führen Sie mit Ergebnissen und „was für Sie dabei ist“, verwenden Sie starke Verben und eine klare Leistungssprache.
- **Bleiben Sie genau:** keine Ansprüche, die über das hinausgehen, was die Funktion bietet; stimmen Sie mit dem Experience League / Adobe-Ton überein (zuversichtlich und klar, nicht sensationalistisch).
- **Erregung generieren** mit **spezifischen** Vorteilen und Deltas (was Marketing-Experten jetzt tun können, welche Reibungen beseitigt werden) - nicht leerer Hype oder unbegründete Superlative.

## Absatzregeln

- Jeder Absatz: **2-3 Sätze**. **Nie mehr als drei Sätze** in einem Absatz - wenn Sie mehr benötigen, beginnen Sie einen **neuen Absatz**.
- Optional: Wenn ein Absatz immer noch länger als **~3 Zeilen**, teilen Sie die gerenderten Dokumente mit der typischen Zeilenlänge weiter auf.

## Nicht hinzufügen

- **Prozedurale Anleitung** Inhalte: nummerierte Schritte, „Klicken Sie **[!UICONTROL …]** dann…“, exemplarische Vorgehensweisen für die vollständige Benutzeroberfläche oder Tutorial-Formulierungen. In den Versionshinweisen **Sie, was** und **warum es wichtig ist** und nicht praktische Lektionen.
- Inhalte, die gegen [Verbotene Inhalte](../generate-release-notes/SKILL.md#prohibited-content) auf der generierten Qualifikation verstoßen (keine Jira-Schlüssel, nur interne URLs, Wiki-as-Proof usw.).

## Beibehalten (nicht abstreifen oder strukturell neu schreiben)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]` und andere ExL-Shortcodes.
- Vorhandene **relative** Dokumentations-Links und Ankermuster: `[phrase](/help/...)` auf aussagekräftigen Ankertext.
- Das Beta-Badge blockiert genau wie in [Beispielen für Versionshinweise generieren](../generate-release-notes/examples.md).

## Workflow-Checkliste

1. [ ] Bestätigen **welche** `###` unter `## … {#latest}` im Umfang enthalten sind (neu in dieser Runde).
2. [ ] Für jede im Umfang enthaltene `###` straffen Sie die Kopien [Sprach- und &#x200B;](#voice-and-tone) und [Absatzregeln](#paragraph-rules).
3. [ ] Entfernen oder kürzen Sie **Anleitungen** Behalten Sie **Benutzerergebnisse** bei.
4. [ ] Überprüfen Sie, ob Links und Shortcodes weiterhin gültig sind. Führen Sie einen Schnellscan für interne IDs oder gesperrte Muster gemäß [Qualitätsprüfungen](#quality-checks) durch.

## Qualitätskontrollen

- [ ] Nur die vereinbarten **neu** `###` Blöcke unter `{#latest}` geändert; Archive und ältere Monate unberührt.
- [ ] Keine neuen IDs im Jira-Stil, keine internen Wiki-URLs oder „Ticket anzeigen“-Sprache.
- [ ] Absätze sind **2-3 Sätze** jeweils (maximal drei Sätze pro Absatz).
- [ ] Copy bleibt **sachlich** und mit der beschriebenen Funktion abgestimmt.

## Weitere Ressourcen

- [Examples.md](examples.md) — before/after patterns.
- [generate-release-notes](../generate-release-notes/SKILL.md) — Entwurf, Archivierung, Beta-Abzeichen, Verknüpfung.
