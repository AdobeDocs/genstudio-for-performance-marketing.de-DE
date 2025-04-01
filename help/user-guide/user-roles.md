---
title: Adobe GenStudio for Performance Marketing-Benutzerrollen und -Berechtigungen
description: Erfahren Sie mehr über Benutzerrollen und Berechtigungen in GenStudio for Performance Marketing.
level: Beginner
feature: Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 10%

---

# Benutzerrollen und -berechtigungen

Das Erstellen und Bereitstellen moderner Marketing-Kampagnen erfordert die Zusammenarbeit von Stakeholdern mit unterschiedlichen Zuständigkeiten und Fähigkeiten. _Benutzerrollen_ steuern den Zugriff der Stakeholder auf die vielen Funktionen von GenStudio for Performance Marketing. Die zugewiesene Benutzerrolle bestimmt die Aufgaben, die Sie auf dieser Plattform ausführen können. Ein Adobe-Systemadministrator weist Ihnen eine Rolle im GenStudio-Produktprofil in der Adobe Admin Console zu. Ihre Begrüßungs-E-Mail identifiziert Ihre zugewiesene Rolle.

>[!NOTE]
>
>Bevor Benutzende für diese Rollen bereitgestellt werden, muss in der Adobe Admin Console ein Adobe-Systemadministrator ernannt werden, um einmalige Einrichtungsaufgaben durchzuführen. Diese Adobe-Administratorrolle funktioniert nur im Kontext der Adobe Admin Console. In der Benutzeroberfläche der GenStudio for Performance Marketing-Plattform spielt sie keine Rolle. Ein Adobe-Systemadministrator, der Berechtigungen für den System Manager benötigt, muss sich selbst als GenStudio-Systemmanager in der Adobe Admin Console bereitstellen. Siehe [Bereitstellen von GenStudio for Performance Marketing](product-provisioning.md).

## Adobe-Systemadministrator im Vergleich zu GenStudio System Manager

Diese Benutzerrollentitel mögen ähnlich aussehen, sie identifizieren jedoch eindeutige Rollen, die Berechtigungen in verschiedenen Umgebungen bereitstellen.

**Adobe-Systemadministratoren** verfügen über Hauptbenutzerberechtigungen in der Adobe Admin Console und führen alle Benutzerverwaltungsaufgaben aus, z. B. das Hinzufügen oder Löschen von Benutzern. Diese Systemadministratorrolle gewährt keine Berechtigungen in der GenStudio for Performance Marketing-Anwendung, was erklärt, warum Adobe-Systemadministratoren keine Lizenz für GenStudio benötigen. Adobe-Systemadministratoren verwenden in der Regel die Admin Console, um Benutzerkonten aus GenStudio-Bereitstellungen hinzuzufügen und zu löschen und Berechtigungen oder Berechtigungen von einzelnen Benutzenden oder Benutzergruppen zuzuweisen oder zu entfernen.

**GenStudio-Systemmanager** sind Hauptbenutzer in GenStudio for Performance Marketing, haben jedoch keine Berechtigung zum Ausführen von Aufgaben in Adobe Admin Console. Diese System Manager-Rolle erfordert eine GenStudio-Produktlizenz und entspricht einem Power User in der [Adobe GenStudio for Performance Marketing-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html). GenStudio-Systemmanager verfügen über alle Berechtigungen für GenStudio for Performance Marketing-Funktionen, einschließlich [!DNL Brands], [!DNL Persona] und [!DNL Product] Erstellung, Löschen, Aktualisieren und Veröffentlichen. [Adobe GenStudio for Performance Marketing-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) Erläutert, wie GenStudio-Benutzerrollen mit Produktlizenzen zusammenhängen.

Siehe [Administratorrollen](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise) im _Administrationshandbuch für Unternehmen und Teams_.

## Berechtigungen

_Berechtigungen_ erteilen Berechtigungen zum Ausführen bestimmter Aufgaben und zum Zugriff auf geschützte Ressourcen. Berechtigungen werden in der Benutzerrolle innerhalb des Produktprofils definiert und Benutzer erhalten diese Berechtigungen, wenn sie dieser Rolle zugewiesen werden.

>[!IMPORTANT]
>
>Fügen Sie keine neuen Produktprofile hinzu und bearbeiten oder löschen Sie sie nicht. Eine Änderung der Standardproduktprofile kann Ihre GenStudio for Performance Marketing-Bereitstellung ernsthaft stören.

## Benutzerrollen

Diese Vielfalt an organisatorischen Rollen wird durch drei Typen von GenStudio for Performance Marketing-Benutzerrollen unterstützt. Berechtigungen sind auf jeden dieser Benutzertypen zugeschnitten und unterstützen die Verantwortlichkeiten der einzelnen Benutzer in der Marketing-Organisation. Diese drei Benutzerrollentypen sind:

* **GenStudio-Editoren** Verwenden Sie die KI-Funktionen von GenStudio for Performance Marketing, um Marketing-Kampagnen-Assets zu erstellen, die Überprüfung und Genehmigung von Inhalten anzufordern und genehmigte Entwürfe dieser Inhalte zu veröffentlichen. Alle GenStudio for Performance Marketing-Benutzer können auf ein Asset zugreifen und es verwenden, sobald der Editor es in [!DNL Content] gespeichert hat. GenStudio-Editoren sind Power-User in GenStudio for Performance Marketing.

* **GenStudio-Mitwirkende** sind die größte Auswahl an GenStudio for Performance Marketing-Benutzenden. Mitwirkende können Inhalte anzeigen und genehmigen und sind ein wesentlicher Teil des Workflows, der sicherstellt, dass die von Ihnen generierten Inhalte den Anforderungen und Standards Ihres Unternehmens entsprechen. GenStudio-Mitarbeiter sind _Mitarbeiter-Benutzer_ in GenStudio for Performance Marketing.

* **GenStudio-** verfügen über die umfassendsten Berechtigungen innerhalb von GenStudio for Performance Marketing. Systemmanager führen die grundlegende Onboarding-Aufgabe aus, nämlich die Festlegung der grundlegenden Leitplanken für die Erstellung und Bereitstellung von Kampagnen-Assets. System-Manager setzen diese Schutzmechanismen um, indem sie marken- und organisationsspezifische Informationen wie z. B. [Markenrichtlinien) ](./guidelines/overview.md). System-Manager sind berechtigt, [!DNL Brands] zu erstellen und zu veröffentlichen, verfügen jedoch nicht über Administratorrechte für Benutzer. GenStudio-Systemmanager sind Power-User in GenStudio for Performance Marketing.

### GenStudio-Editoren

_Bearbeiter_ oder Ersteller von Inhalten verfügen über die grundlegenden Berechtigungen, die zum Erstellen von GenStudio for Performance Marketing-[!DNL Brands], -[!DNL Campaigns] und -[!DNL Content] erforderlich sind. Diese Hauptbenutzer können auch von ihnen erstellte Assets bearbeiten und löschen. GenStudio for Performance Marketing unterstützt die schnelle Erstellung von Hunderten von Inhalten. Diese Benutzenden können Inhaltsfragmente oder ganze Erlebnisse generieren, die einzelne Teile genehmigter Inhalte orchestrieren, um die Anforderungen bestimmter Marketing-Kampagnen zu erfüllen.

Editoren interagieren mit GenStudio for Performance Marketing-KI-Technologien für generative _über_. Die Eingabeaufforderungsschublade auf der Arbeitsfläche bietet Tools zum Platzieren von Eingabeaufforderungen im Kontext der Richtlinien einer bestimmten Kampagne. Daher hängen die Qualität und der Erfolg der generierten Inhalte teilweise von der Qualität der von Ihrem Unternehmen hochgeladenen Markenrichtlinien und der Spezifität Ihrer Eingabeaufforderung ab. Siehe [Effektive Eingabeaufforderungen schreiben](effective-prompts.md).

In der folgenden Tabelle werden die standardmäßigen Editor-Berechtigungen angezeigt:

| Funktion | Erstellen | Update | Löschen | Anzeigen |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | nein | nein | nein | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Create] | ja | ja | ja | ja |
| [!DNL Insights] | Kann nur Connectoren konfigurieren |    |     | ja |
| [!DNL Personas] | ja | Ja* | Ja* | ja |
| [!DNL Products] | ja | Ja* | Ja* | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |
| [!DNL Templates] | nein | nein | nein | ja |

Bearbeiter können [!DNL Personas] und [!DNL Products], die sie erstellt haben, bearbeiten und löschen.

GenStudio-System-Manager können Bearbeitern die Berechtigung zum Bearbeiten und Löschen eines [!DNL Brand] erteilen.

### GenStudio-Mitarbeiter

_Mitwirkende_ können Assets in GenStudio for Performance Marketing anzeigen, diese Assets jedoch nicht erstellen, bearbeiten oder löschen. Teilnehmer sehen beispielsweise die Meldung &quot;*Sie haben keinen Zugriff auf diesen Inhalt* wenn sie versuchen, auf [[!DNL Create]](/help/user-guide/create/overview.md) zuzugreifen.

Zu den Mitwirkenden gehören Stakeholder, die für den Erfolg des Überprüfungs- und Genehmigungsprozesses für Inhalte von entscheidender Bedeutung sind, aber keine Inhalte erstellen oder direkt bearbeiten müssen. Juristen und Manager von Kreativen sind Beispiele für potenzielle Mitarbeiter. GenStudio for Performance Marketing-Mitwirkende sind möglicherweise berechtigt, Assets in anderen Creative Cloud-Produkten zu erstellen und anzuzeigen.

In der folgenden Tabelle werden die standardmäßigen Collaborator-Berechtigungen angezeigt:

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
| [!DNL Templates] | nein | nein | nein | ja |

### GenStudio-Systemmanager

_GenStudio-_ verfügen über den leistungsfähigsten Berechtigungssatz in GenStudio for Performance Marketing. Diese erfahrenen Benutzer führen die grundlegende Onboarding-Aufgabe aus, nämlich die Festlegung der grundlegenden Leitplanken für die Erstellung und Bereitstellung von Kampagnen-Assets. System-Manager setzen diese Schutzmechanismen um, indem sie marken- und organisationsspezifische Informationen wie z. B. [Markenrichtlinien) ](./guidelines/overview.md). System-Manager sind berechtigt, [!DNL Brands] zu erstellen und zu veröffentlichen, verfügen jedoch nicht über Administratorrechte für Benutzer.

In der folgenden Tabelle werden die standardmäßigen System Manager-Berechtigungen angezeigt:

| Funktion | Erstellen | Update | Löschen | Anzeigen |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | ja | ja | ja | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |
| [!DNL Templates] | ja | ja | ja | ja |

System-Manager können auch Vorlagen hochladen.

Unter [Erste Schritte mit Adobe GenStudio for Performance Marketing](get-started.md) finden Sie einen Überblick über vorbereitende Einrichtungsaufgaben.
