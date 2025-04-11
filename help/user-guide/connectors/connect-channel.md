---
title: Bezahlte Medien verbinden
description: Ein Kanalkonto verbinden, um Anzeigen und Medien mit Adobe GenStudio for Performance Marketing zu aktivieren und zu überwachen.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Paid-Media-Konten verbinden

_[!DNL Data connectors]_ermöglichen die nahtlose Integration zwischen GenStudio for Performance Marketing und Ihren Paid-Media-Netzwerkkonten. Durch die Verbindung mit Kanalkonten von Drittanbietern können Sie wichtige Daten wie Kampagnenleistungsmetriken in [[!DNL Insights]](/help/user-guide/insights/overview.md) austauschen und neue Anzeigenplatzierungen mit [[!DNL Activate]](/help/user-guide/activation/overview.md) bereitstellen. Durch diese Integration kann GenStudio for Performance Marketing Ihre Medien und Anzeigen verwalten und gleichzeitig wertvolle Einblicke, einschließlich Impressionen, Klicks und Konversionen, aus Ihren aktiven Kampagnen erhalten.

**So stellen Sie eine Verbindung zu einem Paid-Media-Konto her**:

1. Klicken Sie auf die **[!UICONTROL mit den Auslassungspunkten … Mehr]** in der linken unteren Navigationsleiste.

1. Wählen Sie **[!UICONTROL Einstellungen]** mit dem Zahnradsymbol aus.

1. Wählen _[!UICONTROL in]_ einen Connector-Typ aus dem Abschnitt _[!UICONTROL Data Connectors]_ und klicken Sie auf **[!UICONTROL Verbinden]**.

   Wenn verbundene Konten vorhanden sind, können Sie optional auf _Verbundene Konten_ klicken, um eine Liste mit Kontonamen, Details und Status anzuzeigen.

1. Überprüfen Sie [ ausgewählten Connector](#connector-types)Typ, überprüfen Sie die Voraussetzungen und fahren Sie mit den Verbindungsschritten fort.

## Bezahlte Medienverbindungen

GenStudio for Performance Marketing unterstützt verschiedene Connector-Typen für die Integration mit Ihren bevorzugten Marketing-Plattformen. Für jeden Connector-Typ sind bestimmte Voraussetzungen und Einrichtungsschritte erforderlich, die für eine erfolgreiche Verbindung ausgeführt werden müssen.

### Meta-Anzeigen verbinden

>[!BEGINSHADEBOX]

**Voraussetzungen**:

- Facebook-/Meta-Werbekonto
- Zugriff auf das Meta-Anzeigen-Konto mit `View performance` Berechtigungsstufe für den Zugriff auf Berichte und das Anzeigen von Anzeigen
- Entfernen Sie alle Popup-Blocker in Ihrem Browser

>[!ENDSHADEBOX]

**So verbinden Sie ein Meta Ads-Konto**:

1. Klicken _Abschnitt „Data Connectors_ auf **[!UICONTROL Verbinden]** auf der _Meta Ads_-Karte.

1. Melden Sie sich bei Ihrem Facebook-Konto an.

   Möglicherweise müssen Sie die Popup-Blocker entfernen und dann mit &quot;**[!UICONTROL &quot;]**, um es erneut zu versuchen.

1. Befolgen Sie die Anweisungen zur Facebook-Authentifizierung.

1. Gehen Sie _[!UICONTROL Pop-up „Facebook-Anmeldung für]_&quot; (Meta-zu-Adobe-Symbol) durch die folgenden Auswahlen.

   - Überprüfen Sie die Kontoinformationen und klicken Sie auf **[!UICONTROL Weiter als]**
   - Gewähren Sie Zugriff auf ausgewählte Seiten und klicken Sie auf **[!UICONTROL Weiter]**
   - Gewähren Sie ausgewählten Unternehmen Zugriff und klicken Sie auf **[!UICONTROL Weiter]**
   - Melden Sie sich bei einem oder mehreren Instagram-Konten an und klicken Sie auf **[!UICONTROL Weiter]**
   - Überprüfen Sie die Auswahl und klicken Sie auf **[!UICONTROL Speichern]**

1. Wählen _[!UICONTROL in der Ansicht]_ Meta-Anzeigen“ mindestens ein Konto aus und klicken Sie auf **[!UICONTROL Auswählen]**.

Die _[!UICONTROL Meta Ads-Konten]_ listet die `Account name`, `Added by`, `Date added` und `Status` auf. Verwenden **[!UICONTROL Konto hinzufügen]**, um der Liste weitere Konten hinzuzufügen.

## Datenaufnahme

Zunächst importiert GenStudio for Performance Marketing die historischen Daten der letzten sechs Monate. Dadurch wird sichergestellt, dass Sie sofortigen Zugriff auf relevante Einblicke haben, um Trends zu analysieren, die Leistung zu bewerten und fundierte Entscheidungen zu treffen. Der Aufnahmevorgang kann je nach Datenvolumen in Ihrem Konto ein bis fünf Tage dauern.

>[!BEGINSHADEBOX]

**Richtlinie zur Datenaufnahme und -speicherung**

GenStudio for Performance Marketing bewahrt Kanaldaten 13 Monate lang auf. Diese Aufbewahrungsrichtlinie umfasst die 6 Monate an Daten, die während der ersten Verbindung aufgenommen wurden, um eine umfassende historische Datenanalyse und Berichterstellung sicherzustellen.

>[!ENDSHADEBOX]
