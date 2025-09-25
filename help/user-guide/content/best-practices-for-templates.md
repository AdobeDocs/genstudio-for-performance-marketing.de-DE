---
title: Best Practices für Vorlagen
description: Befolgen Sie die Best Practices bei der Verwendung von Vorlagen mit Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Best Practices für die Verwendung von Vorlagen

Vorlagen reduzieren den Zeit- und Arbeitsaufwand für die Erstellung neuer Inhalte erheblich, indem sie einen Ausgangspunkt bereitstellen, der vorkonfigurierte Layouts und Designelemente enthält.

Verwenden Sie bei der Verwendung von Vorlagen mit GenStudio for Performance Marketing die folgenden Empfehlungen:

1. Know about [template elements](#know-about-template-elements)
1. Konfigurieren [Kanalrichtlinien](#configure-channel-guidelines) für die effektive Personalisierung von Inhalten
1. Design mit [Barrierefreiheitsstandards](accessibility-for-templates.md) für ein optimales Erlebnis
1. Befolgen [kanalspezifischen Vorlagenrichtlinien](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Weitere Informationen über grundlegende Vorlagenelemente und Verfahren finden Sie unter [Arbeiten mit Vorlagen](use-templates.md). und detaillierte Einblicke in [Anpassen einer Vorlage](customize-template.md) zur Verwendung in Ihrer nächsten Kampagne.

## Know about template elements

Es empfiehlt sich, sich mit den Teilen einer Vorlage vertraut zu machen. Jeder Vorlagentyp verwendet verschiedene Elemente, um eine Struktur für die kanalspezifische Inhaltserstellung zu erstellen. Um Ihre Vorlage anzupassen, verwenden Sie die Feldnamen anstelle dieser Elemente, für die GenStudio for Performance Marketing Inhalte generieren muss.

Siehe [Vorlagenelemente](use-templates.md#template-elements).

## Konfigurieren von Kanalrichtlinien

Die Definition klarer Kanal-Richtlinien ist wichtig, um sicherzustellen, dass Ihre generierten Inhalte mit den Anforderungen und Zielen Ihrer Marke übereinstimmen. Mit Kanalrichtlinien können Sie Regeln für Elemente wie Ton, Länge und Stil angeben, die in Ihrer Vorlage verwendet werden. Sie können beispielsweise eine maximale Zeichenanzahl für den Textkörper festlegen oder einen bestimmten call-to-action-Stil erfordern. Indem Sie diese Richtlinien im Voraus festlegen, müssen Sie in jeder KI-Eingabeaufforderung keine detaillierten Anweisungen mehr schreiben, den Prozess der Inhaltserstellung optimieren und die Konsistenz Ihrer E-Mails sicherstellen.

Überprüfen und definieren Sie die [Kanalrichtlinien](/help/user-guide/guidelines/brands.md#channel-guidelines) Ihrer Marke für alle Schlüsselfelder in Ihrer Vorlage. Wenn Sie keine Richtlinien definieren, werden die [Standardkanalrichtlinien](/help/user-guide/guidelines/brands.md#default-channel-guidelines) angewendet, die möglicherweise Ihre Markenanforderungen nicht vollständig widerspiegeln.

![Technische Daten des Textkörpers](/help/assets/channel-email-body.png)

Erfahren Sie, wie [Richtlinien für Marken, Produkte und Personas](/help/user-guide/guidelines/overview.md) generierte Inhalte beeinflussen und wie Sie sie an Ihre Marketing-Ziele anpassen können.

## Befolgen der Richtlinien für kanalspezifische Vorlagen

Stellen Sie beim Erstellen von Vorlagen sicher, dass sie die spezifischen Anforderungen des vorgesehenen Kanals erfüllen. Erstellen Sie Vorlagen, die das Layout und die visuellen Anforderungen für jeden Kanal berücksichtigen. Es gibt allgemeine Richtlinien, die für jede Vorlage gelten, z. B.:

- Verwenden Sie saubere und responsive HTML und Inline-CSS
- Verwenden von Adobe- oder Google-Schriftarten
- Verwenden **nicht** JavaScript

{{note-css-effects}}

Weitere Tipps und Einschränkungen beim Arbeiten mit jedem Vorlagentyp finden Sie, um eine optimale Leistung sicherzustellen:

- [E-Mails](/help/user-guide/templates/email-template.md)
- [Anzeigen und Banner](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta Ads](/help/user-guide/templates/meta-template.md)
