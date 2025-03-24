---
title: Bereitstellen der App Builder-App
description: Stellen Sie Ihre App Builder-App oder Ihr Add-on für GenStudio for Performance Marketing bereit.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Bereitstellen der App

Beim Ausführen der App erhalten Sie einen vorläufigen Schnappschuss des Add-on-Verhaltens, bevor Sie sie bereitstellen. Diese Informationen können das Debugging erleichtern. Sie können die Erstellung und Bereitstellung einer in Ihrer App bereitgestellten erzwingen, ohne sie erneut zur Genehmigung einzureichen.


**So führen Sie die App aus**:

Ausführen der App in `https://localhost:9080`:

```bash
aio app run
```

**So stellen Sie die App bereit**:

1. Navigieren Sie zu Ihrem Bereitstellungsarbeitsbereich. So navigieren Sie beispielsweise zum Arbeitsbereich Produktion :

   ```bash
   aio app use -w Production
   ```

1. Bereitstellen der App:

   ```bash
   aio app deploy
   ```

**So erzwingen Sie eine erneute Bereitstellung**:

>[!NOTE]
>
>Durch das Erzwingen der Erstellung und Bereitstellung wird die vorhandene Bereitstellung überschrieben. Testen Sie zuerst Ihre App gründlich in einer Testumgebung.

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

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Wenn Sie mit Ihrem Add-on zufrieden sind, können Sie es ohne den `query` verteilen.

Sie können jetzt [Ihre App verteilen](distribute-app.md).
