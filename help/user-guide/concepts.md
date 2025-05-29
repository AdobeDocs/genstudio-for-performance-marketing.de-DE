---
title: Adobe GenStudio for Performance Marketing-Konzepte
description: Erfahren Sie mehr über Adobe GenStudio for Performance Marketing-Konzepte und -Terminologie.
feature: Generative AI
role: User
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
source-git-commit: 1ff6a3ecf0a0773c3a6f13d6993042b0620c6dd2
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 0%

---

# Konzepte

GenStudio for Performance Marketing ist ein eigenständiges Unternehmensprodukt, das die Inhaltslieferkette von Adobe enthält, um Marketing-Kampagnen zu optimieren. Es ist eine Herausforderung, personalisierte, von der Marke genehmigte Inhalte in großem Maßstab zu erstellen, die Effektivität zu überwachen und sich schnell an den sich ständig verändernden Markt anzupassen. GenStudio for Performance Marketing führt Creative Cloud und Experience Cloud in einer Anwendung zusammen, die generative KI als Leistungsmultiplikator für Marketing-Teams in Unternehmen nutzt.

Mit GenStudio for Performance Marketing können Sie:

* Erstellen Sie markeninterne Inhalte mit natürlichen Sprachaufforderungen für Ihre digitalen Kanäle der obersten Priorität, wie bezahlte Medien, E-Mail und Display-Anzeigen

* Zusammenarbeit mit Stakeholdern zur Überprüfung und Genehmigung generierter Inhalte
* Generierte und genehmigte Inhalte für den Zugriff auf zukünftige Marketing-Kampagnen speichern
* Bewertung der Content-Effektivität durch Analyse der Asset-Performance und Identifizierung der wichtigsten Attribute leistungsstarker Inhalte

## Generative KI-Technologie

GenStudio for Performance Marketing nutzt die Leistungsfähigkeit generativer KI, um den Prozess der Inhaltserstellung zu beschleunigen und eine hochwertige Inhaltserstellung sicherzustellen. Der iterative Lebenszyklus Ihrer Kreativ-Assets führt zu immer genaueren und markenorientierten Inhalten, die bei Ihrer Zielgruppe Anklang finden.

Beginnen Sie mit der Aufnahme des Brandings, der Kundenrollen und Produktbeschreibungen Ihres Unternehmens durch die leistungsstarke Funktion „Markenrichtlinien“. Informationen zum Vorbereiten und Hochladen [ Richtlinien finden ](../user-guide/guidelines/overview.md) unter „Richtlinien - Übersicht“.

{{in-academy}}

### Große Sprachmodelle

GenStudio for Performance Marketing nutzt Adobes generative KI-Plattform, die grundlegende KI- und maschinelle Lerndienste (ML) bietet. Diese Plattform vereinfacht die Verwendung umfangreicher Sprachmodelle (LLMs) und ermöglicht mit den GenAI-Funktionen von Adobe die Erstellung ansprechender Erlebnisse.

GenStudio for Performance Marketing verwendet die GPT-Serie von Drittanbieter-LLMs über Azure OpenAI.<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

_[!DNL Generative Actions]_sind, wie in der [Adobe GenStudio for Performance Marketing-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) definiert, die Einheiten, die die Verwendung von generativen KI-Funktionen in GenStudio for Performance Marketing quantifizieren.

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not -->

### Tarife

Sie erhalten eine Standardzuteilung von [!DNL Generative Actions], wie in der [GenStudio for Performance Marketing-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) beschrieben.

>[!NOTE]
>
>Die Nutzungsraten können variieren. Pläne können sich ändern. Aktualisierte Informationen zum Tarif finden Sie in ](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) [Adobe GenStudio for Performance Marketing-Produktbeschreibung.

Die folgenden Funktionen verbrauchen [!DNL Generative Actions] mit der angegebenen Rate.

| Funktion | Rate generativer Aktionen |
| -----------------------  | ------------------ |
| E-Mail erstellen | 5 pro Generation |
| Erstellen von Paid Media-Anzeigen | 5 pro Generation |
| Erstellen von Display-Anzeigen | 5 pro Generation |
| Abschnitte regenerieren | 1 pro Generation |

<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

[!DNL Generative Actions] _werden nicht_, wenn:

* Verwendung [Markenvalidierung](/help/user-guide/guidelines/brand-validation.md) während der Variantengenerierung
* Extrahieren von Informationen aus [hochgeladenen Richtlinien](/help/user-guide/guidelines/add-guidelines.md)
* Manuelles [ von Varianten](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* Digitale Assets werden automatisch mit Attributen versehen ([[!DNL Insights]](/help/user-guide/insights/overview.md))

>[!TIP]
>
>Wenn Sie Ihre [!DNL Generative Actions] überschreiten, können Sie direkt bei Ihrem Kundenbetreuer einkaufen.

## Data Governance

Bei der Arbeit mit KI zum Generieren von Inhalten ist es wichtig sicherzustellen, dass die Ausgabe sicher und für alle Benutzer inklusiv ist. Dies erfordert die Auswertung der Inhalte auf potenziell schädliche Vorurteile, Hassreden, beleidigendes Material oder Obszönitäten. Adobe testet die Inhaltserstellungstechnologie aus verschiedenen Perspektiven gründlich, führt umfassende Ethikprüfungen durch und implementiert wirksame Minderungspläne, um zu verhindern, dass schädliche Inhalte in die Ergebnisse gelangen.

Dieser Ansatz stärkt die soziale Verantwortung, minimiert das Reputationsrisiko und stellt die Einhaltung der Richtlinien für Vertrauen und Sicherheit sowie Ethik von [Adobe ](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf).

GenStudio for Performance Marketing umfasst Minderungspläne, um die Verwendung identifizierter schädlicher oder verzerrter Inhalte gemäß den Data Governance-Standards und -Richtlinien von Adobe zu verhindern. Wenn solche Inhalte erkannt werden, werden Sie darauf hingewiesen, dass die Asset-Generierung mit der Meldung „Kann nicht generiert werden“ blockiert wird.

Wenn diese Nachricht angezeigt wird, können Sie die Eingabeaufforderung bearbeiten und erneut versuchen _den Inhalt der Eingabeaufforderung zur Überprüfung durch GenStudio for Performance Marketing kennzeichnen_ oder markieren). Die Prompt-Daten für Inhalte, die zur Überprüfung gekennzeichnet sind, werden zu internen Überprüfungszwecken erfasst.

## Inhaltslebenszyklus

Die Nachfrage nach qualitativ hochwertigen Erlebnissen ist auf mehreren Kanälen schneller. GenStudio for Performance Marketing vereinfacht die Bereitstellung von Inhalten in einem gut organisierten Workflow für Marketing-Fachleute. GenStudio for Performance Marketing nutzt Adobe-Technologie in jeder Phase des Lebenszyklus.

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>Workflow und Planung</strong></p>

    </td>

    <td>

        <p>Ideen austauschen, Richtlinien definieren und eine Strategie rund um Inhalte entwickeln, um Ihre Zielgruppe anzusprechen.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Erstellung und Produktion</strong></p>

    </td>

    <td>

        <p>Erstellen Sie den Inhalt basierend auf dem Plan. Zusammenarbeit in Echtzeit, Empfang von Feedback, Bearbeitung und Genehmigung von Inhalten.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Content-Management</strong></p>

    </td>

    <td>

        <p>Speichern, Freigeben und Suchen von Kreativ-Assets im zentralen Repository. Wiederverwenden und Revitalisieren von Inhalten basierend auf Leistung.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Versand und Aktivierung</strong></p>

    </td>

    <td>

        <p>Aktivieren von Inhalten und Veröffentlichen über mehrere Marketing-Kanäle hinweg.</P>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Reporting und Insights</strong></p>

    </td>

    <td>

        <p>Erfassen Sie Daten und leiten Sie Erkenntnisse zur Asset-Leistungsoptimierung ab.</p>

    </td>

</tr>

</table>
