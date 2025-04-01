---
title: ' [!DNL Brand]  zuweisen'
description: Erfahren Sie mehr über das Zuweisen von Berechtigungen für GenStudio for Performance Marketing [!DNL Brand] Ersteller und Bearbeiter.
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# [!DNL Brand] Berechtigungen zuweisen

Standardmäßig können GenStudio-System-Manager [!DNL Brands] erstellen und bearbeiten. Die Rollen „Inhaltseditor“ und „Mitarbeiter“ verfügen über Bearbeitungs- und Erstellungsberechtigungen, erfordern jedoch möglicherweise keine Berechtigungen für die Systemverwaltung. Um Inhaltseditoren und Mitarbeitern diese Berechtigungen im Zusammenhang mit [!DNL Brand] zu gewähren, muss ein Adobe-Systemadministrator einige zusätzliche Konfigurationsaufgaben in der Adobe Admin Console durchführen. Siehe [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) im _Administrationshandbuch für Unternehmen und Teams_.

Das Hinzufügen von Benutzenden und Benutzergruppen sind grundlegende Aufgaben, die alle Adobe-Produkte mit Berechtigungen gemeinsam haben und über die Admin Console verwaltet werden. Eine Übersicht über die Benutzerverwaltung ](https://helpx.adobe.com/de/enterprise/using/users.html) die Verfahren zum Hinzufügen von _und Benutzergruppen finden Sie_ [Adobe Admin Console-Benutzer im Administrationshandbuch für Unternehmen und Teams.

## Schritt 1: Erstellen einer Benutzergruppe

**Erstellen einer Benutzergruppe**:

1. Melden Sie sich bei Admin Console an und navigieren Sie zu **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzergruppen]**.

1. Klicken Sie **[!UICONTROL Neue Benutzergruppe]**. Das _Erstellen einer neuen Benutzergruppe_ Popup wird geöffnet.

1. Fügen Sie dem Feld **[!UICONTROL Name der Benutzergruppe“ einen informativen]** hinzu, um den Zweck der neuen Gruppe anzugeben. Beispiel: „Brand Manager“.

1. Fügen Sie optional eine Beschreibung der Gruppe und ihres Zwecks hinzu.

1. Klicken Sie auf **[!UICONTROL Speichern]**. Admin Console öffnet das Popup _Neue Gruppe_ mit dem Namen der neu erstellten Gruppe.

Siehe [Benutzergruppen verwalten](https://helpx.adobe.com/de/enterprise/using/user-groups.html) im _Administrationshandbuch für Unternehmen und Teams_.

## Schritt 2: Zuweisen eines GenStudio System Manager-Profils zur Benutzergruppe

Nachdem Sie eine neue Benutzergruppe erstellt und Benutzer hinzugefügt haben, können Sie dieser Gruppe das Profil **Adobe GenStudio System Manager** zuweisen. Die mit dem zugewiesenen Profil verknüpfte Berechtigung gibt allen Benutzenden in dieser Gruppe GenStudio [!DNL Brands] Berechtigungen (Marken erstellen, aktualisieren und löschen).

**So weisen Sie der Benutzergruppe ein Profil zu**:

1. Navigieren Sie zur neu erstellten Benutzergruppe und klicken Sie auf die _Zugewiesene Produktprofile_ .

1. Klicken Sie auf der _Zugewiesene Produktprofile_ auf **[!UICONTROL Profil zuweisen]**. Das _Produkte und Profile zuweisen_ wird geöffnet.

1. Wählen Sie `Adobe GenStudio` aus der Liste _Produkte auswählen_ aus.

1. Klicken Sie **[!UICONTROL Apply]**. Das _Produktprofile auswählen_ Popup wird geöffnet und zeigt die mit Adobe GenStudio verknüpften Produktprofile an.

1. Wählen Sie `Adobe GenStudio system manager`.

1. Klicken Sie **[!UICONTROL Apply]**. Das _Produkte und Profile zuweisen_ wird geöffnet und zeigt das Produktprofil für die neu erstellte Benutzergruppe an.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Siehe [Zuweisen von Produktprofilen zu Benutzergruppen](https://helpx.adobe.com/de/enterprise/using/user-groups.html) im _Administrationshandbuch für Unternehmen und Teams_.

## Schritt 3: Benutzer zur Benutzergruppe hinzufügen

Um Benutzenden die Berechtigung zum Erstellen, Bearbeiten und Veröffentlichen von [!DNL Brands] zuzuweisen, fügen Sie sie der neu erstellten Benutzergruppe hinzu.

>[!NOTE]
>
>Sie müssen mindestens einen Benutzer zu dieser Benutzergruppe hinzufügen, bevor Sie die Gruppe zu Ihrem Projekt hinzufügen.

**So fügen Sie Benutzer zur Benutzergruppe hinzu**:

1. Admin Console Navigieren Sie in der __ zu **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzergruppen]**.

1. Wählen Sie den Namen der zuvor erstellten Benutzergruppe aus. Das _Benutzer zu dieser Benutzergruppe hinzufügen_-Popup wird geöffnet.

1. Fügen Sie einen neuen oder vorhandenen Benutzer anhand des Benutzernamens oder der E-Mail-Adresse hinzu. Wenn Sie einen Namen oder eine E-Mail-Adresse für einen vorhandenen Benutzer eingeben, wird dieses Feld automatisch mit übereinstimmenden Namen für bekannte Benutzer ausgefüllt, die zu dieser IMS-Organisation gehören. Erfahren Sie mehr über die Verwaltung von Benutzergruppen [Benutzergruppen verwalten](https://helpx.adobe.com/de/enterprise/using/user-groups.html) im _Administrationshandbuch für Unternehmen und Teams_.

Benutzern werden die [!DNL Brand] zum Erstellen, Bearbeiten und Veröffentlichen von Adobe GenStudio-System-Managern gewährt, wenn sie der Gruppe hinzugefügt werden. Benutzende erhalten auch eine automatisierte E-Mail-Einladung zum Bearbeiten des Adobe GenStudio for Performance Marketing [!DNL Brands]-Projekts.

## Schritt 4: Erstellen eines [!DNL Brands] Projekts

Ein _Projekt_ bietet einen Speicherort, an dem ausgewählte Benutzer Assets speichern können - in diesem Fall [!DNL Brands] Assets.

**So erstellen Sie ein [!DNL Brands] über die Registerkarte _Speicherung_:**

1. Navigieren Sie zur _Speicher_ in der Admin Console.

1. Klicken Sie **[!UICONTROL der Seitennavigation]** Projekte“. Die _Projekte_ wird geöffnet.

1. Klicken Sie **[!UICONTROL Projekt erstellen]**. Das Popup _Neues Projekt_ wird geöffnet.

1. Geben Sie `Adobe GenStudio Brands` in das Feld Projektname ein. Geben Sie diesen Projektnamen genau so ein, wie er hier angezeigt wird. Verwenden Sie keine zusätzlichen Leerzeichen oder ändern Sie die Groß-/Kleinschreibung.

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Das _Zum Projekt einladen_-Popup wird geöffnet.

Siehe [Projekte verwalten](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) im _Administrationshandbuch für Unternehmen und Teams_.

## Schritt 5: Benutzergruppe zum Projekt einladen

Sie können jetzt die soeben erstellte Benutzergruppe zum `Adobe GenStudio [!DNL Brands]` Projekt hinzufügen.

**So laden Sie die Benutzergruppe zum neu erstellten Projekt ein**:

1. Fügen Sie im _Zum Projekt einladen_ die soeben erstellte Benutzergruppe zu diesem Projekt hinzu.

1. Wählen Sie die **Kann bearbeiten** aus.

1. Klicken Sie **[!UICONTROL Einladen]**.
