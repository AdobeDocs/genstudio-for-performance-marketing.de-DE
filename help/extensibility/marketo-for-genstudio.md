---
title: Marketo für GenStudio
description: Installieren und konfigurieren Sie die App Marketo for GenStudio Adobe Exchange , damit Ihr Unternehmen Marketo Engage-Vorlagen in GenStudio for Performance Marketing verwenden kann.
feature: Extensibility
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# Marketo für GenStudio

Organisationen, die [!DNL Marketo Engage] und [!DNL GenStudio for Performance Marketing] in derselben [!DNL IMS] verwenden, können die App **Marketo for GenStudio** von [!DNL Adobe Exchange] installieren. Nachdem ein Systemadministrator die App genehmigt und die Bereitstellung abgeschlossen hat, können Autoren beim Erstellen von E-Mail-Erlebnissen in GenStudio neben den Vorlagen, die direkt in [!DNL Content] hochgeladen wurden, Marketo-Vorlagen auswählen.

Dieses Thema richtet sich an **Administratoren** die die App installieren, Anmeldedaten von Marketo einholen und die App in Exchange bereitstellen. Informationen zur Funktionsweise der Vorlagensyntax für AJO und Marketo mit GenStudio finden Sie unter [Vorlagen aus AJO und Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Voraussetzungen

* [!DNL Marketo Engage] muss in der Organisation bereitgestellt werden, in der Sie die Erweiterung bereitstellen.
* Benutzende, die die Anwendung bereitstellen, benötigen **Marketo-Anmeldeinformationen**. Um diese Anmeldeinformationen zu erstellen und abzurufen, benötigen Sie Zugriff auf den **Marketo** Produktadministrator. (Der **[!UICONTROL Admin]**-Bereich muss beim Öffnen von Marketo verfügbar sein.)

## Installieren der App über Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483320?captions=ger&learn=on)

1. Öffnen Sie [Adobe Exchange](https://exchange.adobe.com) und wechseln Sie zu **[!UICONTROL CX Enterprise]**.
1. Öffnen Sie die Liste [Marketo for GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio).
   ![Liste der Marketo for GenStudio in Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Wählen Sie **[!UICONTROL Kostenlos]** aus, um die App für Ihre Organisation anzufordern.
1. Nachdem Ihr Unternehmen **die Anfrage geprüft und**, fahren Sie mit [Marketo-Anmeldedaten abrufen](#get-marketo-credentials) und [das Programm über Exchange bereitstellen](#deploy-the-application-from-exchange) fort.

## Marketo-Anmeldedaten abrufen

Sie verwenden Anmeldedaten aus Ihrer **Marketo**-Instanz (nicht aus der Adobe Developer Console). Erfassen Sie anhand der folgenden Schritte die folgenden Anmeldeinformationen, bevor Sie sie in Exchange bereitstellen.

>[!NOTE]
>
>Um Marketo-Anmeldeinformationen zu generieren und abzurufen, benötigen Sie Zugriff auf den Marketo-Produktadministrator, sonst wird die Registerkarte Admin in Marketo nicht angezeigt.

### Nur einen API-Benutzer erstellen (optional, wenn Sie einen vorhandenen API-Benutzer wiederverwenden)

1. Navigieren Sie in Marketo zu **[!UICONTROL Admin]**.
   ![Registerkarte &quot;Marketo Admin“](/help/extensibility/marketo-admin-global.png){width="80%"}
1. Öffnen **[!UICONTROL unter]** Sicherheit **[!UICONTROL die Registerkarte Benutzer und Rollen]** und navigieren Sie zur Registerkarte **[!UICONTROL Rollen]**.
1. Erstellen Sie eine neue Rolle oder bearbeiten Sie eine vorhandene Rolle, mit den folgenden hinzugefügten Berechtigungen: _Access_ und _Access Design Studio_.
1. Klicken Sie für einen neuen API-Benutzer auf **[!UICONTROL Nur API-Benutzer erstellen]** (verwenden Sie für jeden API-Benutzer eine eindeutige E-Mail).
1. Aktivieren Sie das Kontrollkästchen für Rollen und weisen Sie die von Ihnen erstellte neue Rolle zu. Wenn Sie bereits über einen API-Benutzer verfügen, den Sie verwenden möchten, fahren Sie mit [Erstellen oder wählen Sie einen LaunchPoint-Service aus](#create-or-select-a-launchpoint-service) fort.

![Benutzer und Rollen nur mit API-Benutzer- und API-Rollen](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### LaunchPoint-Service erstellen oder auswählen

1. Öffnen Sie **[!UICONTROL Admin]** unter **[!UICONTROL Integration]** die Option **[!UICONTROL LaunchPoint]**.
1. Klicken Sie **[!UICONTROL Erstellen]**, um einen neuen Service zu erstellen (oder einen vorhandenen benutzerdefinierten Service zu verwenden).
   ![Benutzerdefinierter LaunchPoint-Service](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. Klicken Sie für Ihren Dienst auf **[!UICONTROL Details anzeigen]** und kopieren Sie die **[!UICONTROL Client-ID]** und **[!UICONTROL Client-Geheimnis]**. Sie geben diese in Adobe Exchange (**[!UICONTROL )]**.

### Notieren Sie sich Ihre Marketo REST API-Basis-URL

1. Öffnen Sie **[!UICONTROL Admin]** unter **[!UICONTROL Integration]** die Option **[!UICONTROL Web-Services]**.
1. Suchen Sie den **[!UICONTROL REST API]**-Endpunkt. Kopieren Sie nur die **Basis-URL** (Host) in die `https://###-XXX-###.mktorest.com`. Fügen **Pfadsegmente** z. B. `/rest` oder `/identity` ein. Dieser Wert ist pro Marketo-Instanz eindeutig.

![Basis-URL des Web Services REST-API-Endpunkts](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

Sie benötigen außerdem die **[!UICONTROL Marketo Engage Identity URL]** die Ihr Exchange-Bereitstellungsbildschirm anfordert, zusammen mit der REST-Basis-URL sowie der Client-ID und dem Client Secret von LaunchPoint.

## Anwendung von Exchange bereitstellen

Um die Erweiterung in GenStudio verfügbar zu machen, stellen Sie die App über Adobe Exchange bereit.

1. Kehren Sie zu [Adobe Exchange &#x200B;](https://exchange.adobe.com).
1. Wählen Sie **[!UICONTROL Verwalten]** und öffnen Sie die Anwendung **Marketo für GenStudio** (z. B. unter **[!UICONTROL App Builder-Anwendungen]** oder den verwalteten Programmen Ihres Unternehmens).
1. Wählen **[!UICONTROL unter &quot;]**&quot; eine vorhandene Umgebung aus dem Dropdown-Menü aus oder wählen Sie **[!UICONTROL Umgebung hinzufügen]**, um eine Umgebung zu erstellen.
1. Öffnen Sie **[!UICONTROL Konfiguration]** für die ausgewählte Umgebung.
1. Geben Sie die **[!UICONTROL Client-ID]** und **[!UICONTROL Client-Geheimnis]** aus [LaunchPoint](#create-or-select-a-launchpoint-service), die **[!UICONTROL Marketo Engage Identity URL]** und die **[!UICONTROL Marketo Engage REST API-Basis-URL]** (der Basis-Host aus [Web Services](#note-your-marketo-rest-api-base-url)) sowohl für die Marketo Engage Identity URL (&#x200B;) als auch für die Marketo Engage REST API-Basis-URL ein.
1. Klicken Sie auf **[!UICONTROL Bereitstellen]**. Nach erfolgreicher Bereitstellung ändert sich die Aktion in **[!UICONTROL Bereitstellung aufheben]**.

### Konfiguration aktualisieren

Um die Konfigurationswerte für eine Umgebung zu ändern **[!UICONTROL aktualisieren Sie zunächst]** Felder und anschließend erneut **[!UICONTROL Bereitstellen]**.

### Workspace-Konfiguration (optional)

Sie können diesen Schritt überspringen, wenn Sie den Standardarbeitsbereich verwenden möchten. Standardmäßig sind die Felder **Workspace ID** und **Vorlagenlisten-**) vorkonfiguriert.

Wenn Sie jedoch Vorlagen aus einem anderen Arbeitsbereich abrufen müssen:

1. Navigieren Sie in Marketo zu **[!UICONTROL Admin]** → **[!UICONTROL Sicherheit]** → **[!UICONTROL Arbeitsbereiche und Partitionen]**.
1. Die Spalte **Workspace ID** ist standardmäßig ausgeblendet. Um sie zu aktivieren, klicken Sie mit der rechten Maustaste auf die Kopfzeile (in der Spaltennamen angezeigt werden).
1. Wählen Sie **[!UICONTROL Spalten]** aus.
1. Aktivieren Sie **[!UICONTROL ID]** aus der Liste.
   ![Arbeitsbereiche und Partitionen mit aktivierter Workspace ID-Spalte](/help/extensibility/marketo-workspace-id.png){width="80%"}

Sobald sie angezeigt wird, verwenden Sie die entsprechende **Workspace ID** für Ihre Konfiguration.

## Zugriff auf Marketo-Vorlagen in GenStudio

Nachdem Marketo für GenStudio installiert und konfiguriert wurde, wird beim Erstellen eines E-Mail **-Erlebnisses in GenStudio die**&#x200B;**Marketo-Vorlagen** angezeigt. Verwenden Sie diese Registerkarte, um Vorlagen aus Marketo Engage zu durchsuchen.

>[!IMPORTANT]
>
>Erstellen Sie E-Mails unter dem **Standard-E-Mail**-Erlebnisfluss in GenStudio for Performance Marketing. Diese Integration unterstützt KEINE E-Mails, die mit dem neuen E-Mail-Editor erstellt wurden.

![Exchange-Konfiguration mit Marketo-Anmeldeinformationen](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## Fehlerbehebung

### Die Registerkarte Marketo-Vorlagen wird nicht angezeigt

* Vergewissern Sie sich, **die App in** Exchange genehmigt“ ist und die Umgebung **bereitgestellt** mit gültigen Client-ID-, Client-Geheimnis- und Marketo-Basis-URLs bereitgestellt wird.
* Bitten Sie Ihren Administrator, bei der Erstellung der Anmeldeinformationen **Zugriff auf den** Marketo-Produktadministrator zu überprüfen.

### Vorlagen werden nicht geladen

* Laden Sie die Seite neu oder melden Sie sich ab und wieder bei GenStudio an.
* Suchen Sie im Bedienfeld **[!UICONTROL Netzwerk]** der Browser-Entwicklertools nach fehlgeschlagenen API-Aufrufen an Ihre Marketo-Instanz und überprüfen Sie, ob die REST-Basis-URL mit **[!UICONTROL Webservices]** in Marketo übereinstimmt (kein zusätzlicher Pfad nach dem Host).

### Fehler „Keine Vorlagen gefunden“

Wenn die Erweiterung erfolgreich installiert wurde und die Registerkarte Marketo-Vorlagen angezeigt wird, jedoch „Keine Vorlagen gefunden“ angezeigt wird, kann das Problem dadurch verursacht werden, dass die Anwendung beim Rendern von Vorlagen die Größenbeschränkungen überschreitet, was zu einem Absturz führt.
So beheben Sie das Problem:

1. Bereitstellung der Anwendung in Exchange aufheben.
1. Verringern Sie die Seitengröße der Vorlagenliste (legen Sie sie beispielsweise auf 1 oder 2 fest).
1. Stellen Sie die Anwendung erneut bereit.
