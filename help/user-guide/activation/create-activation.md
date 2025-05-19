---
title: Aktivierungs-Workflow
description: Erfahren Sie mehr über den Aktivierungs-Workflow für Werbeanzeigen.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 46453d7cf1901312001aa3b304be9d0832a46079
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Aktivierungs-Workflow

_[!DNL Activate]_&#x200B;unterstützt die Aktivierung von Anzeigenerlebnissen in kanalspezifischen Formaten, wie z. B. einem Meta- oder Google Campaign Manager 360-Anzeigenerlebnis.

Ein GenStudio for Performance Marketing-Erlebnis ist eine Marketing-Kampagnenkomponente (z. B. eine Anzeige), die als Anzeigenerlebnis für eine bestimmte Zielgruppe in einem gebührenpflichtigen Anzeigenkanal oder einer gebührenpflichtigen E-Mail vorbereitet wird. Die zu aktivierenden Erlebnisse umfassen drei Hauptkomponenten:

* **Medien-Assets**: Medien-Assets sind die Bilder (GIFs, PNG, JPEG), die in Ihrem Anzeigenerlebnis enthalten sind. Die Aktivierung unterstützt derzeit statische Bilder.

  Für die Auswahl eines Bild-Assets für das Anzeigen-Erlebnis muss ein geeignetes Seitenverhältnis ausgewählt werden. Seitenverhältnisse definieren die proportionale Beziehung zwischen der Breite und Höhe eines Bildes und sind für die Effektivität von Anzeigenplatzierungen von entscheidender Bedeutung. Paid-Media-Kanäle geben sorgfältig gültige Seitenverhältnisse für jede Anzeigenplatzierung auf ihrer Plattform an. Wenn Sie Bild-Assets zu Ihrer Aktivierung hinzufügen, müssen Sie das Seitenverhältnis basierend auf den endgültigen Anzeigenplatzierungen für Ihr Erlebnis auswählen. Dateitypen sind auf JPEG, PNG und GIF beschränkt.

* **Text**: Text umfasst alle Formen von Kopien, die in Ihrer Anzeige enthalten sind, einschließlich Überschriften, Textkörper und call-to-action-Elemente.

* **Metadaten**: Benutzerdefinierte Attribute, die Sie Inhalten zuweisen können. Metadaten verbessern die Leistungsanalyse, Filterung und Verfolgung. Sie ist für Benutzende normalerweise nicht sichtbar.

Das Erstellen einer Aktivierung umfasst das Verfeinern jeder dieser Anzeigenkomponenten für eine bestimmte Kanalplatzierungs- und Marketing-Kampagne. GenStudio for Performance Marketing unterstützt die Aktivierung von einem Erlebnis für einen gebührenpflichtigen Kanal.

## Workflow-Phasen

Obwohl die individuellen Platzierungsanforderungen jeden gebührenpflichtigen Kanal definieren, verwenden alle Anzeigenaktivierungen dieselben allgemeinen Schritte. Die Aktivierung eines Erlebnisses für einen beliebigen gebührenpflichtigen Kanal umfasst drei Kernphasen:

1. **GenStudio for Performance Marketing mit Ihrem Zielkanal verbinden**. Ein GenStudio-System-Manager muss eine Verbindung zu Ihren Kanalkonten herstellen, bevor Sie ein Erlebnis aktivieren können.

1. **Bereiten Sie Ihr Erlebnis für die Aktivierung**. Es gibt zwei Möglichkeiten, Erlebnisse für die Aktivierung vorzubereiten:

   * Aktivieren eines genehmigten Erlebnisses mit vordefinierten Einstellungen direkt aus _[!DNL Content]_. Diese optimierte Methode zur Aktivierung eines oder mehrerer Anzeigenerlebnisse auf einem einzelnen Kanal. Nachdem Sie ein Erlebnis aus der&#x200B;_[!DNL Content]_-Galerie ausgewählt haben, können Sie keine Assets mehr bearbeiten oder zu Ihrem Anzeigenerlebnis hinzufügen. Activate from _[!DNL Content]_&#x200B;ist für Meta- und Google Campaign Manager 360-Anzeigen-Erlebnisse verfügbar.

   * Stellen Sie Ihr Anzeigenerlebnis zusammen, indem Sie visuelle Assets aus _[!DNL Content]_&#x200B;auswählen, Textelemente hinzufügen und Seitenverhältnisse auswählen. Diese Methode umfasst mehr Schritte, bietet jedoch eine größere kreative Flexibilität. Die Vorbereitung umfasst die Auswahl der Medien-Assets im entsprechenden Seitenverhältnis für Ihre spezifische Anzeigenplatzierung und die Zuweisung von Text zu call-to-action-Elementen und Textkörpern. Sie können informative Metadaten hinzufügen, die Benutzende bei der Suche nach dem Erlebnis nach der Aktivierung unterstützen. Jede Anzeigenkanalplatzierung legt gültige Seitenverhältnisse für visuelle Assets fest, die in der Platzierung enthalten sind.

1. **Überprüfen und veröffentlichen Sie Ihr Erlebnis im Zielkanal**. Verwenden Sie das _Vorschau_-Bedienfeld während der Einrichtung des Erlebnisses, um Ihre Auswahl von Anzeigenplatzierungs- und Textelementen zu bewerten, bevor Sie Ihre Aktivierung abschließen. Ihre endgültige Prüfung vor der Veröffentlichung erfolgt in der Anzeigenverwaltungs-App des Zielkanals. Nachdem Sie beispielsweise ein Meta-Anzeigenerlebnis in GenStudio for Performance Marketing aktiviert haben, müssen Sie sich bei Meta Ads Manager anmelden, Ihr Anzeigenerlebnis überprüfen und dann vor der Veröffentlichung seine spezifischen Attribute auswählen.

Sobald ein Anzeigenerlebnis auf seinem Ziel-Kanal für bezahlte Medien live ist, können _[!DNL Insights]_&#x200B;dessen Leistungsdaten verfolgen und analysieren.

## Unterstützte Kanäle

Jeder Paid-Media-Kanal verfügt über einen eindeutigen Aktivierungs-Workflow. Wählen Sie den gebührenpflichtigen Kanal für Aktivierungsrichtlinien aus:

* [Meta](activate-meta-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
