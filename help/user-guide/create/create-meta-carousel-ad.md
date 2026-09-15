---
title: Erstellen von Meta-Anzeigen-Erlebnissen - Karussellanzeigen
description: Erfahren Sie, wie Sie in [!DNL GenStudio for Performance Marketing] Multi-Card-Meta-Karussell-Ad-Erlebnisse erstellen, Karten verwalten und Markenkonzepte generieren.
role: User
source-git-commit: 1b407c1c66a2426b21cbbf423774ebdff16a7dec
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 2%
---

# Erstellen eines Meta-Karussell-Anzeigen-Erlebnisses

Eine Meta-Karussellanzeige ist ein Paid-Ad-Format, das zwei bis zehn wischbare Karten mit jeweils einem eigenen Bild oder Video, Überschrift und Link anzeigt.

Auf dieser Seite werden die Schritte beschrieben, die für Karussellanzeigen spezifisch sind. Informationen zu den freigegebenen Schritten, die diese Seite nicht wiederholt, z. B. zum Auswählen einer Vorlage, Hinzufügen von Parametern, Überarbeiten von Varianten und Veröffentlichen, finden Sie unter [Erstellen eines Meta-Anzeigenerlebnisses](/help/user-guide/create/create-meta-ad.md).

## Voraussetzungen

Bevor Sie eine Karussellanzeige erstellen, stellen Sie sicher, dass Sie über eine Vorlage verfügen, deren Seiten ein Seitenverhältnis gemeinsam haben, entweder 1:1 oder 4:5. Jede Vorlagenseite wird zu einer Karte. Weitere Informationen finden Sie unter [Richtlinien für Meta-Anzeigenvorlagen](/help/user-guide/templates/meta-template.md).

## Auswählen des Karussellformats

Nachdem Sie eine Vorlage ausgewählt und die Arbeitsfläche geöffnet haben, wählen Sie in der Eingabeaufforderungsschublade das Karussellformat aus.

1. Erweitern Sie im _[!DNL Create your ads]_&#x200B;Bedienfeld&#x200B;_[!UICONTROL &#x200B; Parameter &#x200B;]_.
1. Wählen Sie im Dropdown **[!UICONTROL Menü]** Format“ die Option **[!UICONTROL Karussellanzeige]**.

   ![Erstellen Sie das Bedienfeld Anzeigen mit dem Dropdown-Menü Format , das auf Karussellanzeige eingestellt ist, und einer Liste von Karten](./carousel-format-cards.png){width="70%" zoomable="yes"}

Wenn Sie mit einer einseitigen Vorlage beginnen, dupliziert [!DNL GenStudio for Performance Marketing] die Seite, um das Zwei-Karten-Minimum zu erreichen. Wenn nicht alle Vorlagenseiten dasselbe Seitenverhältnis aufweisen, wird der Formatwechsel blockiert, bis Sie eine Vorlage mit einem einheitlichen Seitenverhältnis verwenden.

## Verwalten von Karten

Erstellen Sie vor dem Generieren das Kartenset in der Eingabeaufforderungsschublade. Um weitere Karten hinzuzufügen, duplizieren Sie eine vorhandene Karte.

* **Um eine Karte zu duplizieren** wählen Sie **[!UICONTROL Duplizieren]** aus den Kartenoptionen.
* **Um Karten neu anzuordnen** ziehen Sie eine Karte am Griff an eine neue Position.
* **Um eine Karte zu löschen** wählen Sie **[!UICONTROL Löschen]** aus den Kartenoptionen aus. Die letzten beiden Karten können nicht gelöscht werden, da für ein Karussell mindestens zwei Karten erforderlich sind.

Wählen Sie für jede Karte ein Bild aus und legen Sie bei Bedarf ein Produkt pro Karte fest, das das übergeordnete Produkt überschreibt. Sie wählen ein Bild pro Karte einzeln aus. Die Ziel-URLs pro Karte werden später in [!DNL Activate] festgelegt. Weitere Informationen finden Sie unter [Aktivieren einer Meta-Anzeige](/help/user-guide/activation/activate-meta-ad.md).

## Schreiben einer Karussellaufforderung

Ihre Eingabeaufforderung signalisiert die Absicht des Karussells. Beschreiben Sie also, wie die Karten miteinander in Beziehung stehen. Eine Karussellkopie kann einem von zwei Ansätzen folgen:

* **Modular:** Jede Karte ist eine in sich abgeschlossene Anzeige, und es fließt keine Kopie über die Karten hinweg. Verwenden Sie diesen Ansatz für eine Reihe miteinander verbundener, aber unabhängiger Nachrichten, z. B. mehrere Produkte.
* **Sequenziell** Die Kopie verbindet sich über Karten hinweg, um eine Geschichte, eine schrittweise Abfolge oder eine Anleitung zu erzählen. Verwenden Sie diesen Ansatz, wenn die Karten aufeinander aufbauen.

Sie können auch beschreiben, ob das Karussell ein einzelnes Produkt oder mehrere Produkte sowie Details pro Karte enthält.

In dieser Eingabeaufforderung wird beispielsweise ein modulares Karussell mit mehreren Produkten beschrieben:

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

In dieser Eingabeaufforderung wird ein sequenzielles Karussell beschrieben, das eine Geschichte auf fünf Karten erzählt:

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

Informationen zu den Grundlagen der Eingabeaufforderung finden Sie unter [Effektive Eingabeaufforderungen schreiben](/help/user-guide/effective-prompts.md).

## Erstellen und Überprüfen von Konzepten

Nachdem Sie die Karten eingerichtet und die Eingabeaufforderung angezeigt haben, generieren Sie das Karussell und überprüfen Sie die Ergebnisse.

1. Wählen Sie **[!UICONTROL Generieren]**.

   [!DNL GenStudio for Performance Marketing] generiert vier Karussellkonzepte. Jedes Konzept ist ein komplettes Multi-Card-Karussell mit eigener Markenbewertung.

   ![Vier generierte Karussellkonzepte mit jeweils einer Markenbewertung und einer Schaltfläche Bearbeiten](./carousel-concepts.png){width="80%" zoomable="yes"}

1. Wählen Sie ein Konzept aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**, um es zur Bearbeitung zu öffnen.
1. Verwenden Sie die Pfeile, um zwischen den Karten zu wechseln, und bearbeiten Sie dann den Text oder wählen Sie **[!UICONTROL Austauschen]** aus, um das Bild einer Karte zu ändern. Weitere Informationen zum Bearbeiten finden Sie unter [Verwalten von Varianten](/help/user-guide/create/manage-variants.md).

Wenn Sie Karten vor dem Generieren neu anordnen, wird die Arbeitsfläche sofort aktualisiert. Wenn Sie die Karten nach dem Generieren in der Eingabeaufforderungsschublade neu anordnen, wird die Änderung erst angewendet, nachdem Sie erneut generiert haben, und eine Regenerierungswarnung wird angezeigt.

## Grundlegendes zu Feldern pro Karte und gemeinsam genutzter Felder

Einige Karussellfelder gelten für jede Karte einzeln und andere für die gesamte Anzeige. In der folgenden Tabelle wird beschrieben, wie sich die einzelnen Felder bei Meta-Karussellanzeigen verhalten.

| Feld | Umfang |
|---|---|
| Überschrift | Pro Karte |
| Beschreibung | Pro Karte, optional, in [!DNL Activate] festgelegt |
| Call to action | Geteilt in der Anzeige |
| Primärer Text | Geteilt in der Anzeige |
| Medien | Pro Karte (Bild, Video oder gemischt) |
| Text auf dem Bild | Pro Karte |
| Ziel-URL | Pro Karte, festgelegt in [!DNL Activate] |

## Veröffentlichen, Exportieren und Aktivieren

Wenn das Karussell fertig ist, veröffentlichen und exportieren Sie es auf die gleiche Weise wie andere Meta-Anzeigen. Ein Karussell wird als einzelnes Erlebnis gespeichert, das einem Konzept entspricht. Der Export liefert eine CSV-Datei sowie die Kartenmedien. Siehe [[!DNL Content]](/help/user-guide/content/overview.md) zur Speicherung veröffentlichter Erlebnisse. Informationen zum Aktivieren Ihres Karussells für Meta finden Sie unter [Aktivieren einer Meta-Anzeige](/help/user-guide/activation/activate-meta-ad.md).
