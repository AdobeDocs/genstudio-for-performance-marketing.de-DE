---
title: Bereitstellen der App Builder-App
description: Stellen Sie Ihre App Builder-App oder Ihr Add-on für GenStudio for Performance Marketing bereit.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Bereitstellen der App

Das Ausführen der App bietet einen vorläufigen Schnappschuss des Verhaltens Ihres Add-ons, bevor Sie es bereitstellen. Diese Informationen können das Debugging erleichtern.

**So führen Sie die App aus**:

Ausführen der App in `https://localhost:9080`:

```bash
aio app run
```

**So stellen Sie die App bereit**:

1. Navigieren Sie zu Ihrem Bereitstellungsarbeitsbereich:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Bereitstellen der App:

   ```bash
   aio app deploy
   ```

**So erzwingen Sie eine erneute Bereitstellung**:

Sie können die Erstellung und Bereitstellung Ihrer App erzwingen, ohne sie erneut zur Genehmigung einzureichen.

>[!NOTE]
>
>Beim Erzwingen eines Builds und einer Bereitstellung wird die vorhandene Bereitstellung überschrieben. **Testen Sie Ihre App** gründlich in einer Testumgebung.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**Gleichzeitiges Erstellen und Bereitstellen**:

```bash
aio app deploy --force-build --force-deploy
```

**So zeigen Sie die App an**:

Nach der Bereitstellung können Sie die App in GenStudio for Performance Marketing anzeigen, indem Sie einen `query` zur GenStudio for Performance Marketing-URL hinzufügen:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

Wenn Sie mit Ihrem Add-on zufrieden sind, können Sie es ohne den `query` verteilen.

Jetzt können Sie [Ihre App verteilen](distribute-app.md).
