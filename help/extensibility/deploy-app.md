---
title: Bereitstellen der App Builder-App
description: Stellen Sie Ihre App Builder-App oder Ihr Add-on für GenStudio for Performance Marketing bereit.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
TQID: https://experienceleague.adobe.com/7Z4Fb-jPi4FHrTeOgHxxO4fl982sqri-7uEDoylFF-s
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: ad3738c7-91ac-48ed-a914-fd0b03f89396id: bfaa655b-e017-428d-80d0-09de2183b296id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: da3860b0-d637-47df-bef0-273751180266
source-git-commit: ca8bfb11a301697c92e97bad41ea3ba8aa359847
workflow-type: tm+mt
source-wordcount: 622
ht-degree: 0%

---

# Bereitstellen der App

Das Ausführen der App bietet einen vorläufigen Schnappschuss des Verhaltens Ihres Add-ons, bevor Sie es bereitstellen. Dies kann beim Debugging helfen.

## Ausführen der App

Ausführen der App in `https://localhost:9080`:

```bash
aio app run
```

## Bereitstellen der App

1. Navigieren Sie zu Ihrem Bereitstellungsarbeitsbereich:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Bereitstellen der App:

   ```bash
   aio app deploy
   ```

## Erzwungene Neuverlegung

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

## Gleichzeitiges Erstellen und Bereitstellen

```bash
aio app deploy --force-build --force-deploy
```

## Neue App suchen

Nach der Bereitstellung können Sie die neue App in GenStudio for Performance Marketing anzeigen.

### Mit URL anzeigen

Sehen Sie sich die neue App an, indem Sie der GenStudio for Performance Marketing-URL einen `query` hinzufügen:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### In der Benutzeroberfläche anzeigen

Je nach dem Typ der bereitgestellten Erweiterung befinden sich neue Erweiterungen an verschiedenen Stellen in der Benutzeroberfläche. Die derzeit verfügbaren Erweiterungspunkte sind:

* Compliance-Erweiterung, die Folgendes umfasst:
   * [*Prompt-Erweiterungspunkte*](#find-prompt-extensions) mit denen Kunden zusätzlichen Kontext zur LLM-Generierung hinzufügen können, und
   * [*Validierungs-Erweiterungspunkte*](#find-validation-extensions) mit denen Kunden den generierten Inhalt aus dem LLM überprüfen können. Die Validierung wird häufig mit einer sofortigen Erweiterung gepaart, um sicherzustellen, dass der mit einer verlängerten Eingabeaufforderung generierte Inhalt den Kundenanforderungen entspricht (z. B. Ansprüche auf medizinische Medikamente oder rechtliche Vorschriften)
* [Erweiterung für Digital Asset Management (DAM)](#find-dam-extensions)
* [Vorlagenerweiterung](#find-template-extensions)
* [Übersetzungs-Erweiterung](#find-translation-extensions)
* [Inhaltsfragment-Erweiterung](#find-content-fragment-extension)

### Prompt-Erweiterungen suchen

Eingabeaufforderungserweiterungen finden Sie im Dropdown **Menü „Add** ons“ im **Parameter** einer Vorlage.

![Prompt-Erweiterungen](./select-prompt-ext.png){width="600" zoomable="yes"}

Das Add-On-Dialogfeld wird geöffnet. Darin können Sie den zusätzlichen Kontext auswählen, der für die LLM-Generierung hinzugefügt werden soll.

![Dropdown-Liste „Eingabeaufforderungserweiterung“](./select-prompt-dropdown.png){width="600" zoomable="yes"}

### Validierungserweiterungen suchen

Validierungs-Erweiterungen finden Sie nach einer Eingabeaufforderungsgenerierung in der rechten Leiste, die mit den Ergebnissen angezeigt wird.

![Validierungserweiterungen](./validation-ext.png){width="600" zoomable="yes"}

Führen Sie die ausgewählte Erweiterung aus, um den generierten Inhalt zu validieren.

![Gültige Validierung](./validation-valid.png){width="600" zoomable="yes"}

Wenn Fehler auftreten, können Sie die Erweiterung verwenden, um die Kopie der Erlebnisse programmgesteuert zu aktualisieren. Durch Klicken auf **[!UICONTROL Kopieren]** wird der vorgeschlagene Text in die Zwischenablage kopiert. Durch Klicken auf **[!UICONTROL Anwenden]**-Schaltfläche wird der Text auf ein bestimmtes Textfeld im generierten Erlebnis angewendet.

![Ein Validierungsfehler, der die Schaltflächen Kopieren und Anwenden anzeigt](./validation-copy-apply.png){width="600" zoomable="yes"}

### DAM-Erweiterungen suchen

DAM-Erweiterungen (Digital Asset Management) werden gefunden, wenn Sie im Abschnitt **Parameter** einer Vorlage Inhalte auswählen. Unten im Dropdown-Menü **Speicherort auswählen** finden Sie Add-ons.

![DAM-Erweiterungen](./dam-ext.png){width="600" zoomable="yes"}

### Vorlagenerweiterungen suchen

Vorlagenerweiterungen finden Sie auf der Registerkarte **Externe Vorlagenanwendung** bei der Auswahl einer Vorlage. Diese Registerkarte wird nur angezeigt, wenn Vorlagen-Apps ausgewählt werden können.

![Vorlagenerweiterungen](./template-ext.png){width="600" zoomable="yes"}

### Suchen von Übersetzungserweiterungen

Verwenden Sie Übersetzungs-Erweiterungspunkte , um Ihren eigenen Übersetzungs-Service über einen Proxy zu übertragen, anstatt die standardmäßige GenStudio-Übersetzung zu verwenden.
Für diese Erweiterungen gibt es keinen Speicherort auf der Benutzeroberfläche.

Wenn die Erweiterung registriert ist, wird der bereitgestellte Übersetzungs-Service verwendet. Andernfalls wird der standardmäßige GenStudio-Übersetzungs-Service verwendet.

### Inhaltsfragmenterweiterung suchen

Die Inhaltsfragment-Erweiterung in [!DNL GenStudio for Performance Marketing] ersetzt Text in generierten E-Mail-Erlebnissen auf der [!DNL Create]-Arbeitsfläche durch Einträge aus einem verbundenen Drittanbieter-Repository (3P). Nachdem Sie die Erweiterung konfiguriert und bereitgestellt haben, tauschen Sie die Kopie aus der Arbeitsfläche aus, ohne den Workflow verlassen zu müssen.

>[!NOTE]
>
>Der Austausch von Inhaltsfragmenterweiterungen ist heute für E **Mail**-Erlebnisse auf der Arbeitsfläche verfügbar. **Horizon**-Channel-Support ist in Kürze verfügbar.

**So tauschen Sie Text mithilfe der Inhaltsfragment-Erweiterung aus**:

1. Klicken Sie auf der Arbeitsfläche in einer generierten E-Mail-Variante auf ein bearbeitbares Textfeld.
1. Klicken Sie **[!UICONTROL Wechseln]**.
   ![Text austauschen](./subject-line-swap.png){width="400" zoomable="yes"}
1. Wählen Sie das Repository eines Drittanbieters aus. Ihr Unternehmen steuert, welche Repositorys angezeigt werden und wie sich die Repository-Benutzeroberfläche verhält.
1. Wählen Sie den Anspruch aus, den Sie als Ersatztext für das Feld verwenden möchten.

Wenn Sie mit Ihrem Add-on zufrieden sind, können Sie es ohne den `query` verteilen.

Jetzt können Sie [Ihre App verteilen](distribute-app.md).
