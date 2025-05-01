---
title: Erstellen einer App Builder-App zur Erweiterung von GenStudio for Performance Marketing
description: Beginnen Sie mit dem Erstellen einer App oder eines Add-ons.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 89b7f477310326755a6b34cb97d5ad5664e98dec
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Entwickeln einer App Builder-App

Entwickelnde, die die nativen Funktionen von GenStudio for Performance Marketing erweitern, verwenden [Adobe App Builder](https://developer.adobe.com/app-builder/), um ihre erweiterbaren Apps oder Add-ons zu erstellen, zu senden und bereitzustellen.

>[!BEGINSHADEBOX]

**Voraussetzungen**:

* Node.js (Version 20.x oder höher)

* npm (im Paket mit Node.js)

* Adobe Developer-Befehlszeilenschnittstelle (CLI). Zur Installation: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Programmstruktur

GenStudio for Performance Marketing-Add-ons sind App Builder-Apps und enthalten dieselben grundlegenden Komponenten wie andere App Builder-Apps.

### Build- und Konfigurationsdateien

Zu den Hauptkomponenten der App Builder-Apps gehören diese Build- und Konfigurationsdateien. Diese Liste enthält nicht alle Build- und Konfigurationsdateien.

* `README.md`: Enthält allgemeine Informationen zur App.

* TS-App-Dateien:

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder-Konfigurationsdateien:

   * `app.config.yaml`
   * `ext.config.yaml`: Konfigurationsdatei für das Add-on
   * `app.config.yaml`: Konfigurationsdatei für das Add-on (einschließlich der Definition Ihrer App als GenStudio for Performance Marketing-Add-on)
   * `.aio`
   * `.env`: Übergeben Sie die `.env` nicht in die Versionsverwaltung

### Quell-Code

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Source-Code-Komponenten

* `ExtensionRegistration.tsx`: Definiert die erforderlichen APIs, die die Host-App (GenStudio for Performance Marketing) zum Laden und Anzeigen des Add-ons benötigt.

* `App.tsx`: Hauptkomponente der App, die das Routing zu anderen Komponenten definiert.

* `AdditionalContextDialog.tsx`: Dialogfeld-Komponente für die Anzeige zusätzlicher Kontext-Add-ons.

* `RightPanel.tsx`: Dialogfeld-Komponente für ein Validierungs-Add-on.

* `Helper`: Enthält `ClaimsChecker`.

## Erstellen einer App Builder-App aus einer bestehenden App

Sie können eine Beispiel-App verwenden, um die Erstellung Ihres Add-ons zu starten.

**So erstellen Sie eine App Builder-App aus einer bestehenden App**:

1. Laden Sie eine Beispielanwendung aus dem Repository [GenStudio UIX-](https://github.com/adobe/genstudio-uix-examples) herunter.

1. Wählen Sie im App Builder-Projekt-Arbeitsbereich auf [Adobe Developer Console](https://developer.adobe.com/console/) die Option **[!UICONTROL Alle herunterladen]** aus, um die Projektdetails herunterzuladen.

1. Öffnen Sie Ihre Beispiel-App lokal in Ihrer bevorzugten integrierten Entwicklungsumgebung (IDE).

1. Authentifizierung über die Adobe Developer-Befehlszeilenschnittstelle:

   ```bash
   aio login
   ```

1. Laden Sie Ihre JSON-Datei herunter und erstellen Sie dann Ihre App:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Hinzufügen von benutzerdefiniertem Code zu Ihrem Add-on

Sie definieren den Add-on-Code in `AdditionalContextDialog.tsx`- und `RightPanel.tsx`. Diese beiden Dateien definieren das Erscheinungsbild und Verhalten von Popups, wenn Benutzer auf das Add-on zugreifen.

* `AdditionalContextDialog.tsx`: Definieren Sie diese Komponente, wenn Sie das Add-on _Kontext hinzufügen_ verwenden möchten. Benutzer interagieren mit dieser Komponente, wenn sie auf _Add-ons_ in der Eingabeaufforderungsschublade in [!DNL Create] klicken.

* `RightPanel.tsx`: Definieren Sie diese Komponente, wenn Sie das Add-on _Bereich rechts_ (Erlebnisvalidierung) verwenden möchten. Benutzer interagieren mit dieser Komponente, wenn sie in einem [!DNL Create] Erlebnisentwurf im rechten Bedienfeld auf das Validierungs-Add-on klicken.

Jetzt können Sie [Ihre App bereitstellen](deploy-app.md)

## Best Practices für die App-Entwicklung

Durch die Wartung Ihrer Entwicklungsumgebung können Sie Fehler bei der App-Entwicklung und -Bereitstellung vermeiden:

* Wenn Sie eine ältere Version einer Beispielanwendung verwenden, aktualisieren Sie die Abhängigkeiten, indem Sie sie erneut installieren:

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Aktualisieren Sie die GenStudio UIX SDK. Vergewissern Sie sich, dass Sie die neueste Version von [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk) verwenden. Unter [Beispiel-Repository für GenStudio UIX](https://github.com/adobe/genstudio-uix-examples) erfahren Sie, wie Sie die neuesten SDK-Änderungen verwenden.
