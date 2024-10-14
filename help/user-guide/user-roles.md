---
title: Benutzerrollen und Berechtigungen in Adobe GenStudio for Performance Marketing
description: Erfahren Sie mehr über GenStudio for Performance Marketing-Benutzerrollen und -Berechtigungen.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 12%

---

# Benutzerrollen und Berechtigungen

Die Erstellung und Bereitstellung moderner Marketing-Kampagnen erfordert die Zusammenarbeit zwischen Interessenträgern mit unterschiedlichen Verantwortlichkeiten und Kenntnissen. _Benutzerrollen_ steuern den Zugriff von Interessengruppen auf die zahlreichen Funktionen von GenStudio for Performance Marketing. Ihre zugewiesene Benutzerrolle bestimmt die Aufgaben, die Sie mit dieser Plattform ausführen können. Ein Adobe-Systemadministrator weist Sie einer Rolle im GenStudio-Produktprofil in der Adobe Admin Console zu. Ihre Begrüßungs-E-Mail identifiziert Ihre zugewiesene Rolle.

>[!NOTE]
>
>Bevor Benutzer für diese Rollen bereitgestellt werden, muss in der Adobe Admin Console ein Adobe-Systemadministrator benannt werden, der die einmalige Einrichtung durchführt. Diese Adobe-Administratorrolle funktioniert nur im Kontext der Adobe Admin Console. In der Benutzeroberfläche der GenStudio for Performance Marketing-Plattform spielt sie keine Rolle. Ein Adobe-Systemadministrator, der Berechtigungen des Systemmanagers benötigt, muss sich in der Adobe Admin Console als GenStudio-Systemmanager bereitstellen. Siehe [GenStudio for Performance Marketing bereitstellen](product-provisioning.md).

## Berechtigungen

_Berechtigungen_ gewähren Berechtigungen zum Ausführen bestimmter Aufgaben und zum Zugriff auf geschützte Ressourcen. Berechtigungen werden in der Benutzerrolle im Produktprofil definiert und Benutzer erhalten diese Berechtigungen, wenn sie dieser Rolle zugewiesen werden.

## Benutzerrollen

Drei Arten von GenStudio for Performance Marketing-Benutzerrollen unterstützen diese Vielfalt von Organisationsrollen. Berechtigungen sind auf jeden dieser Benutzertypen zugeschnitten und unterstützen die Verantwortlichkeiten der einzelnen Benutzer in der Marketing-Organisation. Diese drei Benutzerrollentypen sind:

* **GenStudio-Editoren** verwenden die generativen KI-Funktionen von GenStudio for Performance Marketing, um Marketing-Kampagnen-Assets zu erstellen, Inhaltsüberprüfung und -genehmigung anzufordern und genehmigte Entwürfe zu veröffentlichen. Alle GenStudio for Performance Marketing-Benutzer können auf ein Asset zugreifen und es verwenden, nachdem es im Editor in [!DNL Content] gespeichert wurde.

* **GenStudio-Mitwirkende** sind die umfangreichsten GenStudio for Performance Marketing-Benutzer. Mitwirkende können Inhalte anzeigen und genehmigen. Dies ist ein wesentlicher Bestandteil des Workflows, der sicherstellt, dass die von Ihnen generierten Inhalte den Anforderungen und Standards Ihres Unternehmens entsprechen.

* **GenStudio-Systemmanager** verfügen über die umfassendsten Berechtigungen innerhalb von GenStudio for Performance Marketing. Systemmanager führen die grundlegende Onboarding-Aufgabe durch, die darin besteht, die grundlegenden Limits für die Erstellung und Implementierung von Kampagnen-Assets zu definieren. Systemmanager implementieren diese Limits, indem sie Marken- und organisationsspezifische Informationen wie [Markenrichtlinien](./guidelines/overview.md) hochladen. Systemmanager sind berechtigt, [!DNL Brands] zu erstellen und zu veröffentlichen, haben jedoch keine Benutzeradministrationsberechtigungen.

### GenStudio-Editoren

_Bearbeiter_ oder Ersteller von Inhalten verfügen über die zum Erstellen von GenStudio for Performance Marketing [!DNL Brands]-, [!DNL Campaigns]- und [!DNL Content]-Assets erforderlichen Kernberechtigungen. Sie können auch von ihnen erstellte Assets bearbeiten und löschen. GenStudio for Performance Marketing unterstützt die schnelle Erstellung von Hunderten von Inhaltselementen. Diese Benutzer können Inhaltsfragmente oder ganze Erlebnisse generieren, die diskrete Teile genehmigter Inhalte orchestrieren, um die Anforderungen spezifischer Marketing-Kampagnen zu erfüllen.

Bearbeiter interagieren mit den generativen KI-Technologien von GenStudio for Performance Marketing über _Eingabeaufforderung_. Die Eingabeaufforderung auf der Arbeitsfläche bietet Tools zum Platzieren von Eingabeaufforderungen im Kontext der Richtlinien einer bestimmten Kampagne. Die Qualität und der Erfolg des erstellten Inhalts hängen daher teilweise von der Qualität der Markenrichtlinien ab, die Ihr Unternehmen hochgeladen hat, und von der Spezifität Ihrer Eingabeaufforderung. Siehe [Effektive Eingabeaufforderungen schreiben](effective-prompts.md).

In der folgenden Tabelle werden die standardmäßigen Editor-Berechtigungen angezeigt:

| Funktion | Erstellen | Update | Löschen | Anzeigen |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | nein | nein | nein | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Create] | ja | ja | ja | ja |
| [!DNL Insights] | Nur Anzeigenverbindungen konfigurieren |    |     | ja |
| [!DNL Personas] | ja | ja* | ja* | ja |
| [!DNL Products] | ja | ja* | ja* | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

Bearbeiter können die von ihnen erstellten [!DNL Personas] und [!DNL Products] bearbeiten und löschen.

GenStudio-Systemmanager können Editoren die Berechtigung zum Bearbeiten und Löschen eines [!DNL Brand] erteilen.

### GenStudio-Mitarbeiter

_Mitwirkende_ können Assets in GenStudio for Performance Marketing anzeigen, aber diese Assets nicht erstellen, bearbeiten oder löschen. Mitwirkende sind Akteure, die für den Erfolg des Überprüfungs- und Genehmigungsprozesses für Inhalte unerlässlich sind, aber keine Inhalte erstellen oder direkt bearbeiten müssen. Juristische Experten und Kreativmanager sind Beispiele für potenzielle Mitwirkende. GenStudio for Performance Marketing-Mitwirkende können möglicherweise Assets in anderen Creative Cloud-Produkten erstellen und anzeigen.

In der folgenden Tabelle werden die Standardberechtigungen für Mitwirkende angezeigt:

| Funktion | Erstellen | Update | Löschen | Anzeigen |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | nein | nein | nein | ja |
| [!DNL Campaigns] | nein | nein | nein | ja |
| [!DNL Content] | nein | nein | nein | ja |
| [!DNL Create] | nein | nein | nein | ja |
| [!DNL Insights] | nein | nein | nein | ja |
| [!DNL Personas] | nein | nein | nein | ja |
| [!DNL Products] | nein | nein | nein | ja |
| [!DNL Reviews and approvals] | nein | nein | nein | ja |

### GenStudio-Systemmanager

_GenStudio-Systemmanager_ verfügen über die leistungsstärksten Berechtigungen in GenStudio for Performance Marketing. Systemmanager führen die grundlegende Onboarding-Aufgabe durch, die darin besteht, die grundlegenden Limits für die Erstellung und Implementierung von Kampagnen-Assets zu definieren. Systemmanager implementieren diese Limits, indem sie Marken- und organisationsspezifische Informationen wie [Markenrichtlinien](./guidelines/overview.md) hochladen. Systemmanager sind berechtigt, [!DNL Brands] zu erstellen und zu veröffentlichen, haben jedoch keine Benutzeradministrationsberechtigungen.

In der folgenden Tabelle werden die standardmäßigen Systemmanagerberechtigungen angezeigt:

| Funktion | Erstellen | Update | Löschen | Anzeigen |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | ja | ja | ja | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

Unter [Erste Schritte mit Adobe GenStudio for Performance Marketing](get-started.md) finden Sie einen Überblick über vorbereitende Einrichtungsaufgaben.
