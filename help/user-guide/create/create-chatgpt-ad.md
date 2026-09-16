---
title: Erstellen eines Chat-GPT-Anzeigen-Erlebnisses
description: Erfahren Sie, wie Sie Paid-Media-Erlebnisse mit ChatGPT in Adobe GenStudio for Performance Marketing erstellen, überprüfen, veröffentlichen und aktivieren können.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 9%
---

# Erstellen eines ChatGPT-Werbeerlebnisses

Verwenden Sie [[!DNL Create]](/help/user-guide/create/overview.md) in [!DNL GenStudio for Performance Marketing], um **ChatGPT-Anzeigen** als Erlebnisse für bezahlte Medien zu erstellen, von Richtlinien und Assets über Generierung, Marken- und Kanalprüfungen, Genehmigung, Veröffentlichung in [!DNL Content] und Aktivierung im selben [!DNL Activate], der für Kanäle wie Meta und Google Campaign Manager 360 verwendet wird.

Bevor Sie beginnen, fügen [ bei ](/help/user-guide/guidelines/add-guidelines.md) Richtlinien hinzu und überprüfen Sie [effektive Aufforderungen](/help/user-guide/effective-prompts.md) sodass Ihre Headline-Aufforderungen starke Varianten ergeben.

## Voraussetzungen

Sie müssen entsprechend diesen Voraussetzungen eingerichtet sein, bevor Sie ChatGPT-Anzeigen in [!DNL GenStudio for Performance Marketing] erstellen oder aktivieren.

### Zugriff und Rollen

* Sie haben eine **Editor**-Rolle oder eine höhere in [!DNL GenStudio for Performance Marketing]. Siehe [Benutzerrollen und Berechtigungen](/help/user-guide/user-roles.md).
* Sie haben ein **OpenAI Ad-Konto** und einen **API-Schlüssel** aus diesem Konto.
* Ein **ChatGPT Ads**-Konto ist mit [!DNL GenStudio for Performance Marketing] verbunden.

So erstellen Sie einen API-Schlüssel in OpenAI Ads Manager:

1. Navigieren Sie in OpenAI Ads Manager zu **[!UICONTROL Einstellungen]** > **[!UICONTROL API-Schlüssel]** > **[!UICONTROL Neuen Schlüssel erstellen]**.

So verbinden Sie Ihr ChatGPT Ads-Konto mit [!DNL GenStudio for Performance Marketing]:

1. Klicken Sie unten links auf **[!UICONTROL Mehr]** > **[!UICONTROL Einstellungen]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Verbinden]** > **[!UICONTROL Konto hinzufügen]**.
1. Geben Sie den Namen Ihres OpenAI-Werbekontos ein, fügen Sie Ihren API-Schlüssel ein und klicken Sie auf **[!UICONTROL Konto hinzufügen]**.

Ihr Werbekonto ist verbunden, wenn der Fluss erfolgreich abgeschlossen wurde.

### Erstellen einer Konfiguration

* **[!DNL Brands]**, **[!DNL Products]** und **[!DNL Personas]** sind so konfiguriert, dass die App eine markeninterne Kopie erzeugen kann. Siehe [Richtlinien - Übersicht](/help/user-guide/guidelines/overview.md).
* Die gewünschten Bilder sind in [[!DNL Content]](/help/user-guide/content/overview.md) verfügbar.

## Erstellen einer ChatGPT-Anzeige

Sie erstellen ChatGPT-Anzeigen als Paid-Media-Erlebnisse im [!DNL Create] Workspace.

### ChatGPT-Erlebnis starten

So öffnen Sie die ChatGPT-Erstellung:

1. Navigieren Sie **[!UICONTROL Erstellen]** > **[!UICONTROL ChatGPT]**. Sie wählen keine Vorlagen für ChatGPT aus. Es wird ein einzelnes Anzeigenlayout verwendet.
   ![ChatGPT-Kachel im Erstellungs-Workflow](./create-chatgpt-clp.png){width="60%"}
1. Treffen Sie auf _Arbeitsfläche_ Auswahlen für **[!DNL Brand]**, **[!DNL Product]**, **[!DNL Persona]** und **Sprache**.
1. Wählen Sie ein Bild aus [!DNL Content] aus.
1. Geben Sie eine Eingabeaufforderung für Ihre ChatGPT-Überschriftenkopie ein.
1. Klicken Sie auf **[!UICONTROL Generieren]**.

[!DNL GenStudio for Performance Marketing] **generiert** kreative Varianten.

Sie haben folgende Möglichkeiten:

* Mit **[!UICONTROL Regenerieren]** oder **[!UICONTROL Verfeinern]** können Sie Ton, Länge oder Hervorhebung anpassen.
* Bearbeiten Sie Text direkt auf der _Arbeitsfläche_.
* Verwenden Sie **[!UICONTROL Swap]**, um ein alternatives Bild aus [!DNL Content] auszuwählen.

Unter [Verwalten von Varianten](/help/user-guide/create/manage-variants.md) finden Sie weitere Möglichkeiten, generierte Erlebnisse zu bearbeiten.

### Durchführen von Marken- und Kanalprüfungen

Validieren Sie vor dem Speichern oder Senden des Erlebnisses zur Überprüfung das Kopieren und Layout anhand der Marken- und Kanalregeln.

So führen Sie Inhaltsprüfungen durch:

1. Klicken Sie **[!UICONTROL Inhaltsüberprüfung]** (Marken- und Kanalprüfungen).
1. Überprüfen Sie die Validierungsergebnisse im Bedienfeld [_Inhaltsüberprüfung_ ](/help/user-guide/guidelines/brand-validation.md#content-check-panel).
1. Beheben Sie alle gemeldeten Probleme (z. B. Kopierlänge oder dichten Text auf dem Bildschirm), indem Sie Varianten bearbeiten oder nach Bedarf neu generieren.

Siehe [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md).

## Speichern einer ChatGPT-Anzeige in [!DNL GenStudio for Performance Marketing]

Durch das Speichern wird Ihr ChatGPT-Anzeigen-Erlebnis in [!DNL Content] verschoben, damit es überprüft, wiederverwendet und aktiviert werden kann.

Es gibt zwei Status:

* **Erfahrungsentwurf**: Laufende Arbeiten und nicht genehmigte Arbeiten.
* **Veröffentlichtes Erlebnis**: Genehmigt und zur Aktivierung in [!DNL Content] verfügbar.

### Zur Überprüfung senden

1. Klicken Sie in der Kopfzeile des Erlebnisses auf **[!UICONTROL Überprüfung anfordern]**.
1. Wählen Sie genehmigende Personen aus (z. B. markenrechtliche, rechtliche oder Leistungs-Stakeholder).
1. Optional: Fügen Sie in „Einstellungen **[!UICONTROL einen Hinweis]**.
1. Klicken Sie **[!UICONTROL Zur Überprüfung senden]**.

Genehmigende Personen können die Ergebnisse der ChatGPT-Erlebnisse, Marken- und Kanalprüfungen anzeigen und **[!UICONTROL genehmigen]** oder Änderungen anfordern.

Siehe [Anfordern von Überprüfungen und ](/help/user-guide/approvals/request-review.md) und [Überprüfungen und Genehmigungen](/help/user-guide/approvals/overview.md).

### In Inhalt veröffentlichen

Nach allen erforderlichen Genehmigungen veröffentlichen Sie in [!DNL Content]:

1. Klicken Sie **[!UICONTROL In Inhalt veröffentlichen]**.
1. Bestätigen von Metadaten, z. B. Kampagnen- oder Aktivierungsname, Region, Sprache, Persona, funnel-Phase und **Kanal: ChatGPT**.
1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

Die ChatGPT-Anzeige wird in [!DNL Content] angezeigt, kann mit Filtern wie Kanal oder Kampagne gefunden werden und ist in [!DNL Activate] zur Auswahl bereit.

Siehe [Genehmigte Inhalte veröffentlichen](/help/user-guide/approvals/publish-content.md) und [[!DNL Content] Übersicht](/help/user-guide/content/overview.md).

## Aktivieren einer ChatGPT-Anzeige

Die ChatGPT-Aktivierung verwendet dasselbe [[!DNL Activate]](/help/user-guide/activation/overview.md) wie andere gebührenpflichtige Kanäle. Siehe [Aktivieren einer ChatGPT-Anzeige](/help/user-guide/activation/activate-chatgpt-ad.md) für Voraussetzungen und Setup-Felder, die speziell für ChatGPT gelten.
