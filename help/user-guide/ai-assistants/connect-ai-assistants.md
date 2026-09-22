---
title: Verbinden eines KI-Assistenten
description: Erfahren Sie, wie Sie einen unterstützten KI-Assistenten verbinden, um den Zugriff auf verfügbare Tools zu [!DNL GenStudio for Performance Marketing] und zu überprüfen.
role: User
source-git-commit: 3d22af77d3893233e497a22f7b00c1faf0070cff
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# KI-Assistenten verbinden

Verbinden Sie einen unterstützten KI-Assistenten mit [!DNL GenStudio for Performance Marketing], bevor Sie Leistungsdaten abfragen, Entwürfe zusammenstellen oder genehmigte Anzeigen veröffentlichen. Die Verbindungsoptionen variieren je nach KI-Assistent und Organisation.

## Voraussetzungen

Bevor Sie eine Verbindung herstellen, überprüfen Sie Folgendes:

- Ein gültiges Adobe-Konto mit Zugriff auf [!DNL GenStudio for Performance Marketing].
- Ein unterstützter Plan, der Remote-MCP-Verbindungen ermöglicht, wenn Sie Claude, ChatGPT oder Microsoft Copilot verwenden. Spezifische Anweisungen zum manuellen Konfigurieren von MCP-Verbindungen finden Sie in der Dokumentation zum KI-Assistenten.

## Adobe CX Enterprise Coworker verbinden

[!DNL GenStudio for Performance Marketing] Tools werden in Adobe CX Enterprise Coworker als native Verbindung verwaltet. Ihre Organisation kontrolliert die Verfügbarkeit, sodass Sie nicht die direkte MCP-Server-URL eingeben.

Beginnen Sie eine neue Unterhaltung und [&#x200B; Sie die Verbindung &#x200B;](#verify-the-connection). Wenn die Tools nicht angezeigt werden, wenden Sie sich an den Administrator Ihres Unternehmens oder den Adobe-Support.

## Connect Claude

Claude benötigt einen Pro-, Max-, Team- oder Enterprise-Plan. Derselbe Remote-Connector funktioniert in Claude im Web und in der Desktop-Anwendung.

1. Wählen Sie in Claude **[!UICONTROL Anpassen]** in der linken Seitenleiste aus.
1. Wählen Sie **[!UICONTROL Connectoren]** und klicken Sie auf das Symbol Hinzufügen .
1. Wählen Sie **[!UICONTROL Benutzerdefinierten Connector hinzufügen]** aus.
1. Geben Sie `https://genstudio-services.adobe.io/mcp` als MCP-Server-URL ein.
1. Melden Sie sich mit Ihrer Adobe ID an.
1. Wählen Sie die IMS-Organisation aus, die Zugriff auf [!DNL GenStudio for Performance Marketing] hat.

>[!NOTE]
>
>Bei einem Team- oder Enterprise-Plan muss ein Organisationsverantwortlicher möglicherweise zuerst den Connector hinzufügen. Wenn der Connector bereits verfügbar ist, wählen Sie stattdessen **[!UICONTROL Verbinden]** aus.

## ChatGPT verbinden

ChatGPT erfordert ein Plus-, Pro-, Business-, Enterprise- oder Education-Konto. Benutzerdefinierte MCP-Verbindungen sind im Web über den Entwicklermodus verfügbar.

1. Melden Sie sich bei [ChatGPT](https://chatgpt.com) in einem Webbrowser an.
1. Öffnen Sie **[!UICONTROL Einstellungen]** und aktivieren Sie dann **[!UICONTROL Entwicklermodus]**.
1. Öffnen **[!UICONTROL in]** Einstellungen“ den Bereich für Apps oder Connectoren.
1. Fügen Sie eine benutzerdefinierte MCP-Verbindung namens `GenStudio` hinzu.
1. Geben Sie `https://genstudio-services.adobe.io/mcp` als MCP-Server-URL ein.
1. **[!UICONTROL OAuth]** als Authentifizierungsmethode beibehalten.
1. Melden Sie sich mit Ihrer Adobe ID an.
1. Wählen Sie die IMS-Organisation aus, die Zugriff auf [!DNL GenStudio for Performance Marketing] hat.

>[!NOTE]
>
>ChatGPT kann den Speicherort der Entwickler- und Connector-Einstellungen ändern. Wenn diese Beschriftungen in Ihrem Konto unterschiedlich sind, befolgen Sie die aktuellen OpenAI-Anweisungen zum Hinzufügen eines Remote-MCP-Connectors.

## Codex verbinden

Der Codex erfordert die Codex-Befehlszeilenschnittstelle und ein authentifiziertes Codex-Konto.

1. Offene `~/.codex/config.toml` für alle Projekte oder `.codex/config.toml` für ein Projekt.
1. Fügen Sie diese Konfiguration hinzu:

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. `codex mcp login genstudio` ausführen.
1. Melden Sie sich mit Ihrer Adobe ID im sich öffnenden Browserfenster an.
1. Wählen Sie die IMS-Organisation aus, die Zugriff auf [!DNL GenStudio for Performance Marketing] hat.

## Connect Writer

Writer benötigt Zugriff auf AI Studio.

1. Öffnen Sie in Writer **[!UICONTROL AI Studio]**.
1. Wählen Sie **[!UICONTROL Connectoren und Tools]** aus.
1. Wählen Sie **[!UICONTROL Benutzerdefinierten Connector erstellen]** aus.
1. Wählen Sie **[!UICONTROL Connector-Typ]** MCP-Server) aus.
1. Geben Sie einen Namen und eine Beschreibung für den Connector ein.
1. Geben Sie `https://genstudio-services.adobe.io/mcp` als MCP-Server-URL ein.
1. Festlegen des Team-Zugriffs für den Connector.
1. Wählen **[!UICONTROL OAuth 2.0 (Benutzerebene)]** als Authentifizierungsmethode aus.
1. Melden Sie sich mit Ihrer Adobe ID an.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

[!DNL GenStudio for Performance Marketing] Tools werden in der AI Studio-Tool-Bibliothek angezeigt. Jeder Writer-Benutzer meldet sich mit einer individuellen Adobe ID an.

## Microsoft Copilot verbinden

Microsoft steuert den Einrichtungsfluss für benutzerdefinierte MCP-Verbindungen in Copilot. Befolgen Sie die aktuelle [Microsoft Copilot](https://learn.microsoft.com/en-us/copilot/)-Dokumentation, um einen Remote-MCP-Server hinzuzufügen, und verwenden Sie dann `https://genstudio-services.adobe.io/mcp` als Server-URL.

Wenn Sie dazu aufgefordert werden, melden Sie sich bei Ihrer Adobe ID an und wählen Sie die IMS-Organisation aus, die Zugriff auf [!DNL GenStudio for Performance Marketing] hat.

## Verbindung überprüfen

Überprüfen Sie nach dem Setup, ob die Tools verfügbar sind.

1. Beginnen Sie ein neues Gespräch in Ihrem KI-Assistenten.
1. Fragen Sie den Assistenten, auf welche [!DNL GenStudio for Performance Marketing] er zugreifen kann.
1. Bestätigen Sie, dass die Antwort Tools in Insights, Erstellen und Aktivieren auflistet.
1. Fragen Sie nach einer Leistungszusammenfassung für einen verbundenen Paid-Media-Kanal.

Der Assistent gibt verfügbare Leistungsdaten zurück oder erklärt, warum keine Daten mit der Anfrage übereinstimmen.

>[!TIP]
>
>Wenn die Authentifizierung fehlschlägt, stellen Sie erneut eine Verbindung her und bestätigen Sie, dass Sie die richtige IMS-Organisation ausgewählt haben. Wenn keine Tools angezeigt werden, vergewissern Sie sich, dass Ihr Konto Zugriff auf [!DNL GenStudio for Performance Marketing] hat.

## Verwandte Funktionen

- [Übersicht über KI-Assistenten](overview.md)
- [Verwenden von KI-Assistenten](use-ai-assistants.md)
- [Referenz zu KI-Assistenten-Tools](tools-reference.md)
