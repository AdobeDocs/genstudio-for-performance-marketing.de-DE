---
title: Optimieren der Aktivierung
description: Erfahren Sie, wie Sie Aktivierungen für bezahlte Anzeigenkanäle von Drittanbietern optimieren können.
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Optimieren von Aktivierungen

Die Aktivierung eines Anzeigenerlebnisses für Paid-Ad-Kanäle umfasst zwei Hauptphasen:

* Vorbereiten Ihres Erlebnisses für die Aktivierung

* Veröffentlichen Ihres Erlebnisses auf dem dafür vorgesehenen bezahlten Kanal und in den dafür zuständigen Managern

Die Befolgung der Best Practices beim Erstellen und Aktivieren Ihres Anzeigen-Erlebnisses kann dazu beitragen, potenzielle Komplikationen oder Fehler beim Versand an die Zielkanäle zu minimieren.

## Best Practices

Im Folgenden finden Sie einige gängige Best Practices und die Fehler, die sie verhindern können.

* **Verwenden gültiger, vollständiger Ziel-URLs**

  Ungültige URLs können Trigger verursachen. Beispielfehler: _Die eingegebene URL führt nicht zu einer Website. Bitte eine gültige URL eingeben und erneut versuchen. (100)_

* **Stellen Sie sicher, dass die Token-Gültigkeit von Ihrer Anwendung korrekt verarbeitet wird**

  Anwendungen sollten bei Bedarf neue Token anfordern. Authentifizieren Sie sich bei Bedarf erneut und rufen Sie ein neues Zugriffstoken ab, indem Sie sich erneut anmelden oder die Sitzung aktualisieren. Beispielfehler: _Fehler beim Überprüfen des Zugriffs-Tokens: Die Sitzung wurde ungültig gemacht, da der Benutzer sein Kennwort geändert hat oder Facebook die Sitzung aus Sicherheitsgründen geändert hat. (190)_

* **Überprüfen Sie Ihren Anzeigensatz und stellen Sie sicher, dass immer nur eine Anzeige aktiv ist**

  Wenn Sie mehrere Meta-Anzeigen aktivieren müssen, erstellen Sie für jedes davon einen separaten Dynamic Creative-Anzeigensatz. Beispielfehler: _Dynamic Creative-Anzeigensatz lässt maximal eine aktive Anzeige darin zu. Benutzende dürfen nicht mehr als eine Anzeige unter demselben Dynamic Creative-Anzeigensatz erstellen. (100)_

* **Gleicht die Anzahl der angewendeten Regeln mit dem von der Plattform angegebenen Betrag ab**

  Bezahlte Kanäle erwarten, dass die Anzahl der angewendeten Regeln ihrem angegebenen Format entspricht.  Passen Sie bei Bedarf die Anzahl der Regeln an den von der Plattform angegebenen Wert an. Beispielfehler: _Der Anzeigen-Asset-Feed hat X Zielregel(n) für Format: Formatname, aber es wird genau X Zielregel für dieses Format erwartet. (100)_

* **Wählen Sie eine call-to-action (CTA) aus, die mit Ihrem Anzeigenziel kompatibel ist**

  Aktionsaufrufe, die mit dem Ziel in Dynamic Creative Ad inkompatibel sind, geben dem Trigger einen Fehler. Beispielfehler: _Der call to action-Typ X wird für das Ziel Y in Dynamic Creative Ad Set nicht unterstützt. (100)_

* **Stellen Sie sicher, dass die Begrenzung des Zielanzeigensatzes die Anzahl der Anzeigenerlebnisse unterstützt**

  Bestätigen Sie, dass das Anzeigenlimit des Zielgruppen-Anzeigensatzes Ihren aktivierten Anzeigenerlebnissen entsprechen kann. Entfernen Sie bei Bedarf alle unnötigen oder inaktiven Anzeigen aus dem Anzeigensatz, um innerhalb dieses Limits zu bleiben. Alternativ können Sie einen neuen Anzeigensatz erstellen, um zusätzliche Anzeigen zu aktivieren. Beispielfehler: _Sie haben die Kampagnen-, Anzeigensatz- oder Anzeigenbeschränkungen pro Werbekonto erreicht. Jeder Anzeigensatz kann maximal 50 Anzeigen enthalten. Dazu gehören pausierte/inaktive/ausgeschaltete Anzeigen. (100)_

* **Stellen Sie sicher, dass die Plattform Ihren ausgewählten CTA-Typ unterstützt**

  Vergewissern Sie sich, dass Ihr Erlebnis einen unterstützten CTA-Typ enthält. Beispielfehler: _(#100) Ungültiger call to action-Typ (100)_
