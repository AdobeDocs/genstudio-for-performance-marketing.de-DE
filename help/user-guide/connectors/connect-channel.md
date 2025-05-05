---
title: Bezahlte Medien verbinden
description: Ein Kanalkonto verbinden, um Anzeigen und Medien mit Adobe GenStudio for Performance Marketing zu aktivieren und zu überwachen.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: cf4be61925761c9630cb8ea5c995d017b3938a31
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Paid-Media-Konten verbinden

_[!DNL Data connectors]_&#x200B;ermöglichen die nahtlose Integration zwischen GenStudio for Performance Marketing und Ihren Paid-Media-Netzwerkkonten. Durch die Verbindung mit Kanalkonten von Drittanbietern können Sie wichtige Daten wie Kampagnenleistungsmetriken in [[!DNL Insights]](/help/user-guide/insights/overview.md) austauschen und neue Anzeigenplatzierungen mit [[!DNL Activate]](/help/user-guide/activation/overview.md) bereitstellen. Durch diese Integration kann GenStudio for Performance Marketing Ihre Medien und Anzeigen verwalten und gleichzeitig wertvolle Einblicke, einschließlich Impressionen, Klicks und Konversionen, aus Ihren aktiven Kampagnen erhalten.

**So stellen Sie eine Verbindung zu einem Paid-Media-Konto her**:

1. Klicken Sie auf die **[!UICONTROL mit den Auslassungspunkten … Mehr]** in der linken unteren Navigationsleiste.

1. Wählen Sie **[!UICONTROL Einstellungen]** mit dem Zahnradsymbol aus.

1. Wählen _[!UICONTROL in]_ einen Connector-Typ aus dem Abschnitt _[!UICONTROL Data Connectors]_ und klicken Sie auf **[!UICONTROL Verbinden]**.

   Wenn verbundene Konten vorhanden sind, können Sie optional auf _Verbundene Konten_ klicken, um eine Liste mit Kontonamen, Details und Status anzuzeigen.

1. Überprüfen Sie [ ausgewählten Connector](#connector-types)Typ, überprüfen Sie die Voraussetzungen und fahren Sie mit den Verbindungsschritten fort.

## Bezahlte Medienverbindungen

GenStudio for Performance Marketing unterstützt verschiedene Connector-Typen für die Integration mit Ihren bevorzugten Marketing-Plattformen. Für jeden Connector-Typ sind bestimmte Voraussetzungen und Einrichtungsschritte erforderlich, die für eine erfolgreiche Verbindung ausgeführt werden müssen.

### Google Campaign Manager 360 Connect

>[!BEGINSHADEBOX]

**Voraussetzungen**:

- Google Campaign Manager 360-Konto
- Entfernen Sie alle Popup-Blocker in Ihrem Browser

>[!ENDSHADEBOX]

**So verbinden Sie ein Google Campaign Manager 360-Konto**:

1. Klicken Sie im Abschnitt _Data Connectors_ auf **[!UICONTROL Verbinden]** auf der Karte _Google Campaign Manager 360_ .

1. Melden Sie sich bei Ihrem Google Campaign Manager 360-Konto an.

   Möglicherweise müssen Sie die Popup-Blocker entfernen und dann mit &quot;**[!UICONTROL &quot;]**, um es erneut zu versuchen.

1. Lesen Sie die Nutzungsbedingungen und klicken Sie auf **[!UICONTROL Zulassen]**, um Zugriff zu gewähren.

1. Wählen Sie in der Ansicht _[!UICONTROL Google Campaign Manager 360]_ einen oder mehrere Advertiser aus und klicken Sie auf **[!UICONTROL Auswählen]**.

Die Ansicht _[!UICONTROL Google Campaign Manager 360-Konten]_ listet die `Account name`, `Added by`, `Date added` und `Status` auf. Verwenden **[!UICONTROL Konto hinzufügen]**, um der Liste weitere Konten hinzuzufügen.

### Meta-Anzeigen verbinden

Wenn Sie Ihr _Meta Business_-Profil mit GenStudio for Performance Marketing verbinden, sorgt dies für den nahtlosen Zugriff auf Werbedaten für Ihre Geschäftsseiten, Meta Ads-Konten und andere Meta-Assets.

>[!BEGINSHADEBOX]

**Voraussetzungen**:

- Facebook-/Meta-Anmeldung, die auf alle Meta-Services zugreifen kann, z. B. Meta Ads-Konto und Facebook-Geschäftsprofil
- Zugriff auf das Meta Ads-Konto mit `View performance` Berechtigungsstufe für den Zugriff auf Berichte und das Anzeigen von Anzeigen, einschließlich der folgenden
   - Für die Verwendung mit [!DNL Insights] erforderliche Berechtigungen:

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - Für die Verwendung mit [!DNL Activate] erforderliche Berechtigungen:

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- Entfernen Sie alle Popup-Blocker in Ihrem Browser

>[!ENDSHADEBOX]

**So verbinden Sie ein Meta Ads-Konto**:

1. Klicken _Abschnitt „Data Connectors_ auf **[!UICONTROL Verbinden]** auf der _Meta Ads_-Karte.

1. Melden Sie sich bei Ihrem Facebook-Konto an.

   Möglicherweise müssen Sie die Popup-Blocker entfernen und dann mit &quot;**[!UICONTROL &quot;]**, um es erneut zu versuchen.

1. Befolgen Sie die Anweisungen zur Facebook-Authentifizierung, überprüfen Sie die Kontoinformationen und klicken Sie auf **[!UICONTROL Weiter als …]**

1. Gehen Sie _[!UICONTROL Facebook-Anmeldung für Unternehmen]_ (Metasymbol für Adobe) durch die folgenden Auswahlen, um GenStudio for Performance Marketing Zugriff zu gewähren:

   - Wählen Sie ein oder mehrere Meta Business-Profile aus und klicken Sie auf **[!UICONTROL Weiter]**
   - Wählen Sie eine oder mehrere Meta-Seiten aus und klicken Sie auf **[!UICONTROL Weiter]**
   - Wählen Sie ein oder mehrere Instagram-Konten aus und klicken Sie auf **[!UICONTROL Weiter]**
   - Überprüfen Sie die Auswahl und klicken Sie auf **[!UICONTROL Speichern]**

1. Sobald Sie die Bestätigung erhalten haben, dass Ihr Konto verbunden ist, klicken Sie auf **[!UICONTROL Verstanden]**.

   Dieser Schritt stellt sicher, dass GenStudio for Performance Marketing Zugriff auf alle Anzeigen, Metadaten und Metriken erhält, um eine optimale Leistung zu erzielen.

1. Wählen _[!UICONTROL in &quot;]_&quot; ein oder mehrere Konten aus, die in [!DNL Insights] aufgenommen werden sollen, und klicken Sie auf **[!UICONTROL Auswählen]**.

1. Sobald Sie eine Bestätigung für _Platform Connected_ erhalten haben, klicken Sie auf **[!UICONTROL Konten anzeigen]**.

   Die _[!UICONTROL Meta Ads-Konten]_ listet die `Account name`, `Added by`, `Date added` und `Status` auf.

Verwenden **[!UICONTROL Konto hinzufügen]**, um der Liste weitere Konten hinzuzufügen. Der Autorisierungsfluss kann beim Hinzufügen von Konten, die mit demselben Meta Business-Profil verknüpft sind, geringfügig abweichen. Sie wählen während des Verbindungsprozesses nur die neuen Meta Ads-Konten aus.

## Datenaufnahme

Zunächst importiert GenStudio for Performance Marketing die historischen Daten der letzten sechs Monate. Dadurch wird sichergestellt, dass Sie sofortigen Zugriff auf relevante Einblicke haben, um Trends zu analysieren, die Leistung zu bewerten und fundierte Entscheidungen zu treffen. Der Aufnahmevorgang kann je nach Datenvolumen in Ihrem Konto ein bis fünf Tage dauern.

>[!BEGINSHADEBOX]

**Richtlinie zur Datenaufnahme und -speicherung**

GenStudio for Performance Marketing bewahrt Kanaldaten 13 Monate lang auf. Diese Aufbewahrungsrichtlinie umfasst die 6 Monate an Daten, die während der ersten Verbindung aufgenommen wurden, um eine umfassende historische Datenanalyse und Berichterstellung sicherzustellen.

>[!ENDSHADEBOX]
