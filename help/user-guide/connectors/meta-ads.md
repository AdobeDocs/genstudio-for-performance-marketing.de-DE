---
title: Mit Meta Ads verbinden
description: Verbinden Sie ein Meta Ads-Konto, um Ihre Anzeigen und Medien mit Adobe GenStudio for Performance Marketing zu aktivieren und zu überwachen.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: 40c7d2d40f1c4bea9794e706d8e1ce7bf92042e3
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Mit Meta Ads verbinden

Auf dieser Seite wird beschrieben, wie Sie Ihr Meta Ads-Profilkonto mit GenStudio for Performance Marketing verbinden und verwalten können, um Kampagnen zu verwalten, Inhalte zu exportieren und auf Werbedaten für Ihre aktiven Kampagnen zuzugreifen.

>[!BEGINSHADEBOX]

**Voraussetzungen**:

- Anmeldung bei Facebook/Meta, die auf alle Meta-Services zugreifen kann

- _Vollständige Kontrolle_ über Meta Business Portfolio und Werbekonten, einschließlich:

   - Verwalten von Kampagnen
   - Leistung anzeigen
   - Verwalten von Creative Hub-Mockups
   - Erweiterte Analyse

- Deaktivieren Sie alle Popup-Blocker in Ihrem Browser

>[!ENDSHADEBOX]

## Verbinden eines Meta Ads-Kontos

1. Klicken Sie auf **[!UICONTROL Mehr]** > **[!UICONTROL Einstellungen]**.

1. Klicken Sie im Abschnitt _Data Connectors_ auf **[!UICONTROL Verbinden]** der Karte _Meta Ads_.

1. Melden Sie sich bei Ihrem Facebook-Konto an.

   Möglicherweise müssen Sie die Popup-Blocker entfernen und dann mit &quot;**[!UICONTROL &quot;]**, um es erneut zu versuchen.

1. Befolgen Sie die Anweisungen zur Facebook-Authentifizierung, überprüfen Sie die Kontoinformationen und klicken Sie auf **[!UICONTROL Weiter als …]**

1. Gehen Sie _[!UICONTROL Facebook-Anmeldung für Unternehmen]_ (Symbol &quot;Meta zu Adobe„) durch die folgenden Auswahlen, um GenStudio for Performance Marketing Zugriff zu gewähren:

   - Wählen Sie mindestens ein Meta-Geschäftsprofil aus und klicken Sie auf **[!UICONTROL Weiter]**
   - Wählen Sie mindestens eine Meta-Seite aus und klicken Sie auf **[!UICONTROL Weiter]**
   - Wählen Sie ein oder mehrere Instagram-Konten aus und klicken Sie auf **[!UICONTROL Weiter]**
   - Überprüfen Sie die Auswahl und klicken Sie auf **[!UICONTROL Speichern]**

     ![Auswahlen überprüfen](/help/assets/meta/meta-review-selections.png "Auswahlen überprüfen"){width="400" zoomable="yes"}

1. Sobald Sie die Bestätigung erhalten haben, dass Ihr Konto verbunden ist, klicken Sie auf **[!UICONTROL Verstanden]**.

   Dieser Schritt stellt sicher, dass GenStudio for Performance Marketing Zugriff auf alle Anzeigen, Metadaten und Metriken erhält, um eine optimale Leistung zu erzielen.

1. Wählen Sie in _[!UICONTROL Meta Ads]_ ein oder mehrere Konten aus, die in [!DNL Insights] aufgenommen werden sollen, und klicken Sie auf **[!UICONTROL Auswählen]**.

1. Sobald Sie eine Bestätigung für _Platform Connected_ erhalten haben, klicken Sie auf **[!UICONTROL Konten anzeigen]**.

   Die Ansicht _[!UICONTROL Meta Ads]_ listet die `Account name`, `Added by`, `Date added` und `Status` auf.

   ![Liste der Meta](/help/assets/meta/meta-accounts-list.png "Konten/Liste der verbundenen Meta-Konten"){zoomable="yes"}

Verwenden **[!UICONTROL Konto hinzufügen]**, um der Liste weitere Konten hinzuzufügen. Der Autorisierungsfluss kann beim Hinzufügen von Konten, die mit demselben Meta-Geschäftsprofil verknüpft sind, geringfügig abweichen. Sie wählen während des Verbindungsprozesses nur die neuen Meta Ads-Konten aus.

## Trennen und Fehlerbehebung bei einer Meta Ads-Integration

Manchmal ist eine GenStudio for Performance Marketing-Instanz falsch mit einem Meta Ads-Konto verbunden. Zu den häufigen Setups, die Probleme verursachen können, gehören:

- Ein Instagram-Konto wird ohne die zugehörige Facebook-Seite ausgewählt
- hat einem Benutzer, der die ursprüngliche Verbindung hergestellt hat, die Berechtigungen entzogen

In diesen Situationen ist es am besten, das Meta Ad-Konto erneut mit der GenStudio for Performance Marketing-Instanz zu verbinden. Zunächst muss die Benutzerin bzw. der Benutzer die App-Integration direkt aus ihrem Meta Business Manager entfernen, um einen Neuanfang für das Zurücksetzen von Berechtigungen zu schaffen. Dies erfordert Administratorzugriff auf den Meta Business Manager.

Mit diesen Schritten werden zwischengespeicherte Berechtigungen gelöscht und der Integrationsfluss zurückgesetzt:

1. Greifen Sie auf [Meta Business Manager](https://business.facebook.com) zu, indem Sie die Facebook-Website besuchen.
1. Melden Sie sich mit Ihrem Konto an. Das Konto muss Administratorzugriff auf den Business Manager haben.
1. Klicken Sie auf **[!UICONTROL Einstellungen]** Zahnradsymbol unten links, um zu Ihren Portfolio-Einstellungen für Ihr Unternehmen zu navigieren.
1. Klicken Sie im Menü links auf &quot;**[!UICONTROL &quot;]**.
1. Wählen Sie **[!UICONTROL Verbundene Apps]** aus. Adobe GenStudio wird in der Liste der verbundenen Apps angezeigt.
   ![Mit Meta Business Manager verbundene Apps](./meta-connected-apps.png "Bereich für mit Meta Business Manager verbundene Apps")
1. Klicken Sie auf den App-Namen.
1. Klicken Sie auf **[!UICONTROL Entfernen]**.
1. Bestätigen Sie die Entfernung, wenn Sie dazu aufgefordert werden.

Sie können jetzt Ihre Meta-Werbekonten, Instagram-Profile und Facebook-Seiten neu verbinden.
