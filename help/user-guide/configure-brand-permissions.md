---
title: Zuweisen von  [!DNL Brand] Berechtigungen
description: Erfahren Sie mehr über die Zuweisung von Berechtigungen für GenStudio for Performance Marketing [!DNL Brand] Ersteller und Editoren.
level: Intermediate
feature: Brands Service, Generative AI
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%

---

# Zuweisen von [!DNL Brand] -Berechtigungen

Standardmäßig können GenStudio-Systemmanager [!DNL Brands] erstellen und bearbeiten. Die Rollen &quot;Inhaltseditor&quot;und &quot;Mitarbeiter&quot;verfügen über Bearbeitungs- und Erstellungsberechtigungen, erfordern jedoch möglicherweise keine Systemverwaltungsberechtigungen. Um Inhaltseditoren und Mitarbeitern diese [!DNL Brand]-bezogenen Berechtigungen zu gewähren, muss ein Adobe-Systemadministrator einige zusätzliche Konfigurationsaufgaben in der Adobe Admin Console durchführen. Siehe [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) im _Verwaltungshandbuch für Unternehmen und Teams_.

Das Hinzufügen von Benutzern und Benutzergruppen sind grundlegende Aufgaben, die für alle Adobe-Produkte mit Berechtigungen gelten, die über die Admin Console verwaltet werden. Eine Übersicht über die Benutzerverwaltung und die Verfahren zum Hinzufügen von Benutzern und Benutzergruppen finden Sie unter [Adobe Admin Console-Benutzer](https://helpx.adobe.com/de/enterprise/using/users.html) im _Administratorhandbuch für Unternehmen und Teams_ .

## Schritt 1: Erstellen einer Benutzergruppe

**So erstellen Sie eine Benutzergruppe**:

1. Melden Sie sich bei der Admin Console an und navigieren Sie zu **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzergruppen]**.

1. Klicken Sie auf **[!UICONTROL Neue Benutzergruppe]**. Das Popup _Neue Benutzergruppe erstellen_ wird geöffnet.

1. Fügen Sie dem Feld **[!UICONTROL Benutzergruppenname]** einen informativen Benutzergruppennamen hinzu, um den Zweck der neuen Gruppe zu identifizieren. Beispiel: &quot;Markenmanager&quot;.

1. Fügen Sie optional eine Beschreibung der Gruppe und ihren Zweck hinzu.

1. Klicken Sie auf **[!UICONTROL Speichern]**. Die Admin Console öffnet das Popup _Neue Gruppe_ mit dem Namen der neu erstellten Gruppe.

Siehe [Verwalten von Benutzergruppen](https://helpx.adobe.com/de/enterprise/using/user-groups.html) im _Administratorhandbuch für Unternehmen und Teams_.

## Schritt 2: Zuweisen eines GenStudio-Systemmanagerprofils zur Benutzergruppe

Nachdem Sie eine neue Benutzergruppe erstellt und Benutzer hinzugefügt haben, können Sie dieser Gruppe das Profil **Adobe GenStudio-Systemmanager** zuweisen. Die mit dem zugewiesenen Profil verknüpften Berechtigungen verleihen allen Benutzern der Gruppe GenStudio [!DNL Brands] Berechtigungen (Erstellen, Aktualisieren und Löschen von Marken).

**So weisen Sie der Benutzergruppe ein Profil zu**:

1. Navigieren Sie zur neu erstellten Benutzergruppe und klicken Sie auf die Registerkarte _Zugewiesene Produktprofile_ .

1. Klicken Sie auf der Registerkarte _Zugewiesene Produktprofile_ auf **[!UICONTROL Profil zuweisen]**. Das Popup &quot;_Produkte und Profile zuweisen_&quot; wird geöffnet.

1. Wählen Sie `Adobe GenStudio` aus der Liste _Produkte auswählen_ aus.

1. Klicken Sie auf **[!UICONTROL Anwenden]**. Das Popup _Produktprofile auswählen_ wird geöffnet und zeigt die Produktprofile an, die mit Adobe GenStudio verknüpft sind.

1. Wählen Sie `Adobe GenStudio system manager`.

1. Klicken Sie auf **[!UICONTROL Anwenden]**. Das Popup &quot;Produkte und Profile zuweisen&quot;_wird geöffnet und zeigt das Produktprofil für die neu erstellte Benutzergruppe an._

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Siehe [Zuweisen von Produktprofilen zu Benutzergruppen](https://helpx.adobe.com/de/enterprise/using/user-groups.html) im _Verwaltungshandbuch für Unternehmen und Teams_.

## Schritt 3: Erstellen eines [!DNL Brands] -Projekts

Ein _Projekt_ bietet einen Speicherort, an dem ausgewählte Benutzer Assets speichern können - in diesem Fall [!DNL Brands] Assets.

**So erstellen Sie ein [!DNL Brands] -Projekt über die Registerkarte _Speicher_**:

1. Navigieren Sie zur Registerkarte _Speicher_ in der Admin Console.

1. Klicken Sie in der Seitennavigation auf **[!UICONTROL Projekte]** . Die Registerkarte _Projekte_ wird geöffnet.

1. Klicken Sie auf **[!UICONTROL Projekt erstellen]**. Das Popup _Neues Projekt_ wird geöffnet.

1. Geben Sie `Adobe GenStudio Brands` in das Feld für den Projektnamen ein. Geben Sie diesen Projektnamen genau wie hier dargestellt ein. Fügen Sie keine zusätzlichen Leerzeichen hinzu oder ändern Sie die Groß-/Kleinschreibung.

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Das Popup _Einladen zum Projekt_ wird geöffnet.

Siehe [Verwalten von Projekten](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) im _Verwaltungshandbuch für Unternehmen und Teams_.

## Schritt 4: Einladen einer Benutzergruppe zum Projekt

Sie können jetzt die soeben erstellte Benutzergruppe zum Projekt `Adobe GenStudio [!DNL Brands]` hinzufügen.

**So laden Sie die Benutzergruppe zum neu erstellten Projekt ein**:

1. Fügen Sie im Popup _Einladen zum Projekt_ die soeben erstellte Benutzergruppe zu diesem Projekt hinzu.

1. Wählen Sie die Option **Kann die Berechtigungen bearbeiten** aus.

1. Klicken Sie auf **[!UICONTROL Einladen]**.

## Schritt 5: Benutzer zur Benutzergruppe hinzufügen

Um Benutzern die Berechtigung zum Erstellen, Bearbeiten und Veröffentlichen von [!DNL Brands] zuzuweisen, fügen Sie sie zur neu erstellten Benutzergruppe hinzu.

**Hinzufügen von Benutzern zur Benutzergruppe**:

1. Navigieren Sie von der _Admin Console_ zu **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzergruppen]**.

1. Wählen Sie den Namen der zuvor erstellten Benutzergruppe aus. Das Popup _Benutzer zu dieser Benutzergruppe hinzufügen_ wird geöffnet.

1. Fügen Sie einen neuen oder vorhandenen Benutzer entweder nach Benutzername oder E-Mail-Adresse hinzu. Erfahren Sie mehr über die Verwaltung von Benutzergruppen in [Benutzergruppen verwalten](https://helpx.adobe.com/de/enterprise/using/user-groups.html) im _Administratorhandbuch für Unternehmen und Teams_.

Benutzern werden die [!DNL Brand] Berechtigungen zum Erstellen, Bearbeiten und Veröffentlichen von Adobe GenStudio-Systemmanagern gewährt, wenn sie zur Gruppe hinzugefügt werden. Benutzer erhalten außerdem eine automatische E-Mail-Einladung zur Bearbeitung des Adobe GenStudio for Performance Marketing [!DNL Brands] -Projekts.
