---
title: GenStudio Experience Selector-MFE
description: Erfahren Sie, wie Sie den Experience Selector Micro FrontEnd für Ihre GenStudio-Programme und -Add-ons implementieren.
feature: Extensibility, Extensions, Experiences
source-git-commit: 2d6453274d1bfeb35df2821e7e31eec1ca87b013
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# GenStudio Experience Selector-MFE

Experience Selector ist ein Micro Frontend (MFE), das eine `ExperienceSelectorDialog` für die Auswahl von GenStudio-Erlebnissen bietet. Verwenden Sie die -Komponente in Ihrem Programm, indem Sie die `renderExperienceSelectorWithSUSI` aus dem eigenständigen JavaScript-Bundle importieren, das automatisch das neueste bereitgestellte Micro Frontend lädt und eine natürliche Komponentenschnittstelle bietet.

Mit dem GenStudio Experience Selector-MFE können Benutzer:

- GenStudio-Erlebnisse durchsuchen und auswählen
- Filtern von Erlebnissen nach verschiedenen Kriterien
- Unterstützt sowohl einzelne als auch mehrere Auswahlmodi
- Authentifizierung über die SUSI-Integration (Sign-up) durchführen
- Bereitstellung einer konsistenten Benutzeroberfläche über verschiedene Frameworks hinweg

## Integrationsoptionen

Der MFE kann mithilfe von zwei verschiedenen Ansätzen integriert werden:

### ESM (ES-Module) - empfohlen

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Universal Module Definition)

```html
<script src="https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Konfigurationseigenschaften

Die `renderExperienceSelectorWithSUSI`-Funktion akzeptiert ein Konfigurationsobjekt mit den folgenden Eigenschaften:

| Eigenschaft | Typ | Erforderlich | Beschreibung |
|----------|------|----------|-------------|
| `apiKey` | Zeichenfolge | Ja | API-Schlüssel für GenStudio-Services |
| `imsOrg` | Zeichenfolge | Ja | IMS-Organisations-ID |
| `env` | Zeichenfolge | Ja | Umgebung (`stage`, `prod`) |
| `susiConfig` | object | Ja | [SUSI-Authentifizierungskonfiguration](#susi-configuration) |
| `onSelectionConfirmed` | Funktion | Ja | Callback bei Bestätigung der Auswahl |
| `onDismiss` | Funktion | Ja | Rückruf, wenn Dialogfeld geschlossen wird |
| `locale` | Zeichenfolge | Nein | Sprachgebietsschema (z. B. `en-US`) |
| `isOpen` | Boolesch | Nein | Anfänglicher Dialogstatus |
| `selectionType` | Zeichenfolge | Nein | Der Auswahlmodus (`single` oder `multiple`) |
| `customFilters` | Array | Nein | Benutzerdefinierte Filterkriterien |
| `dialogTitle` | Zeichenfolge | Nein | Titel des benutzerdefinierten Dialogs |

### SUSI-Konfiguration

Das `susiConfig` kann Folgendes umfassen:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## Schnellstart

1. **Wählen Sie Ihr Framework** aus den unten stehenden verfügbaren Beispielen
1. **Navigieren Sie zum Beispielverzeichnis**
1. **Installieren von Abhängigkeiten** (für React-/Vue-Beispiele)
1. **Aktualisieren der Konfiguration** mit Ihren API-Schlüsseln und Ihrer IMS-Organisation:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Ausführen des Entwicklungs-Servers**

### Beispielimplementierungen

Dieses Repository enthält Arbeitsbeispiele für verschiedene Frameworks:

- [Eine **vollständige React-Anwendung** die die Integration mit dem Vite-Build-System &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [Eine **Vue 3-Anwendung** mit Kompositions-API-Integration](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Zwei **Vanilla JavaScript-Implementierungen**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

   - [Diese **Vanilla ESM**-Version verwendet ES6-Module und moderne JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

   - [Diese **Vanilla UMD**-Version verwendet das über ein Skript-Tag geladene UMD-Paket](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Authentifizierungsfluss

Der Erlebnisselektor verarbeitet die Authentifizierung automatisch über SUSI:

1. Wenn das Dialogfeld geöffnet wird, wird auf vorhandene Authentifizierung geprüft.
1. Wenn er nicht authentifiziert ist, wird ein SUSI-Anmeldefluss geöffnet.
1. Nach erfolgreicher Authentifizierung wird der Erlebnisselektor angezeigt.
1. Benutzer können Erlebnisse durchsuchen und auswählen.
1. Ausgewählte Erlebnisse werden über den `onSelectionConfirmed`-Callback zurückgegeben.
