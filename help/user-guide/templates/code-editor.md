---
title: Vorlagen-Code-Editor
description: Erfahren Sie, wie Sie den Vorlagen-Code-Editor in GenStudio for Performance Marketing verwenden.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 1%

---

# Vorlagen-Code-Editor

Der Vorlagen-Code-Editor soll Ihnen dabei helfen, Ihre Vorlage zu überprüfen und zu verfeinern, damit sie beim Generieren neuer Erlebnisse mit GenStudio for Performance Marketing optimal verwendet werden kann. Der Editor unterstützt die Handlebars-Syntax, die Platzhalter in der Vorlage verwendet, um anzugeben, wo GenStudio for Performance Marketing Inhalte für Sie generieren soll.

>[!TIP]
>
>Bereiten Sie Ihre Vorlage vor dem Hochladen des HTML[!DNL Content]Vorlagencodes in der Ansicht _Vorlagen_ vor, indem Sie die in der Anleitung [Anpassen von Vorlagen](customize-template.md) definierten Platzhalter für Inhalte einfügen.

## Überprüfen erkannter Felder

Der Bereich _[!UICONTROL Erkannte Felder überprüfen]_ zeigt eine Liste von Feldern an, die GenStudio for Performance Marketing in Ihrer Vorlage erkennt. Überprüfen Sie die Liste und Sie können durch den HTML-Code scrollen, um die Bildung Ihrer Vorlage anzuzeigen.

![Code-Editor-Ansicht](/help/assets/template-detected-fields.png "Überprüfung erkannter Felder"){width="600"}

Wenn Sie feststellen, dass ein Feld in der Liste fehlt, durchsuchen Sie den Vorlagencode und suchen Sie nach dem Speicherort für das fehlende Feld. Fügen Sie den richtigen Platzhalter mithilfe der Handlebars-Syntax und eines [erkannten Feldnamens](/help/user-guide/templates/customize-template.md#recognized-field-names) ein. Verwenden Sie das Formular Suchen und Ersetzen unten im Code-Editor, um nach bestimmten Zeichenfolgen im Code zu suchen. (Windows `CTRL`+`F` oder macOS `CMD`+`F`)

## Anpassen der Rollen für eine Variable

Sie können Feldrollen für textbasierte Feldrollen (z. B. `headline`, `sub_headline`, `body`, `cta`, `on_image_text`, `custom`) während der Überprüfung der Vorlagenstruktur mit einem Dropdown-Menü auswählen und ändern. Die Feldrollenauswahl bleibt während der Vorlagenbearbeitung erhalten, sodass die Anpassungen nicht verloren gehen, was die Workflow-Effizienz verbessert.

>[!NOTE]
>
>Die Rollen von Bildvariablen können nicht angepasst werden.

![Mehrfachrollenfeldauswahl](/help/assets/multirole-dropdown-field.png "Mehrfachrollenfeldauswahl"){width="600"}

So weisen Sie einer Variablen eine Rolle zu:

1. Suchen Sie die Variable im Bereich _[!UICONTROL Erkannte Felder überprüfen]_. Diese Variablen werden automatisch erkannt.
2. Überprüfen Sie die den einzelnen Variablen zugewiesenen Rollen. Rollen werden automatisch zugewiesen, können jedoch über das Dropdown-Menü für jede Variable in der Vorlage angepasst werden.
3. Passen Sie eine Rolle an, indem Sie eine neue Rolle aus der Dropdown-Liste auswählen.
4. Klicken Sie auf **[!UICONTROL Weiter]**, um fortzufahren.

## Korrektur vornehmen

Wenn Ihre Vorlage Fehler enthält, wird möglicherweise eine `Template is invalid` mit einer kurzen Erläuterung des Problems angezeigt. Im folgenden Beispiel zeigt die Meldung an, dass das `_image` Feld nicht der in der Multi-Pod-Vorlage festgelegten Feldnamenskonvention entspricht. In der Meldung wird außerdem darauf hingewiesen, dass Sie den Feldnamen mit dem richtigen Präfix aktualisieren müssen. Suchen Sie das Feld `_image` im Vorlagen-Code-Editor und aktualisieren Sie den Namen wie empfohlen.

![Ungültige Vorlage korrigieren](/help/assets/animation/template-code-editor.gif){width="600"}

Der _[!UICONTROL Überprüfen erkannter Felder]_ wird aktualisiert und zeigt die von Ihnen vorgenommenen Änderungen an. Wenn Sie sich vergewissert haben, dass die Felder korrekt und vollständig sind, klicken Sie auf **[!UICONTROL Weiter]**, um mit dem [ (Hochladen der Vorlage) ](/help/user-guide/templates/use-templates.md#add-a-template).

## Häufige Probleme mit Vorlagen und Lösungen

| **Fehler** | **Beschreibung** | **Lösung** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Parsen fehlgeschlagen | Der Vorlageninhalt konnte nicht als gültige Handlebars geparst werden. | Überprüfen Sie Ihre Vorlage auf HTML- und Handlebars-Syntaxfehler und korrigieren Sie diese, um eine gültige Formatierung für [Inhalts-Platzhalter“ ](/help/user-guide/templates/customize-template.md#content-placeholders). |
| Gruppe nicht zugewiesen | Ein Bildfeld in einer E-Mail-Vorlage mit mehreren Gruppen ist keiner Gruppe zugewiesen. | Prüfen Sie, ob Abschnittspräfixe konsistent verwendet werden. Jeder [Abschnitt](/help/user-guide/templates/customize-template.md#sections-or-groups) kann nur einen Feldtyp (`headline`, `body`, `image` `cta`) verwenden. Weisen Sie das Feld `image` einer gültigen Gruppe in Ihrer Vorlage zu. |
| Bild fehlt | Ein erforderliches Bildfeld fehlt. | Für bestimmte Vorlagentypen ist genau ein `image` erforderlich, z. B. eine Meta-, Display- oder Banneranzeige. Fügen Sie das erforderliche `image` Feld zu Ihrer Vorlage hinzu. |
| Ungültige einzelne Gruppe | Die E-Mail-Vorlage enthält genau eine Gruppe, die ungültig ist. | Eine einfache E-Mail-Vorlage enthält einen einzigen Satz von Vorlagenelementen, für die keine Namenskonvention für Gruppen gemäß der Definition in [Abschnitte oder Gruppen](/help/user-guide/templates/customize-template.md#sections-or-groups) erforderlich ist. Passen Sie Ihre Vorlage so an, dass sie null Abschnitte enthält, indem Sie eine beliebige Gruppensyntax entfernen. |
| Keine Felder | Die Vorlage enthält keine Felder. | Fügen Sie [erkannte Feldnamen](/help/user-guide/templates/customize-template.md#recognized-field-names) mithilfe der Handlebars-Syntax zu Ihrer Vorlage hinzu, für die GenStudio for Performance Marketing einen bestimmten Inhaltstyp generieren muss. |
| Erforderliche Eigenschaften fehlen | Einige erforderliche Metadateneigenschaften fehlen. | Jeder Vorlagentyp verfügt über Anforderungen und Einschränkungen, die auf den Kanalrichtlinien basieren. Meta erfordert beispielsweise ein Seitenverhältnis, und für Display-Anzeigen sind Dimensionen erforderlich. [Befolgen Sie die Richtlinien für kanalspezifische Vorlagen](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Verwendeter reservierter Name | Ein unzulässiger oder reservierter Feldname wird verwendet. | Bestimmte [Feldnamen](/help/user-guide/templates/customize-template.md#recognized-field-names) wie `subject` oder `introductory_text` sind reserviert. Umbenennen von Feldern, die reservierte oder verbotene Namen verwenden. |
| Zu viele Felder | Die Anzahl der Felder überschreitet die globale Beschränkung von 20. | Entfernen Sie unnötige Felder, um sicherzustellen, dass die Gesamtanzahl 20 nicht überschreitet. |
| Zu viele Gruppen | Die Anzahl der Gruppen überschreitet das zulässige Maximum des Kanals. | Meta-, Display- und LinkedIn-Vorlagen lassen mehrere Abschnitte nicht zu. E-Mail erfordert beim Definieren von zwei oder drei Abschnitten eine Gruppenbenennung. Verringern Sie die Anzahl der Gruppen in Ihrer Vorlage, um die [Anforderungen des Kanals“ zu ](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Nicht unterstütztes Feld | Die Vorlage verwendet ein Feld, das der Kanal nicht unterstützt. | Ersetzen oder entfernen Sie nicht unterstützte Felder gemäß den [erkannten Feldnamen](/help/user-guide/templates/customize-template.md#recognized-field-names). |
