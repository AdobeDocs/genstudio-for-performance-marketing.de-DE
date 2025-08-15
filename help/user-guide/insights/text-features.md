---
title: Textfunktionen
description: Erfahren Sie mehr über die Textfunktion der in GenStudio for Performance Marketing verwendeten Attributkategorien.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 3ccc6313a7c559f1c0846c144d23b783da0aecfa
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 1%

---

# Textfunktionen

Zu den Textfunktionen gehören Zählungen für bestimmte Textelemente wie Wörter, Sätze, Emojis und Klassifizierungen für Semantik, Emotion und Ton, die für die Analyse mit [!DNL Insights] verwendet werden. Text kann auch einen Lesbarkeitswert erhalten.

GenStudio for Performance Marketing verwendet die KI- und maschinellen Lernfunktionen von Adobe, um Text zu studieren und [!UICONTROL Medienattribute] basierend auf den zugehörigen Texttönen und Marketing-Erzählungen anzuwenden. Der Prozess validiert den Eingabetext, um sicherzustellen, dass er alphanumerische Zeichen enthält, wobei zusätzliche Leerzeichen und nicht druckbare Zeichen entfernt und der Text auf die maximal zulässigen 1500 Wörter gekürzt wird. Vor dem Anwenden erkannter Attribut-Tags sagt die KI den vorherrschenden Ton voraus.

## Tonfall

Der Ton repräsentiert einen allgemeinen Charakter, eine allgemeine Einstellung oder eine Atmosphäre, die durch Sprache gezeigt wird. Eine einfache Auswahl von Wörtern und Satzzeichen, Satzstruktur und Stil kann den Ton Ihrer Nachricht ändern. Betrachten Sie beispielsweise die folgenden dringenden Nachrichten mit den drei grundlegenden Tonstufen:

| Ton | Beschreibung | Beispiel |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Förmlich | Gepflegte und professionelle Sprache. | `Take advantage of this distinctive and exceptional opportunity!` |
| mitteilsam | Freundliche und informelle Sprache. | `Don't miss out on this great opportunity!` |
| Direkt | Einfach und auf den Punkt. | `Don't miss the chance!` |

Andere Nebenwerte für den Ton bieten eine genauere Unterscheidung des Charakters und der Haltung Ihrer Nachricht. Im Einklang mit dem früheren Beispiel einer dringenden Nachricht könnte die GenAI einen _poetischen)_ in diesem skurrilen Beispiel entdecken: `Embrace the moment, without delay, for this occasion won't always stay.`

In der folgenden Tabelle sind die von der GenStudio for Performance Marketing-KI erkannten Tonwerte aufgeführt.

| Ton | Beschreibung | Beispiel |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| selbstbewusst | Selbstbewusst und kraftvoll in der Ausdrucksweise. | `You need to act now to secure this deal!` |
| Direkt | Einfach und auf den Punkt. | `Don't miss the chance!` |
| einfühlsam | Verständnis und Sensibilität zeigen. | `We understand your needs, and this is perfect for you.` |
| begeistert | Zeigen Sie intensives und eifriges Vergnügen, Interesse oder Zustimmung. | `This is an amazing opportunity you can't miss!` |
| humorvoll/witzig | Unbeschwert und klug. | `Why wait? Grab this deal before it's gone!` |
| inspirierend | Ermutigend und erhebend. | `Believe in yourself and seize this opportunity!` |
| poetisch | Künstlerisch und expressiv. | `Embrace the dawn of a new opportunity.` |
| quantitativ | Basierend auf numerischen Daten. | `99% of users loved this offer, and you will too.` |
| sensorisch | Die Sinne einbeziehen. | `Feel the excitement with this incredible offer!` |
| Storytelling | Erzählen einer Geschichte, um eine Botschaft zu vermitteln. | `Once upon a time, there was an offer you couldn't refuse.` |

## emotionale Anziehungskraft

Marketing-Experten nutzen die Macht menschlicher Emotionen, um eine starke Verbindung zwischen dem Publikum und der Marke zu schaffen. Indem sie sich Sinneswahrnehmungen wie Glück, Angst, Aufregung oder Nostalgie zunutze machen, können Marketing-Fachleute Botschaften verfassen, die auf einer tieferen Ebene Resonanz finden, die die Interaktion fördern und das Verbraucherverhalten beeinflussen. Emotionale Anziehungskraft trägt dazu bei, zusammenhängende und einprägsame Inhalte bereitzustellen, was letztendlich die Markentreue fördert und gewünschte Aktionen fördert.

Überzeugungstaktiken, Marketing-Emotionen und Erzählstile arbeiten zusammen, um Kundensegmente anzusprechen.

- **Erzählstile** wie Authentizität, Feiern und Community, helfen dabei, die Werte und Identitäten zu vermitteln, die bei der Zielgruppe Anklang finden, und schaffen so eine überzeugendere und nachvollziehbare Botschaft.
- **Überzeugungstaktiken** wie Knappheit, sozialer Beweis und Gegenseitigkeit, sind so konzipiert, dass sie das Verbraucherverhalten beeinflussen, indem sie an ihre Emotionen und Vorlieben appellieren.
- **Marketing-Emotionen** zielen darauf ab, Gefühle zu stimulieren, die die Interaktion und Verbindung mit der Marke verbessern.

GenStudio for Performance Marketing AI erkennt und unterscheidet diese Merkmale, indem es den Text auf emotionale Hinweise, den Ton und den Erzählstil analysiert. Die KI nutzt Algorithmen der natürlichen Sprachverarbeitung (NLP) und des maschinellen Lernens, um Muster zu identifizieren und den Text anhand vordefinierter emotionaler und überzeugender Attribute zu klassifizieren.

### Erzählstil

Die Attribute der Erzählung oder des Appellationsfaktors helfen, Medien zu identifizieren, die die Werte, den Zweck oder die Identität kommunizieren, die bei Ihrer Zielgruppe Anklang finden. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing-KI erkannten Erzählungsstile aufgeführt.

| Berufungsfaktor | Beschreibung | Beispiel |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Authentizität | Echt und real, wobei oft Transparenz und Ehrlichkeit hervorgehoben werden. | `A behind-the-scenes look at how our products are made.` |
| Feier | Mit Freude und Feierlichkeit besondere Anlässe oder Errungenschaften markieren. | `Join us in celebrating our 10th anniversary with special offers!` |
| Community | Förderung des Zugehörigkeits- und Zusammengehörigkeitsgefühls innerhalb einer Gruppe. | `Our brand is built on the strength of our community.` |
| Komfort | Betonung der Benutzerfreundlichkeit und der zeitsparenden Vorteile. | `Get what you need with just one click.` |
| Befähigung | Individuen ermutigen und befähigen, Kontrolle zu übernehmen und Entscheidungen zu treffen. | `Empower yourself with our latest tools and resources.` |
| Exploration | Einladende Entdeckungen und Abenteuer, oft verbunden mit neuen Erlebnissen. | `Discover new horizons with our travel packages.` |
| futuristisch | Hervorhebung von Innovation und zukunftsorientierten Ideen. | `Experience the future of technology today.` |
| Übertreibung | Generieren von Spannung und Vorfreude rund um ein Produkt oder Ereignis. | `Don't miss out on the most anticipated event of the year!` |
| Nachgiebigkeit | Appell an Fantasien, Wünsche oder Vergnügen. | `Treat yourself to the finest gourmet chocolates.` |
| Ein sicheres Gefühl | Für Beruhigung und ein Gefühl der Sicherheit. | `Rest easy knowing your data is safe with us.` |
| Personalisierung | Erlebnisse oder Produkte auf individuelle Vorlieben zuschneiden. | `Get a custom-fit solution just for you.` |
| Prestige | Verbindung mit hohem Status und Exklusivität. | `Join the elite with our premium membership.` |
| Zeitlosigkeit | Die Betonung auf dauerhafte Qualität und klassische Anziehungskraft. | `Our designs are timeless and never go out of style.` |
| Vielseitigkeit | Hervorhebung der Anpassungsfähigkeit und der vielfältigen Verwendungsmöglichkeiten. | `Our product fits seamlessly into any lifestyle.` |
| Wohlbefinden | Gesundheit, Glück und allgemeines Wohlbefinden fördern. | `Enhance your well-being with our holistic approach.` |

### Überzeugungstaktik

Überzeugungstechniken werden verwendet, um das Verbraucherverhalten zu beeinflussen und gewünschte Aktionen zu fördern. Diese Strategien zielen auf bestimmte psychologische Trigger und Kundensegmente ab, um die Effektivität von Marketing-Nachrichten zu erhöhen. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing-KI erkannten Überzeugungstaktiken aufgeführt.

| Taktik | Beschreibung | Beispiel |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Anthropomorphismus | Zuordnung menschlicher Eigenschaften zu Produkten oder Marken. | `Our friendly chatbot is here to help you.` |
| Vergleich | Hervorheben von Unterschieden zwischen Optionen zur Beeinflussung der Auswahl. | `See how we compare to the competition.` |
| Konkretheit | Bereitstellung spezifischer Details, um die Botschaft greifbarer zu machen. | `Save 20% on your next purchase.` |
| Empfehlung | Mit Genehmigung von glaubwürdigen Quellen oder Influencern. | `Recommended by top industry experts.` |
| Fuß in der Tür | Beginnend mit einer kleinen Anfrage, um die Wahrscheinlichkeit der Zustimmung zu einer größeren Anfrage zu erhöhen. | `Try our free trial today.` |
| Überwindung der Reaktanz | Reduzierung des Widerstands durch Anerkennung und Behandlung von Einwänden. | `We understand your concerns, and here's how we address them.` |
| Reziprozität | Etwas Wertvolles anbieten, um eine Rückgabe zu fördern. | `Get a free gift with your purchase.` |
| Knappheit | Dringlichkeit schaffen, indem die begrenzte Verfügbarkeit hervorgehoben wird. | `Only a few items left in stock!` |
| Soziale Identität | Nutzung des Gefühls der Zugehörigkeit des Verbrauchers zu einer Gruppe. | `Join our community of innovators.` |
| Soziale Auswirkungen | Hervorhebung der positiven Auswirkungen auf Gesellschaft oder Umwelt. | `Your purchase helps plant a tree.` |
| Social-Korrekturabzug | Verwenden von Empfehlungen oder benutzergenerierten Inhalten zum Aufbau von Vertrauen. | `See why thousands of users love our product.` |

### Marketingemotionen

Emotionen werden in Marketing-Nachrichten gezielt angesprochen, um bestimmte Gefühle und Reaktionen aus dem Publikum hervorzurufen, was die Interaktion und die Verbindung mit der Marke verbessern kann. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing-KI erkannten Emotionen aufgeführt.

| Gefühl | Beschreibung | Beispiel |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Streben | Inspirieren eines Wunsches, etwas Größeres zu erreichen. | `Imagine the possibilities with our premium service.` |
| Herausforderung | Die Zielgruppe wird ermutigt, ein Hindernis zu überwinden oder eine neue Aufgabe anzunehmen. | `Are you ready to take the next step in your career?` |
| Kuriosität | Interesse wecken und Lust haben, mehr zu erfahren. | `Discover the secrets behind our success.` |
| Exklusivität | Das Gefühl erzeugen, Teil einer ausgewählten Gruppe zu sein. | `Join our exclusive club for members-only benefits.` |
| Faszination | Fesselnde Zuschauer mit spannenden Inhalten. | `Be amazed by our latest innovations.` |
| Befriedigung | Bereitstellung von Zufriedenheit und Freude bei der Verwendung des Produkts oder der Dienstleistung. | `Enjoy the ultimate comfort with our luxury bedding.` |
| Erkennung | Anerkennung und Bewertung der Leistungen oder des Status der Zielgruppe. | `Get the recognition you deserve with our award-winning service.` |
| Vertrauen | Aufbau von Vertrauen und Zuverlässigkeit in der Marke. | `Trust us to deliver quality and excellence every time.` |
| Dringlichkeit | Sofortiges Handeln durch Hervorhebung zeitkritischer Möglichkeiten. | `Act now before this limited-time offer expires!` |

## Lesbarkeitsbewertung

Die Lesbarkeitsbewertung bewertet, wie einfach ein Textstück zu lesen und zu verstehen ist. Dadurch wird sichergestellt, dass Ihre Inhalte für Ihre Zielgruppe geeignet sind. Die Punktzahl hängt von verschiedenen Faktoren ab, einschließlich der Satzlänge und der Wortkomplexität. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing-KI erkannten Lesbarkeitsstufen aufgeführt.

| Lesbarkeitsstufe | Beschreibung | Beispiel |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| &#x200B;5. Klasse | Sehr einfache Sprache, geeignet für kleine Kinder. | `The cat sat on the mat.` |
| &#x200B;6. Klasse | Einfache und klare Sprache, geeignet für ein allgemeines Publikum. | `You can find great deals on our website.` |
| &#x200B;7. Klasse | Einfach zu verstehen, mit einfachem Vokabular und Struktur. | `Our new product is simple to use and very effective.` |
| &#x200B;8. und 9. Klasse | Klare und knappe Sprache, geeignet für Jugendliche. | `This guide will help you understand the basics of our service.` |
| &#x200B;10. bis 12. Klasse | Komplexere Sprache, geeignet für ältere Jugendliche und Erwachsene. | `The comprehensive manual provides detailed instructions for setup.` |
| Hochschule | Fortgeschrittene Sprache, geeignet für ein gut ausgebildetes Publikum. | `The study explores the multifaceted implications of the new policy.` |
| Hochschulabsolvent | Hoch entwickelte Sprache, geeignet für Experten und Spezialisten. | `The dissertation delves into the intricacies of quantum mechanics.` |

## Zählungen

Das Verständnis und die Nutzung von Zählattributen wie Hashtag-Zahlen, Wortzahlen, Satzzählungen und Stoppwörter-Verhältnissen können Ihre Inhaltsstrategie erheblich verbessern. Diese Metriken bieten wertvolle Einblicke in die Effektivität und Reichweite Ihrer Marketing-Maßnahmen. In der folgenden Tabelle sind die von der GenStudio for Performance Marketing-KI erkannten Zählkategorien aufgeführt.

| Kategorie | Beschreibung | Beispiel |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Emojis-Anzahl | Die Anzahl der im Text vorhandenen Emojis. Emojis können die Interaktion verbessern und Emotionen schnell vermitteln. | `😊`, `🚀`, `❤️` |
| Anzahl der Hash-Tags | Die Anzahl der im Text verwendeten Hashtags. Hashtags helfen, Inhalte zu kategorisieren und die Auffindbarkeit in Social Media zu verbessern. | `#Marketing`, `#Sale` |
| Wortzahl pro Satz | Die durchschnittliche Anzahl von Wörtern pro Satz im Text. Kürzere Sätze sind oft leichter zu lesen und zu verstehen. | `10` |
| Wortzahl | Die Gesamtzahl der Wörter im Text. Eine höhere Wortzahl kann detailliertere Informationen liefern, kann aber auch mehr Aufwand zum Lesen erfordern. | `1500 words` |
| Stoppwörter-Verhältnis | Das Verhältnis von Stoppwörtern zu sinnvollen Wörtern im Text. Stoppwörter (wie „a“ „an“ „the„) werden in Suchabfragen und -ergebnissen häufig ignoriert. Ein hoher Anteil an Stoppwörtern kann Inhalte weniger ansprechend und schwieriger zu lesen machen. | `0.375` |
| Anzahl der Sätze | Die Gesamtzahl der Sätze im Text. Mehr Sätze können detailliertere Inhalte anzeigen, aber zu lange Texte können das Interesse des Lesers verlieren. | `75 sentences` |
