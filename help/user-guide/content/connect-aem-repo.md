---
title: "Verbindung zu einem [!DNL AEM Assets Content Hub] Repository herstellen"
description: Erfahren Sie, wie Sie Adobe GenStudio for Performance Marketing mit einem Adobe Experience Manager (AEM) [!DNL Content Hub] Repository verbinden und vorhandene genehmigte Inhalte nutzen.
level: Experienced
feature: Assets, Content
source-git-commit: 82ac164cb852305fce206845d15f04c4b4395387
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Herstellen einer Verbindung zu einem [!DNL AEM Assets Content Hub]-Repository

Wenn Sie Assets in Adobe Experience Manager (AEM) haben, können Sie diese Schritte ausführen, um sie in GenStudio for Performance Marketing verfügbar zu machen.

>[!BEGINSHADEBOX]

**Voraussetzungen**:

Die folgenden Schritte erfordern Administratorzugriff auf Admin Console und AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Schritt 1: Aktivieren Sie [!DNL AEM Assets Content Hub]

Führen Sie den Self-Service-Prozess **Content Hub bereitstellen** aus, um [!DNL Content Hub] für Ihre vorhandene AEM Assets in Cloud Manager zu aktivieren. Siehe [Bereitstellen [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) in der Dokumentation zu _AEM as a Cloud Service_.

Nachdem Sie [!DNL AEM Assets Content Hub] aktiviert haben, haben Sie eine neue Instanz mit dem Suffix `contenthub` innerhalb von [!DNL AEM Assets as a Cloud Service] auf der Admin Console.

>[!IMPORTANT]
>
>Administratoren sollten sicherstellen, dass sich das [!DNL AEM Assets Content Hub] -Repository in derselben Organisation wie GenStudio for Performance Marketing befindet.

## Schritt 2: Onboard GenStudio-Benutzer

Fügen Sie unter &quot;[!DNL Admin Console]&quot;einen GenStudio for Performance Marketing-Benutzer oder eine Benutzergruppe zum Produktprofil &quot;[!DNL AEM Assets Content Hub]&quot;hinzu. Wenn ein Inhaltsvalidierer keinen Zugriff auf dieselbe Organisation wie das [!DNL AEM Assets Content Hub]-Repository hat, kann es bei der Überprüfung und Genehmigung von Inhalten zu Problemen kommen.

- [Onboard [!DNL Content Hub] administrator](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Onboard [!DNL Content Hub] users](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Schritt 3: Genehmigen von Assets

Genehmigen Sie Assets zur Verwendung in [!DNL AEM Assets Content Hub], wodurch sie in GenStudio for Performance Marketing verfügbar gemacht werden.

Siehe [Genehmigen von Assets in Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) in der Dokumentation zu _AEM as a Cloud Service_ .

## Schritt 4: Konfigurieren der Asset-Sichtbarkeit

Überprüfen Sie in den Konfigurationsoptionen für _[!DNL AEM Assets Content Hub]_die einzelnen Konfigurationsoptionen für Filter, Asset-Details, Suche und Branding.

Siehe [Konfigurieren der Content Hub-Benutzeroberfläche](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) in der Dokumentation zu _AEM as a Cloud Service_ .

## Schritt 5: Verbindung überprüfen

In GenStudio for Performance Marketing Content ist die Liste _[!UICONTROL Position]_ rechts über der Galerie verfügbar. Die Liste ist nicht verfügbar, wenn Sie keinen Zugriff haben oder Ihr Unternehmen kein [!DNL AEM Assets Content Hub] -Repository bereitgestellt und verbunden hat.
