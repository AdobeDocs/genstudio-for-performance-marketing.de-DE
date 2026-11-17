---
title: Anzeigennamen generieren
description: Erfahren Sie, wie Sie Namensvorlagen konfigurieren, konsistente Anzeigenamen generieren und Namen überprüfen oder anpassen können, bevor Sie Anzeigen an Ihre unterstützten Aktivierungsplattformen senden.
role: User
source-git-commit: 6db986fefd199181e568e5fbc7a3b23554e5e70d
workflow-type: tm+mt
source-wordcount: '1684'
ht-degree: 1%
---

# Anzeigennamen generieren

Die automatisierte Anzeigenbenennung in [!DNL GenStudio for Performance Marketing] hilft Ihnen bei der Aktivierung von Anzeigen, die Namenskonventionen Ihres Unternehmens einzuhalten. Konsistente Namen unterstützen Leistungsberichte, Attribution und die Abstimmung der Ausgaben.

Eine Benennungsvorlage definiert die Teile eines Anzeigenamens und ihre Reihenfolge. Zu den Beispielteilen gehören das Produkt, die Kampagne und der Markt. Um eine Vorlage zu erstellen, laden Sie eine Excel-Datei hoch, die die Namenskonvention Ihres Unternehmens beschreibt.

Verwenden Sie die Vorlage, um Namen aus Informationen zu jedem Erlebnis zu generieren, z. B. zu seinem Produkt oder seiner Kampagne. Überprüfen und korrigieren Sie die Ergebnisse, bevor Sie Ihre Anzeigen senden. Die endgültigen Namen werden als Anzeigenamen an jede Zielplattform gesendet.

## Voraussetzungen

Sie müssen eine Vorlage nur einmal einrichten. Wenn Ihrem aktuellen Projekt bereits eine Vorlage zugewiesen ist, navigieren Sie direkt zu [Namen für eine Aktivierung generieren](#generate-names-for-an-activation).

Erstellen Sie andernfalls eine Vorlage und bitten Sie einen System Manager, sie [Ihren Plattformen zuzuweisen](#assign-a-template-to-platforms). Jedes Projekt kann eine andere Standardvorlage für dieselbe Plattform haben.

Bereiten Sie für die Vorlageneinrichtung eine Excel-Datei mit höchstens 3 MB und nur einem Blatt vor. CSV-Dateien werden nicht unterstützt. Beschreiben Sie die Namenskonvention für einzelne Anzeigen, nicht für Kampagnen oder Anzeigengruppen.

Listen Sie die Felder in der erforderlichen Reihenfolge auf. Geben Sie für jedes Feld die zulässigen Werte, die entsprechenden Codes und Anweisungen zur Auswahl eines Werts an. Beispielsweise verwendet die Option `Image` für das Feld `format` den im Namen `IMG` Code.

Laden Sie für eine Beispielstruktur das Beispiel [WKND Meta Naming Convention (Excel) herunter](assets/wknd-meta-naming-convention.xlsx). Die Datei definiert Felder und Beispielwerte für Produkt, Kampagne, Markt und andere Teile eines Anzeigenamens.

Ersetzen Sie die Beispielwerte und Regeln durch die Konvention Ihres Unternehmens, bevor Sie die Datei für Ihre eigenen Aktivierungen verwenden. Die Plattformwerte des Beispiels veranschaulichen Namensoptionen, keine Liste unterstützter Aktivierungsziele.

## Benennungsvorlage erstellen

Erstellen Sie eine Vorlage aus Ihrer vorhandenen Namenskonventionsdatei und überprüfen Sie dann die extrahierte Struktur, bevor Sie sie verwenden.

1. Öffnen Sie das Projekt, in dem Sie die Vorlage verwenden möchten.
1. Navigieren Sie zu **[!UICONTROL Mehr]** > **[!UICONTROL Einstellungen]**.
1. Wählen **[!UICONTROL Einrichten]** neben **[!UICONTROL Anzeigenamenvorlage]** aus.

   Wenn bereits Vorlagen vorhanden sind, öffnen Sie **[!UICONTROL Anzeigenamenvorlage]** und wählen Sie dann **[!UICONTROL Vorlage erstellen]** aus.

1. Wählen **[!UICONTROL Datei auswählen]** im Dialogfeld **[!UICONTROL Datei hochladen]**.
1. Wählen Sie Ihre Excel-Datei.

   Alternativ können Sie die Datei in den Upload-Bereich ziehen. Während **[!UICONTROL Arbeitsblatt analysieren…]** angezeigt wird, werden die Felder und Werte Ihrer Vorlage zugeordnet. Warten Sie einige Minuten, bis die Analyse abgeschlossen ist.

1. Überprüfen Sie die Felder, zulässigen Werte und **[!UICONTROL Anzeigenamenvorschau]**.

   Die Vorschau verwendet Beispielwerte, nicht die Details einer bestimmten Anzeige.

1. Wählen Sie **[!UICONTROL Speichern]** aus.

Dateien mit mehr als 3 MB, nicht unterstützte Dateitypen und leere Dateien zeigen einen Fehler an, ohne vorhandene Vorlagen oder Plattformzuweisungen zu ändern.

## Anpassen einer Vorlage

Bearbeiten Sie eine gespeicherte Vorlage, um ihren Namen, ihre Felder, ihr Trennzeichen oder ihre Regeln anzupassen.

1. Navigieren Sie zu **[!UICONTROL Mehr]** > **[!UICONTROL Einstellungen]** > **[!UICONTROL Anzeigenamenvorlage]**.
1. Öffnen Sie das Dreipunkt-Menü neben Ihrer Vorlage.
1. Wählen Sie **[!UICONTROL Bearbeiten]** aus.
1. Um die Vorlage umzubenennen, klicken Sie auf das Stiftsymbol neben dem Titel.
1. Setzen Sie **[!UICONTROL Feldtrennzeichen]** auf das Zeichen, das die Teile des Namens trennt, z. B. einen Unterstrich (`_`).
1. Ziehen Sie die Felder in die gewünschte Reihenfolge.

   Verwenden Sie **[!UICONTROL Feld hinzufügen]** oder das Papierkorbsymbol eines Felds, wenn Sie ändern müssen, welche Felder enthalten sind.

1. Um die Einstellungen eines Felds zu öffnen, klicken Sie auf sein Stiftsymbol.
1. Überprüfen Sie **[!UICONTROL Typ]** und **[!UICONTROL Name]** im Dialogfeld **[!UICONTROL Feld bearbeiten]**.

   Verwenden Sie **[!UICONTROL Dropdown]** für ein Feld mit vordefinierten Auswahlmöglichkeiten oder **[!UICONTROL Freier Text]** für einen von Ihnen eingegebenen Wert.

1. Überprüfen Sie für ein Dropdown-Feld **[!UICONTROL Optionen]** und **[!UICONTROL Code]**.

   **[!UICONTROL options]** enthält die lesbaren Auswahlmöglichkeiten. **[!UICONTROL Code]** enthält die entsprechenden Werte, die im Anzeigenamen verwendet werden. Beispielsweise verwendet die Option `Image` die Code-`IMG`.

   Um eine Auswahl hinzuzufügen, wählen Sie **[!UICONTROL Option hinzufügen]** aus. Um eine Auswahl zu entfernen, klicken Sie auf das entsprechende Minussymbol. Doppelte Werte in einem Feld sind nicht zulässig.

1. Geben Sie alle **[!UICONTROL Feldregeln]** ein, die zum Auswählen oder Formatieren des Feldwerts erforderlich sind.

   Geben Sie für das `creativeVersion`-Freitextfeld diese Beispielregel ein: `Use the experience name as a starting value, with spaces removed.`

1. Wählen **[!UICONTROL im]** Feld die Option „Speichern“ aus.

   Wiederholen Sie die Feldüberprüfung für alle anderen Felder, die geändert werden müssen.

1. Geben Sie alle **[!UICONTROL Vorlagenregeln]** ein, die für den gesamten Namen gelten.

   Geben Sie beispielsweise `Remove spaces from Product and Campaign values.` ein

1. Wählen **[!UICONTROL oben]** der Seite „Speichern“ aus.

Die Vorschau spiegelt die aktualisierte Feldreihenfolge und das Trennzeichen wider. Öffnen Sie die Vorlage erneut, um Ihre gespeicherten Änderungen zu überprüfen.

Der Feldeditor zeigt, wie lesbare Optionen den Codes zugeordnet werden, die in generierten Namen enthalten sind:

![Bearbeiten eines Felddialogfelds mit den Formatoptionen „Bild“, „Video“, „Karussell“ und &quot;HTML5“ sowie den entsprechenden Codes.](images/ad-name-field-options-codes.png)

## Zuweisen einer Vorlage zu Plattformen

System Manager legen die Standardvorlage für jede Plattform innerhalb eines Projekts fest. Wenn Sie kein System Manager sind, bitten Sie einen, dieses Verfahren abzuschließen.

1. Öffnen Sie das Projekt, dessen Plattform-Standardeinstellungen Sie festlegen möchten.
1. Navigieren Sie zu **[!UICONTROL Mehr]** > **[!UICONTROL Einstellungen]** > **[!UICONTROL Anzeigenamenvorlage]**.
1. Öffnen Sie das Dreipunkt-Menü neben Ihrer Vorlage.
1. Wählen Sie **[!UICONTROL Bearbeiten]** aus.
1. Wählen Sie unten im Editor unter **[!UICONTROL Bevorzugte Plattformen]** eine oder mehrere Plattformen aus.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

Jede Plattform verfügt über eine Standardvorlage pro Projekt. Sie können dieselbe Vorlage mehreren Plattformen zuweisen.

Vorlagen stehen zur Anzeige und Bearbeitung in verschiedenen Projekten zur Verfügung. Sie können Platform-Zuweisungen jedoch nur in Ihrem aktuellen Projekt ändern.

Wenn Sie den Standard einer Plattform ersetzen, wird weder die vorherige Vorlage gelöscht noch werden die Zuweisungen anderer Projekte geändert.

Das folgende Beispiel zeigt die Vorschau der Vorlage, die Reihenfolge der Felder, die Regeln und **[!UICONTROL Bevorzugte Plattformen]** wobei Meta Ads ausgewählt ist:

![WKND-Vorlageneditor mit einem Unterstrichtrennzeichen, 12 Feldern mit Anzeigenamen, Vorlagenregeln und Meta Ads, die unter „Bevorzugte Plattformen“ ausgewählt wurden.](images/ad-name-template-editor.png)

## Generieren von Namen für eine Aktivierung

Bereiten Sie die Aktivierung vor, bevor Sie Namen generieren. Die Metadaten der einzelnen Erlebnisse enthalten Informationen wie die Kampagne, das Produkt oder die Rolle. Vergewissern Sie sich, dass die Metadaten die Werte enthalten, die Ihre Vorlage benötigt. Siehe [Aktivierungs-Workflow](create-activation.md) für Hilfe bei der Vorbereitung einer Aktivierung.

1. Öffnen **[!UICONTROL Aktivieren]** im gewünschten Projekt.
1. Hinzufügen von Erlebnissen zu einer Aktivierung.
1. Schließen Sie die Plattform-Einrichtung und alle erforderlichen Informationen ab, einschließlich Kopie, call-to-action (CTA) und Website-URL.
1. Vergewissern Sie sich, dass die Erlebnisse über die Metadaten verfügen, die von Ihrer Namenskonvention benötigt werden.
1. Wählen **[!UICONTROL Anzeigenamen generieren]** über der Aktivierungstabelle aus.

   Warten Sie, bis **[!UICONTROL Generating Ad Names]** abgeschlossen ist, bevor Sie die Ergebnisse überprüfen.

1. Überprüfen Sie die Spalte **[!UICONTROL Anzeigename]**.

Die Generierung gilt für alle Anzeigen auf Plattformen mit einer zugewiesenen Vorlage, mit Ausnahme von Anzeigen mit &quot;[ Namensüberschreibungen](#use-a-custom-ad-name). Beim Öffnen der Tabelle werden die Namen nicht automatisch generiert.

Anfangs verwendet jede Anzeige den Namen ihres Erlebnisses. Wenn einer Plattform keine Vorlage zugewiesen ist, bleiben die Namen bei der Generierung unverändert. Bearbeiten Sie diese Namen nach Bedarf manuell.

Wenn keine Plattformen Vorlagen zugewiesen haben, werden keine Namen generiert.

## Korrigieren eines einzelnen Anzeigenamens

Überprüfen Sie die generierten Namen, bevor Sie Ihre Anzeigen senden. Fehlende Werte werden als hervorgehobene Platzhalter für Felder angezeigt, z. B. `[market]`, und die betroffenen Anzeigen zeigen &quot;**[!UICONTROL Aufmerksamkeit erforderlich]**.

Um Namen zu finden, die korrigiert werden müssen, suchen Sie in der Aktivierungstabelle nach hervorgehobenen Platzhaltern und **[!UICONTROL Erfordert]**) Status:

![Aktivierungstabelle mit einer Warnung zu fehlenden Werten, hervorgehobenen Market-Platzhaltern in der Spalte Anzeigename und Erfordert einen Wartungsstatus.](images/ad-names-missing-values.png)

1. Wählen Sie die Zeile der Anzeige in der Aktivierungstabelle aus.
1. Wählen Sie **[!UICONTROL Anzeigenamen bearbeiten]** aus.
1. Aktualisieren Sie die entsprechenden Dropdown-Listen oder Textfelder.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

Wenn `market` beispielsweise keinen Wert hat, geben Sie den entsprechenden Markt ein, der im Namen `[market]` ersetzen soll, oder wählen Sie ihn aus.

Überprüfen Sie den aktualisierten Namen entsprechend Ihrer Konvention.

## Mögliche doppelte Namen auflösen

Identische Anzeigenamen auf derselben Plattform werden als potenzielle Duplikate gekennzeichnet.

1. Wählen Sie eine der betroffenen Anzeigen aus.
1. Wählen Sie **[!UICONTROL Anzeigenamen bearbeiten]** aus.
1. Ändern Sie den Namen, sodass die beiden Namen unterschiedlich sind.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

Der Warnhinweis „potenzielle Duplikate“ wird gelöscht, nachdem die Namen geändert wurden.

## Mehrere Anzeigennamen bearbeiten {#edit-several-ad-names-at-once}

Verwenden Sie die Massenbearbeitung, um eine gemeinsame Korrektur anzuwenden und gleichzeitig Werte beizubehalten, die sich zwischen Anzeigen unterscheiden.

1. Wählen Sie die Anzeigen mithilfe ihrer Zeilenkontrollkästchen aus.
1. Wählen Sie **[!UICONTROL Anzeigenamen bearbeiten]** in der Auswahlsymbolleiste aus.
1. Nur Felder ändern, die in allen ausgewählten Anzeigen denselben Wert benötigen.

   **[!UICONTROL Gemischte Werte]** bedeutet, dass die ausgewählten Anzeigen derzeit unterschiedliche Werte für ein Feld aufweisen. Lassen Sie dieses Feld unberührt, um den Wert jeder Anzeige zu erhalten.

1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Überprüfen Sie die aktualisierten Namen auf Genauigkeit und mögliche Duplikate.

Nur ausgewählte Anzeigen werden aktualisiert. Nicht ausgewählte Anzeigen bleiben unverändert.

Der Bulk Editor zeigt **[!UICONTROL Gemischte Werte]** für Felder an, die sich in den ausgewählten Anzeigen unterscheiden:

![Detail des Dialogfelds „4 Anzeigenamen bearbeiten“ mit gemischten Werten für Produkt, Kampagne, CreativeVersion und Persona.](images/ad-names-bulk-edit.png)

Wenn Sie beispielsweise nur die Rolle von `OutdoorBeginners` in `Adventurers` ändern, bleiben die verschiedenen Produkte erhalten. Diese gekürzten Namen veranschaulichen die Änderung:

| Vorher | Nachher |
| --- | --- |
| `WKND_TrailBag_OutdoorBeginners` | `WKND_TrailBag_Adventurers` |
| `WKND_RiosShirt_OutdoorBeginners` | `WKND_RiosShirt_Adventurers` |

## Verwenden eines benutzerdefinierten Anzeigenamens

Verwenden Sie eine Überschreibung, um den gesamten generierten Namen durch einen benutzerdefinierten Namen zu ersetzen, anstatt einzelne Vorlagenfelder zu bearbeiten.

1. Wählen Sie die Zeile der Anzeige aus.
1. Wählen Sie **[!UICONTROL Anzeigenamen bearbeiten]** aus.
1. Aktivieren Sie **[!UICONTROL Anzeigenamen überschreiben]**.
1. Geben Sie den benutzerdefinierten Namen ein.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

Der benutzerdefinierte Name bleibt unverändert, wenn Sie erneut Namen generieren.

Wenn die Überschreibung aktiviert ist, bearbeiten Sie den vollständigen Namen anstelle der einzelnen Vorlagenfelder:

![Das Dialogfeld „Anzeigenamen bearbeiten“ mit aktiviertem „Anzeigenamen überschreiben“ und dem vollständigen WKND-Anzeigenamen, der zur Bearbeitung verfügbar ist.](images/ad-name-override.png)

Gehen Sie wie folgt vor, um zur vorlagenbasierten Benennung zurückzukehren:

1. Öffnen Sie **[!UICONTROL Anzeigenamen bearbeiten]** für die Anzeige.
1. Deaktivieren Sie **[!UICONTROL Anzeigenamen überschreiben]**.
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen **[!UICONTROL Anzeigenamen generieren]** über der Aktivierungstabelle aus.

Diese Aktion generiert auch Namen für andere Anzeigen in der Tabelle, denen eine Vorlage zugewiesen ist und die keinen benutzerdefinierten Namen überschreiben.

## Auf Vorlagenänderungen reagieren

Beim Bearbeiten einer Aktivierungstabelle wird eine Warnung angezeigt, wenn eine von ihr verwendete Vorlage geändert wurde oder gelöscht wurde.

Wenn sich die Vorlage geändert hat, überprüfen Sie die aktualisierte Vorlage, bevor Sie Namen neu generieren. Wählen Sie **[!UICONTROL Anzeigenamen generieren]** aus, um sie anzuwenden.

Wenn die Vorlage gelöscht wurde oder Sie einen Ersatz benötigen, führen Sie die folgenden Schritte aus:

1. Bitten Sie einen Systemmanager, der betroffenen Plattform im selben Projekt eine Ersatzvorlage zuzuweisen.
1. Zurück zur Aktivierungstabelle.
1. Wählen Sie **[!UICONTROL Anzeigenamen generieren]** aus.
1. Überprüfen Sie die aktualisierten Namen.

Namen mit aktivierten Überschreibungen bleiben während der Regenerierung unverändert.

## Anzeigen an Plattformen senden

Überprüfen Sie Ihre endgültigen Namen und beheben Sie ungelöste Felder, potenzielle Duplikate und andere **[!UICONTROL Aufmerksamkeit erforderlich]** Probleme, bevor Sie Anzeigen senden.

Wenn die Aktivierung fertig ist, wählen Sie **[!UICONTROL An Plattformen senden]** aus.

[!DNL GenStudio for Performance Marketing] sendet den endgültigen Namen jeder Anzeige als Anzeigename an die Zielplattform. Der gesendete Name enthält alle Änderungen an Vorlagenfeldern oder Überschreibungen benutzerdefinierter Namen. Die Anzeigenamen auf der Plattform stimmen genau mit den endgültigen Namen überein, die Sie geprüft haben.

Bei Anzeigezielen wie Innovid werden Namen als kreative Namen angezeigt.
