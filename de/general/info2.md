# 📜 Cloury Informationsstruktur

## `/rules`

### Das zentrale Regelwerk

Die Hauptseite `/rules` erklärt das gesamte Regelsystem und führt zu den einzelnen Bereichen.

```text
/rules

📜 Cloury Network Regelwerk
│
├── 🌐 Allgemeine Regeln
│   └── /rules/general
│
├── 🎮 Spiele
│   └── /rules/games
│       ├── /rules/games/bedwars
│       ├── /rules/games/...
│       └── ...
│
├── 🎉 Events
│   └── /rules/events
│       ├── Aktuelle Events
│       └── Vergangene Events
│
├── 👥 Team-Regelwerk
│   └── /rules/team
│       ├── Allgemeines Team-Regelwerk
│       ├── Rangrechte & Zuständigkeiten
│       ├── Build Server
│       └── ...
│
└── ⚖️ Strafen
    └── /rules/punishments
```

Dabei ist wichtig:

> **Die allgemeinen Regeln gelten grundsätzlich überall.**
> Spielmodi und Events können zusätzliche Regeln festlegen. In ihrem jeweiligen Geltungsbereich können sie allgemeine Regeln ergänzen oder – wenn ausdrücklich festgelegt – außer Kraft setzen.

Damit wäre die grundlegende Regel-Hierarchie klar definiert.

---

# 🌐 `/rules/general`

Das ist das **Grundregelwerk des gesamten Cloury Networks**.

Hier stehen alle Regeln, die grundsätzlich für Spieler gelten, zum Beispiel:

* Verhalten
* Respekt
* Chat
* Beleidigungen
* Spam
* Werbung
* Cheating
* Hacks
* Unerlaubte Mods
* Bugusing
* Exploiting
* Scamming
* Accountmissbrauch
* Umgehung von Strafen
* Umgang mit persönlichen Daten
* Ausnutzung von Fehlern
* Befolgen von Team-Anweisungen
* usw.

Ganz oben könnte zum Beispiel stehen:

> Mit dem Betreten und der Nutzung des Cloury Networks erklärst du dich mit den geltenden Regeln einverstanden. Die allgemeinen Regeln gelten auf dem gesamten Netzwerk, sofern für einen bestimmten Bereich oder Spielmodus keine abweichenden Regeln festgelegt wurden.

Damit wäre das Fundament für das gesamte Regelwerk geschaffen.

---

# 🎮 `/rules/games`

Hier würde ich **keine langen Regeln** schreiben.

Die Seite erklärt stattdessen kurz das System:

> Auf Cloury gelten für jeden Spielmodus die allgemeinen Regeln. Zusätzlich können einzelne Spielmodi eigene Regeln besitzen, die speziell auf ihre Spielmechaniken und Besonderheiten zugeschnitten sind.

Danach werden die einzelnen Spiele angezeigt:

```text
BedWars
SMP
Citybuild
...
```

Für jedes Spiel könnte man anzeigen:

* Name
* Kurze Erklärung
* Status
* Ob eigene Regeln vorhanden sind
* Link zum jeweiligen Spielmodus

---

# 🎮 `/rules/games/bedwars`

Hier wird es interessanter.

Eine Game-Regelseite würde ich in **zwei Bereiche** aufteilen.

## 1. Das Spiel erklären

Zum Beispiel:

> BedWars ist ein Team-basiertes Spiel, bei dem Spieler ihre Basis und ihr Bett schützen müssen.

Also genau das, was du beschrieben hast: **Auf den Game-Seiten darf auch erklärt werden, wie das jeweilige Spiel funktioniert.**

## 2. Die Regeln

Danach kommen die eigentlichen Regeln:

* Allgemeine Regeln gelten
* BedWars-spezifische Regeln
* Verbotene Strategien
* Exploits
* Teaming
* Verhalten
* Spezielle Spielmechaniken

### Regel-Hierarchie

```text
Allgemeine Regeln
       ↓
Game-Regeln
       ↓
Spezielle Event-Regeln
```

Wenn eine Game-Regel einer allgemeinen Regel widerspricht, gilt für diesen Spielmodus die spezielle Game-Regel.

Beispiel:

> Allgemeine Regel: Eine bestimmte Aktion ist verboten.
> BedWars-Regel: Diese Aktion ist in BedWars ausdrücklich erlaubt.

Dann gilt **für BedWars die spezielle BedWars-Regel**.

Wichtig ist allerdings, dass solche Ausnahmen immer **klar und ausdrücklich formuliert** werden. So muss niemand selbst interpretieren, welche Regel in diesem Fall gilt.

---

# 🎉 `/rules/events`

Die Event-Regeln würde ich ähnlich wie die Game-Regeln aufbauen. Allerdings gibt es hier einen wichtigen Unterschied.

## Aktuelle Events

Hier werden alle Events angezeigt, deren Regeln aktuell gelten.

Zum Beispiel:

```text
🎉 Summer Event 2026
Regeln gültig bis: 31.08.2026
→ Regeln ansehen

🏆 Cloury Tournament
Regeln gültig bis: 15.08.2026
→ Regeln ansehen
```

Die Regeln könnten dann zum Beispiel unter folgendem Pfad liegen:

`/rules/events/summer-2026`

---

## Vergangene Events

Nach dem Ende eines Events werden die Regeln **nicht sofort gelöscht**.

Sie bleiben noch **7 Tage öffentlich verfügbar**. Danach verschwinden sie aus dem öffentlichen Regelwerk.

Das finde ich sinnvoll, weil:

* Spieler noch nachschauen können, welche Regeln bei einem gerade beendeten Event galten.
* Das Regelwerk nicht mit alten Events überladen wird.
* Die aktuelle Übersicht trotzdem sauber und übersichtlich bleibt.

Auf `/events` selbst können natürlich deutlich länger Informationen zum Event bestehen bleiben.

Damit hätten wir eine klare Trennung:

**`/events` = Event-System, Informationen, Teilnahme, Ergebnisse**

**`/rules/events` = ausschließlich die Regeln der Events**

---

# 👥 `/rules/team`

Hier würde ich die **Team-Regeln** bündeln.

An dieser Stelle kommt auch die Unterscheidung zwischen **Team Wiki** und **Team Rules** ins Spiel.

### Team Wiki

> **Wie funktioniert etwas?**

### Team Rules

> **Was darf ich? Was muss ich? Was ist verboten?**

Beispiel:

**Team Wiki:**

> Wie funktioniert das Ticketsystem?

**Team-Regelwerk:**

> Teammitglieder dürfen keine internen Ticketinformationen außerhalb des Teams weitergeben.

Die Hauptseite des Team-Regelwerks könnte zum Beispiel erklären:

> Das Team-Regelwerk enthält verbindliche Regeln und Richtlinien für Teammitglieder des Cloury Networks. Je nach Rang, Aufgabe und Einsatzbereich können zusätzliche Regeln und Berechtigungen gelten.

Danach könnten die einzelnen Bereiche folgen:

```text
/rules/team

👥 Allgemeines Team-Regelwerk
🎖️ Ränge, Rechte & Zuständigkeiten
🛠️ Build Server
🖥️ Server & Systeme
🛡️ Moderation
🔒 Datenschutz & Vertraulichkeit
⚖️ Teaminterne Maßnahmen
```

---

# 🛠️ `/rules/team/build-server`

Das wäre dann genau dein Beispiel.

Hier stehen Regeln wie:

* Wer darf den Build Server betreten?
* Wer darf dort bauen?
* Welche Teamränge dürfen welche Bereiche nutzen?
* Wer darf WorldEdit verwenden?
* Wer darf Projekte erstellen?
* Wer darf bestehende Builds verändern?
* Wer darf Builds freigeben?
* Wer darf anderen Zugriff geben?
* Was darf nicht gemacht werden?
* Was passiert bei Missbrauch?

Das ist **kein Wiki**.

Das Team Wiki könnte erklären:

> **So funktioniert der Build Server.**

Das Regelwerk sagt dagegen:

> **Das darfst du auf dem Build Server.**

Diese Trennung finde ich sehr wichtig.

---

# 🎖️ Rangrechte – meine Empfehlung

Hier würde ich **keine riesige Permission-Tabelle** erstellen.

Also nicht:

| Permission   | Jr. Supporter | Supporter | Sr. Supporter |
| ------------ | ------------- | --------- | ------------- |
| Permission 1 | ✓             | ✓         | ✓             |
| Permission 2 | ✗             | ✓         | ✓             |

Solche Tabellen werden schnell unübersichtlich und veralten leicht.

Stattdessen würde ich eine **leicht verständliche Rangübersicht** erstellen.

Zum Beispiel:

### Jr. Supporter

**Darf:**

* Spieler unterstützen
* Bestimmte Support-Aufgaben übernehmen

**Darf nicht:**

* Eigenständig Moderationsmaßnahmen durchführen
* Interne Teamentscheidungen treffen

**Zuständig für:**

* Spieler-Support
* Einfache Fragen

Danach könnte man beim nächsthöheren Rang schreiben:

### Supporter

**Zusätzlich zu den Rechten des Jr. Supporters:**

* ...

Das hat zwei große Vorteile:

1. Neue Teammitglieder verstehen sofort ihre Rolle.
2. Die Übersicht ist deutlich einfacher zu aktualisieren.

Die **technischen Permissions** würde ich meiner Meinung nach nicht ins Regelwerk aufnehmen. Diese gehören eher ins Team Wiki oder in eine interne technische Dokumentation.

---

# ⚖️ `/rules/punishments`

Hier würde ich **nicht den kompletten Strafenkatalog** veröffentlichen.

Die Seite sollte nur erklären, welche Arten von Sanktionen grundsätzlich möglich sind.

Zum Beispiel:

* Verwarnung
* Mute
* Kick
* Temporärer Ausschluss
* Permanenter Ausschluss
* Ausschluss von Events
* Einschränkung bestimmter Funktionen

Danach könnte dort stehen:

> Die konkrete Maßnahme richtet sich nach der Art und Schwere des Verstoßes, bisherigen Verstößen sowie den Umständen des jeweiligen Falls.

**Wann welche Strafe angewendet wird**, gehört meiner Meinung nach ins **Team-Regelwerk**.

Damit hätten wir eine klare Trennung:

```text
/rules/punishments
↓
Welche Strafen gibt es grundsätzlich?

/rules/team
↓
Wie entscheidet das Team über Strafen?
```

Das würde ich genau so umsetzen.

---

# 🧩 Das komplette Cloury-System

Damit hätten wir am Ende **drei große Informationsbereiche**:

## 📜 Rules

**Was ist erlaubt? Was ist verboten?**

```text
/rules
/rules/general
/rules/games
/rules/games/...
/rules/events
/rules/events/...
/rules/team
/rules/team/...
/rules/punishments
```

## 📚 Wiki

**Wie funktioniert etwas?**

```text
/wiki
/wiki/...
```

## 🔐 Team Wiki

**Wie funktioniert etwas intern für das Team?**

```text
/team/wiki
/team/wiki/...
```

Diese Trennung finde ich für Cloury sehr sinnvoll, weil sich die Systeme dadurch nicht unnötig überschneiden.

Ein Beispiel:

> **BedWars-Regel:** „Das absichtliche Ausnutzen von Bugs ist verboten.“
> → `/rules/games/bedwars`

> **BedWars erklärt:** „So funktioniert BedWars.“
> → `/wiki/bedwars`

> **Wie wird ein BedWars-Event technisch erstellt?**
> → `/team/wiki/events`

> **Welche Rechte hat ein Moderator bei einem BedWars-Verstoß?**
> → `/rules/team/moderation`

So hat jeder Inhalt seinen festen Platz.

--
