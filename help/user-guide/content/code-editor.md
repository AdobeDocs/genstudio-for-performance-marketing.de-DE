---
title: Vorlagen-Code-Editor
description: Erfahren Sie, wie Sie den Vorlagen-Code-Editor in GenStudio for Performance Marketing verwenden.
level: Intermediate
feature: Templates, Content
source-git-commit: 96ed2b3e1a1d854b35bdddb5aa694fdfec727e1a
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Vorlagen-Code-Editor

Der Vorlagen-Code-Editor soll Ihnen dabei helfen, Ihre Vorlage zu überprüfen und zu verfeinern, damit sie beim Generieren neuer Erlebnisse mit GenStudio for Performance Marketing optimal verwendet werden kann. Der Editor unterstützt die Handlebars-Syntax, die Platzhalter in der Vorlage verwendet, um anzugeben, wo GenStudio for Performance Marketing Inhalte für Sie generieren soll.

>[!TIP]
>
>Bereiten Sie Ihre Vorlage vor dem Hochladen des HTML[!DNL Content]Vorlagencodes in der Ansicht _Vorlagen_ vor, indem Sie die in der Anleitung [Anpassen von Vorlagen](customize-template.md) definierten Platzhalter für Inhalte einfügen.

## Überprüfen erkannter Felder

Der Bereich _[!UICONTROL Erkannte Felder überprüfen]_ zeigt eine Liste von Feldern an, die GenStudio for Performance Marketing in Ihrer Vorlage erkennt. Überprüfen Sie die Liste und Sie können durch den HTML-Code scrollen, um die Bildung Ihrer Vorlage anzuzeigen.

![Code-Editor-Ansicht](/help/assets/template-detected-fields.png "Überprüfung erkannter Felder"){width="600" zoomable="yes"}

Wenn Sie feststellen, dass ein Feld in der Liste fehlt, durchsuchen Sie den Vorlagencode und suchen Sie nach dem Speicherort für das fehlende Feld. Fügen Sie den richtigen Platzhalter mithilfe der Handlebars-Syntax und eines [erkannten Feldnamens](/help/user-guide/content/customize-template.md#recognized-field-names) ein. Verwenden Sie das Formular Suchen und Ersetzen unten im Code-Editor, um nach bestimmten Zeichenfolgen im Code zu suchen. (Windows `CTRL`+`F` oder macOS `CMD`+`F`)

### Korrektur vornehmen

Wenn Ihre Vorlage Fehler enthält, wird möglicherweise eine `Template is invalid` mit einer kurzen Erläuterung des Problems angezeigt. Im folgenden Beispiel zeigt die Meldung an, dass das `_image` Feld nicht der in der Multi-Pod-Vorlage festgelegten Feldnamenskonvention entspricht. In der Meldung wird außerdem darauf hingewiesen, dass Sie den Feldnamen mit dem richtigen Präfix aktualisieren müssen. Suchen Sie das Feld `_image` im Vorlagen-Code-Editor und aktualisieren Sie den Namen wie empfohlen.

![Ungültige Vorlage korrigieren](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

Der _[!UICONTROL Überprüfen erkannter Felder]_ wird aktualisiert und zeigt die von Ihnen vorgenommenen Änderungen an. Wenn Sie sich vergewissert haben, dass die Felder korrekt und vollständig sind, klicken Sie auf **[!UICONTROL Weiter]**, um mit dem [ (Hochladen der Vorlage) ](/help/user-guide/content/use-templates.md#add-a-template).
