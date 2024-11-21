---
title: Erste Schritte mit Adobe GenStudio for Performance Marketing
description: Erfahren Sie, wie Sie mit GenStudio for Performance Marketing beginnen, um neue Marketing-Inhalte zu generieren, die auf Ihre Marken abgestimmt sind.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 2%

---

# Erste Schritte mit Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing bietet eine umfassende Palette von Tools, die die Erstellung, Verwaltung und Analyse von Inhalten optimieren. Er fügt den Lebenszyklus der Inhaltserstellung mit generativen KI-Funktionen in den Vordergrund, die die Erstellung, Überprüfung, Freigabe und Analyse von Marketing-Inhalten verändern.

## Erstellen, Freigeben und Überprüfen von Inhalten

Wenn Sie mit generativen KI-basierten Tools noch nicht vertraut sind oder sich einfach nur für die Grundprinzipien von GenStudio for Performance Marketing interessieren, finden Sie weitere Informationen unter [Konzepte](concepts.md) und [Wirksame Eingabeaufforderungen schreiben](effective-prompts.md). Sehen Sie sich die Online-Lernplattform [Adobe GenStudio Academy](https://learningmanager.adobe.com/genstudioacademy) an, die Adobe-Lernplattform zur Nutzung generativer KI-Technologien im Kreativprozess.

## Trainieren von GenStudio for Performance Marketing

GenStudio for Performance Marketing verwendet Informationen über Ihre Marke und Ihre Märkte, um die Erstellung markenkonformer Inhalte zu verbessern. Schulungsmaterialien umfassen Beispiele, Beschreibungen der Kunden [personas](/help/user-guide/guidelines/personas.md) und [products](/help/user-guide/guidelines/products.md) sowie [Markenrichtlinien](/help/user-guide/guidelines/overview.md).

Systemmanager richten Adobe GenStudio for Performance Marketing ein, indem sie unternehmensspezifische Informationen eingeben oder hochladen. Diese Vorbereitung stellt sicher, dass Inhaltseditoren und Mitarbeiter die generativen KI-Funktionen effektiv verwenden können, um Kampagnen-Assets zu erstellen und zu überprüfen. Sobald ein Adobe-Systemadministrator die Produktinstanz Ihres Unternehmens bereitstellt und eine GenStudio-Systemmanagerberechtigung zuweist, kann der GenStudio-Systemmanager das zugrunde liegende generative KI-Framework des Produkts mithilfe von Richtlinien vorbereiten.

### Schritt 1: Richtlinien hinzufügen

Die Einrichtung der wichtigsten Bausteine der Markenidentität Ihres Unternehmens ist eine wesentliche Voraussetzung für die Arbeit von Inhaltseditoren und -mitarbeitern. [Richtlinien](./guidelines/overview.md) erfassen Markenmerkmale wie Logos, Ton der Stimme und Farbpaletten. Sie können entweder [[!DNL Brands] guidelines](./guidelines/brands.md)-Dokumente hochladen oder Marktinformationen manuell eingeben. Auch [[!DNL Personas] guidelines](./guidelines/personas.md) und [[!DNL Products] guidelines](./guidelines/products.md) sind wichtig. Die zugrunde liegenden generativen KI-Funktionen von GenStudio for Performance Marketing verwenden diese Richtlinien, um Limits festzulegen, die die Inhaltserstellung leiten.

#### Vorbereiten Ihrer Führungsdokumente

Umfassende und fokussierte Richtlinien für [[!DNL Brands]](./guidelines/brands.md), [[!DNL Products]](./guidelines/products.md) und [[!DNL Personas]](./guidelines/personas.md) definieren die Kernaspekte der Marketing-Kampagnen Ihres Unternehmens. GenStudio for Performance Marketing extrahiert Informationen aus diesen Richtlinien, um Ihre Marke zu erstellen.

Befolgen Sie diese Best Practices bei der Erstellung von Leitlinien:

* Verwenden Sie eine bestimmte Sprache.

* Beziehen Sie die besten Beispiele für den Stil und Ton ein, den Kampagnen-Assets darstellen sollen.

* Vermeiden Sie Redundanz. Sie sind möglicherweise versucht, eine Richtlinie mehrmals zu wiederholen, doch die Redundanz in Ihren Richtlinien hilft nicht der zugrunde liegenden LLM-Erfassung und Implementierung Ihrer Markenrichtlinien.

* Identifizieren Sie Elemente, die vom LLM bei der Inhaltserstellung ausgeschlossen werden sollen (z. B. Ausrufepunkte im Text).

Sie können Führungslinien-Dokumente hochladen oder sie konsultieren, wenn Sie Informationen manuell in GenStudio for Performance Marketing eingeben. Anleitungen zum Hochladen oder Eingeben dieser Informationen finden Sie unter [Richtlinien hinzufügen](./guidelines/overview.md) .

#### Überarbeiten von Leitlinien

Ein GenStudio-Systemmanager kann das zugrunde liegende generative KI-Framework des Produkts vorbereiten, indem Sie manuell die spezifischen Markenanforderungen Ihres Unternehmens eingeben oder hochladen. Obwohl die Einrichtung der Markenrichtlinien eines Unternehmens eine einmalige Aktion ist, können Sie diese Richtlinien auf Grundlage der Volatilität, des Wachstums und der sich ändernden Marktbedingungen in Ihrem Unternehmen überarbeiten und verbessern.

## Schritt 2: Einrichten eines Adobe Admin Console-Projekts für GenStudio [!DNL Brands]

Systemadministratoren müssen zusätzliche Einrichtungsaufgaben ausführen, bevor sie [!DNL Brands] bearbeiten oder erstellen können. Adobe-Systemadministratoren führen diese Aufgaben in der Adobe Admin Console aus:

* Erstellen Sie eine neue Benutzergruppe, die alle Benutzer enthält, die bearbeitet werden müssen, und erstellen Sie [!DNL Brands] -Berechtigungen.

* Erstellen Sie ein neues Projekt in der Adobe Admin Console.

Siehe [Zuweisen von Markenberechtigungen](configure-brand-permissions.md).

### Schritt 3: Vorlagen hochladen

Vorlagen beschleunigen die Inhaltserstellung. Eine Vorlage enthält genehmigte Funktionen wie Kopf- und Fußzeilen und ist für bestimmte Kanäle optimiert. Systemmanager laden normalerweise Vorlagen für ihre Organisation hoch und verwalten sie. Inhaltseditoren verwenden Vorlagen, um den Inhaltserstellungsprozess innerhalb der festgelegten Grenzen der Organisationsmarke zu starten.

Siehe [Arbeiten mit Vorlagen](./content/use-templates.md).

### Schritt 4: Hochladen genehmigter Assets

Genehmigte Assets in [!DNL Content] stehen allen GenStudio for Performance Marketing-Editoren zur Verfügung. Sie können [!DNL Content] mit Assets füllen, damit Inhaltseditoren neue Erlebnisse oder Assets erstellen können.

Siehe [Hochladen genehmigter Assets](./content/manage-assets.md).

### Schritt 5: Verbindung zu einem Meta (Facebook)-Konto herstellen

Konfigurieren Sie eine Verbindung zwischen GenStudio for Performance Marketing und den Social-Konten Ihres Unternehmens, um Daten aus Ihren aktiven Marketing-Kampagnen, -Assets und -Erlebnissen zu erhalten. [[!DNL Insights]](./insights/overview.md) bietet Tools zur Analyse von kanalabgeleiteten Daten. Siehe [Verbindung zu einem Meta (Facebook)-Konto herstellen](./insights/connect-channel.md#meta-ads-connect).
