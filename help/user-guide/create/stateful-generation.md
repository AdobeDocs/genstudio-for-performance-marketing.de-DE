---
title: Erstellen und Verfeinern von Inhalten mit zustandsbasierter Generierung
description: Erfahren Sie, wie Sie markeninterne Inhalte generieren und diese nacheinander in einem Gespräch mit Stimmdruck und visuellen Hinweisen in [!DNL GenStudio for Performance Marketing] verfeinern können.
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# Erstellen und Verfeinern von Inhalten mit Stateful-Generierung

[!DNL GenStudio for Performance Marketing] verwendet die statusbehaftete Generierung, um Ihnen zu helfen, markeninterne Inhalte zu erstellen und diese dann in einem Gespräch abwechselnd zu verfeinern, anstatt jedes Mal mit einer neuen Eingabeaufforderung von vorne zu beginnen. Beim Verfeinern speichert die Generierung Ihre früheren Anweisungen und die Varianten, die Sie beibehalten, und wendet dann nur die gewünschte Änderung an.

Die statusbehaftete Generierung fügt Ihren Generationen drei Arten von Kontext hinzu: Beim Stimmdruck wird die Kopie in der Markensprache beibehalten, bei visuellen Hinweisen wird die Basiskopie in einem Bild oder Video beibehalten, und eine Web-Seiten-URL fügt den Referenzkontext einer von Ihnen ausgewählten Seite hinzu.

## Erstellen und Verfeinern von Inhalten

1. Starten Sie [!DNL GenStudio for Performance Marketing] eine Generierung für Ihren Kanal und Ihr Format. Unter [[!DNL Create] Übersicht](/help/user-guide/create/overview.md) können Sie für jeden Kanal eine Generierung starten.
1. _Optional_: Um die Kopie in Ihrem eigenen Kreativ zu erden, wählen Sie **[!UICONTROL Aus Inhalt auswählen]** und wählen Sie dann ein Bild oder Video aus, das als [visueller Hinweis verwendet werden soll](#ground-content-in-an-image-or-video).
1. Wählen Sie **[!UICONTROL Generieren]**. [!DNL GenStudio for Performance Marketing] erstellt einen Variantensatz und wendet Ihre [Markensprache](#keep-copy-in-your-brand-voice) automatisch auf unterstützte Kanäle an.
1. Verfeinern Sie die Ergebnisse in der Eingabeaufforderungs-Schublade. Geben Sie die gewünschte Änderung ein, z. B. `shorten the headline`, `make variant 2 punchier` oder `change the headline`. Die Generierung gilt nur für diese Änderung und behält Ihre früheren Anweisungen bei.
1. Um eine Variante beizubehalten, während Sie weiter verfeinern, geben Sie eine Anweisung in die Eingabeaufforderungsschublade ein, z. B. `keep variant 2`.
1. Wenn der Inhalt fertig ist, exportieren Sie ihn oder senden Sie ihn zur Überprüfung.

## Grundlegender Inhalt in einem Bild oder Video

Visuelle Hinweise ermöglichen es der Generierung, ein angehängtes Bild oder Video zu lesen und dann eine Kopie zu schreiben, die diese kreative Seite widerspiegelt. Der Umschalter **[!UICONTROL Creative]** Optionen“ steuert visuelle Hinweise, die standardmäßig aktiviert sind.

Um einen visuellen Hinweis zu verwenden, wählen Sie **[!UICONTROL Aus Inhalt auswählen]** und wählen Sie vor dem Generieren ein Bild oder Video aus. Um ohne visuellen Hinweis zu generieren, deaktivieren Sie **[!UICONTROL Creative-Optionen]**.

>[!NOTE]
>Visuelle Hinweise sind für Anzeigen mit mehreren Frames oder Karussellanzeigen nicht verfügbar.

## Kopie in der Markensprache aufbewahren

Der Sprachdruck wendet die erlernte Stimme Ihrer Marke auf eine generierte Kopie an, sodass sie ohne zusätzliche Aufforderung in der Marke klingt. Bei Kanälen mit „Insights[&#x200B; wie LinkedIn und Meta &#x200B;](/help/user-guide/insights/overview.md) sie standardmäßig aktiviert.

## Web-Seite als Kontext verwenden

Sie können die Generierung auf eine Web-Seite verweisen und ihren Inhalt als Kontext verwenden. Geben Sie in die Eingabeaufforderungs-Schublade eine Anweisung ein, die die URL enthält, z. B. `Use this URL to generate an ad for this channel: https://www.example.com`.

>[!NOTE]
>Geben Sie die URL in Ihrer Eingabeaufforderung ein. Fügen Sie sie nicht über &quot;_&quot;_.

## Verwandte Funktionen

- [Varianten verwalten](/help/user-guide/create/manage-variants.md): Bearbeiten und optimieren Sie generierte Varianten direkt auf der Arbeitsfläche.
- [Effektive Eingabeaufforderungen schreiben](/help/user-guide/effective-prompts.md): Erstellen Sie Eingabeaufforderungen, die bessere Ergebnisse erzielen.
