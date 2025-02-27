---
title: Textfunktionen
description: Erfahren Sie mehr über die Textfunktion der in GenStudio for Performance Marketing verwendeten Attributkategorien.
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 5cff6d1dd097b18e4fa3d286afddc1db553a415d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# Textfunktionen

Zu den Textfunktionen gehören Zählungen für bestimmte Textelemente wie Wörter, Sätze, Emojis und Klassifizierungen für Semantik, Emotion und Ton, die für die Analyse mit [!DNL Insights] verwendet werden. Text kann auch einen Lesbarkeitswert erhalten.

GenStudio for Performance Marketing verwendet die KI- und maschinellen Lernfunktionen von Adobe, um Text zu studieren und [!UICONTROL Asset-Attribute] basierend auf den zugehörigen Texttönen und Marketing-Erzählungen anzuwenden. Der Prozess validiert den Eingabetext, um sicherzustellen, dass er alphanumerische Zeichen enthält, wobei zusätzliche Leerzeichen und nicht druckbare Zeichen entfernt und der Text auf die maximal zulässigen 1500 Wörter gekürzt wird. Vor dem Anwenden erkannter Attribut-Tags sagt die KI den vorherrschenden Ton voraus.

## Tonfall

Der Ton repräsentiert einen allgemeinen Charakter, eine allgemeine Einstellung oder eine Atmosphäre, die durch Sprache gezeigt wird. Eine einfache Auswahl von Wörtern und Satzzeichen, Satzstruktur und Stil kann den Ton Ihrer Nachricht ändern. Betrachten Sie beispielsweise die folgenden dringenden Nachrichten mit den drei grundlegenden Tonstufen:

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

Die KI erkennt außerdem einen nuancierteren Ton. Unter Verwendung der gleichen dringenden Anweisung aus dem früheren Beispiel verwendet die folgende Version einen skurrilen `poetic`:

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Weitere sekundäre Werte für den Ton sind: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Erzählung

Die erzählerischen Attribute helfen Ihnen, Assets zu identifizieren, die die Werte, den Zweck oder die Identität kommunizieren, die bei Ihrer Zielgruppe Anklang finden.

| Erzählung | Beschreibung | Beispiel |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Lesbarkeitsbewertung

Die Lesbarkeitsbewertung bewertet, wie einfach ein Textstück zu lesen und zu verstehen ist. Dadurch wird sichergestellt, dass Ihre Inhalte für Ihre Zielgruppe geeignet sind. Die Punktzahl hängt von verschiedenen Faktoren ab, einschließlich der Satzlänge und der Wortkomplexität.

| Punktzahl | Schulstufe | Anmerkungen |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00 | 5. Klasse | Sehr leicht zu lesen. Leicht verständlich für einen durchschnittlichen 11-jährigen Schüler. |
| 90,0-80,0 | 6. Klasse | Leicht zu lesen. Konversatives Englisch für Verbraucher. |
| 80,0-70,0 | 7. Klasse | Ziemlich einfach zu lesen. |
| 70,0-60,0 | 8. und 9. Klasse | Einfaches Englisch. Leicht verständlich für 13- bis 15-jährige Studierende. |
| 60,0-50,0 | 10. bis 12. Klasse | Ziemlich schwer zu lesen. |
| 50,0-30,0 | Hochschule | Schwer zu lesen. |
| 30,0-0,0 | Hochschulabsolvent | Sehr schwer zu lesen. Am besten von Universitätsabsolventen verstanden. |

## Wortzählung

TBD

In der folgenden Tabelle sind die Bildfunktionskategorien aufgeführt, die von der GenStudio for Performance Marketing-KI erkannt werden.

| Kategorie | Beschreibung | Beispiel |
| -------------------- | ------------- | --------------------- |
| Emojis-Anzahl |             |        |
| Anzahl der Hash-Tags |             |        |
| Keywords |             |        |
| Marketinggefühle | Emotionen werden in Marketing-Nachrichten gezielt angesprochen, um bestimmte Gefühle und Reaktionen aus dem Publikum hervorzurufen, was die Interaktion und die Verbindung mit der Marke verbessern kann. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Überredungsstrategien | Techniken zur Beeinflussung des Verbraucherverhaltens und zur Förderung erwünschter Aktionen. Diese Strategien zielen auf bestimmte psychologische Trigger und Kundensegmente ab, um die Effektivität von Marketing-Nachrichten zu erhöhen. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Tonfall | Der allgemeine Charakter, die Einstellung oder die Atmosphäre, die in einer Marketing-Botschaft durch Wortwahl, Interpunktion, Satzstruktur und Stil vermittelt wird. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
