---
title: Herstellen einer Verbindung zu einem  [!DNL AEM Assets Content Hub] -Repository
description: Erfahren Sie, wie Sie Adobe GenStudio for Performance Marketing mit einem Adobe Experience Manager (AEM)- [!DNL Content Hub]  verbinden und vorhandene genehmigte Inhalte nutzen können.
level: Experienced
role: Admin, Developer
feature: Content Management
recommendations: noDisplay
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
TQID: https://experienceleague.adobe.com/FJ6G7qlBlkrsGk1H7SHhlkqHUHYYGKkTqklTeGDxJho
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 387
ht-degree: 3%

---

# Herstellen einer Verbindung zu einem [!DNL AEM Assets Content Hub] Repository

Wenn Sie Assets in Adobe Experience Manager (AEM) haben, können Sie diese Schritte ausführen, um sie in GenStudio for Performance Marketing verfügbar zu machen.

>[!BEGINSHADEBOX]

**Voraussetzungen**:

Für die folgenden Schritte ist ein administrativer Zugriff auf Admin Console und AEM Assets as a Cloud Service erforderlich.

>[!ENDSHADEBOX]

## Schritt 1: [!DNL AEM Assets Content Hub] aktivieren

Befolgen Sie **Selbstbedienungsprozess &quot;Content Hub bereitstellen** um [!DNL Content Hub] für Ihre bestehende AEM Assets in Cloud Manager zu aktivieren. Siehe [Bereitstellen [!DNL Content Hub]](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) in der Dokumentation zu _AEM as a Cloud Service_.

Nach der Aktivierung von [!DNL AEM Assets Content Hub] haben Sie eine neue Instanz mit dem `contenthub` Suffix in [!DNL AEM Assets as a Cloud Service] auf Admin Console.

>[!IMPORTANT]
>
>Admins sollten sicherstellen, dass sich das [!DNL AEM Assets Content Hub]-Repository in derselben Organisation wie GenStudio for Performance Marketing befindet.

## Schritt 2: Onboarding von GenStudio-Benutzern

Fügen Sie in der [!DNL Admin Console] einen GenStudio for Performance Marketing-Benutzer oder eine -Benutzergruppe zum [!DNL AEM Assets Content Hub] Produktprofil hinzu. Wenn ein Content Reviewer nicht auf dieselbe Organisation wie das [!DNL AEM Assets Content Hub]-Repository zugreifen kann, kann es zu Schwierigkeiten bei der Überprüfung und Genehmigung von Inhalten kommen.

- [Onboard [!DNL Content Hub] administrator](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Onboard [!DNL Content Hub] users](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Schritt 3: Assets genehmigen

Genehmigen von Assets für die Verwendung in [!DNL AEM Assets Content Hub], wodurch sie in GenStudio for Performance Marketing verfügbar werden.

Siehe [Genehmigen von Assets in Experience Manager](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) in der _AEM as a Cloud Service_-Dokumentation.

## Schritt 4: Asset-Sichtbarkeit konfigurieren

Überprüfen Sie unter _[!DNL AEM Assets Content Hub]_&#x200B;Konfigurationsoptionen jeden Satz von Konfigurationsoptionen für Filter, Asset-Details, Suche und Branding.

Siehe [Konfigurieren der Benutzeroberfläche von Content Hub](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) in der Dokumentation zu _AEM as a Cloud Service_.

## Schritt 5: Verbindung überprüfen

Im GenStudio for Performance Marketing-Inhalt _[!UICONTROL die Liste]_ Speicherort“ über der Galerie auf der rechten Seite verfügbar. Die Liste ist nicht verfügbar, wenn Sie keinen Zugriff haben oder Ihre Organisation kein [!DNL AEM Assets Content Hub]-Repository bereitgestellt und verbunden hat.

Siehe [Speicherort in Assets](manage-assets.md#assets-location), um mehr über die Liste der Speicherorte und das Ändern von Repositorys zu erfahren.
