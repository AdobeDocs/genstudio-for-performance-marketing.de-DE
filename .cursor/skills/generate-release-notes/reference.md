---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# Referenz: Versionshinweise zum Authoring

## Titelei

Die Live-Seite [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md) enthält Experience League-Metadaten, die über einen Mindestsatz hinausgehen (z. B. `TQID`, `product_v2`, `feature_v2`, Taxonomie-IDs).

**Regeln:**

- Beim Bearbeiten des Inhalts **Versionshinweisen (**) **vorhandene** und Werte beibehalten, es sei denn, die Aufgabe fordert ausdrücklich zur Änderung von Metadaten auf.
- Entfernen Sie keine Taxonomie- oder Produktmetadaten, um sie mit einer kürzeren Vorlage abzugleichen.
- Zu den erforderlichen Konzepten für ExL-Seiten gehören im Allgemeinen `title`, `description` und `role`. Befolgen Sie für neue Seiten die [Anleitungen ](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata) Experience League-Metadaten.

## Interne Quellen (KT und Release-Wikis)

Verwenden Sie diese Felder **nur beim Entwerfen**. Die veröffentlichten Versionshinweise dürfen keine internen Dokumente referenzieren.

### Dokumente zum Wissenstransfer (KT)

Extrahieren aus:

| Feld | Verwenden |
|-------|-----|
| Beschreibung | Erläuterung der Hauptfunktionen |
| Höhenruderneigung | Wertvorschlag |
| Bereitgestellte Funktionen | Konkretes Verhalten |
| Problembeschreibung | Problempunkt des Benutzers |
| Veröffentlichungstyp und Datum | Timing |

### Wiki-Seiten veröffentlichen

Gruppieren und Umfang nach:

| Feld | Verwenden |
|-------|-----|
| Veröffentlichungsdatum (Version korrigieren) | Gleiches Datum → gleichem Batch mit Versionshinweisen |
| Initiative | Nur Kontext; nicht intern im öffentlichen Text verknüpfen |
| PM stellt die Funktion mithilfe von KT dar | Signale mit tieferen KT-Details können vorhanden sein |

**Bereichsregel:** Elemente mit demselben Veröffentlichungsdatum (Fix-Version) gehören in denselben monatlichen Veröffentlichungsblock.

## Verknüpfung von Dokumentationen

- Link zum **relevantesten** Satz (z. B. Link „Nicht unterstützte Bild- und Video-Assets“ zum Abschnitt „Anzeigenformate„).
- Ziehen Sie `#anchor` Links in den rechten Unterabschnitt vor.
- Übersichtsseiten sind akzeptabel, wenn kein tieferer Anker vorhanden ist.

## Allgemeine Dokumentationspfade

| Bereich | Pfadpräfix |
|------|-------------|
| Erstellen | `/help/user-guide/create/` |
| Inhalt | `/help/user-guide/content/` |
| Aktivierung | `/help/user-guide/activation/` |
| Genehmigungen | `/help/user-guide/approvals/` |
| Insights | `/help/user-guide/insights/` |
| Richtlinien | `/help/user-guide/guidelines/` |
| Vorlagen | `/help/user-guide/templates/` |
| Kampagnen | `/help/user-guide/campaigns/` |
| Erweiterbarkeit | `/help/extensibility/` |
