# Scratch Heißluftballon

Einige langjährige GitHub Nutzer würden mich für diesen Gebrauch der Plattform stark kritisieren. Ich bin mir dessen bewusst, das einige von mir genuzte Funktionen von GitHub im speziellen, wie z.B. die Issuedokumentation und allgemeine Git Funktionen nicht so gedacht sind, wie Ich sie hier genutzt habe. Unter [Probleme](#probleme) gehe ich teilweise näher darauf ein, da die spezielle Situatione diese Art der Verwendung nahelegt.

## Inhaltsverzeichniss

- [Scratch Heißluftballon](#scratch-heißluftballon)
  - [Inhaltsverzeichniss](#inhaltsverzeichniss)
  - [Projektinformationen](#projektinformationen)
  - [Inspiration](#inspiration)
  - [Funktionen](#funktionen)
    - [Einstellungen](#einstellungen)
    - [Spielablauf](#spielablauf)
    - [Spielende](#spielende)
  - [Instalation / Anwendung](#instalation--anwendung)
  - [Probleme](#probleme)
    - [Speicherung und Versionierung](#speicherung-und-versionierung)
    - [Eigenheiten Im Programmablauf](#eigenheiten-im-programmablauf)
  - [Danksagung](#danksagung)
  - [Lizenz](#lizenz)

## Projektinformationen

Die Idee zu diesem Spiel stammt aus dem schulischen Informatikunterricht des Wahlpflichtkurses Informatik der Klassenstufe 9.  
Dieses Projekt ist der Einstieg in die Programmierung und für viele meiner Mitschüler das erste selbstgeschriebene Programm überhaupt. Dieses Git-Repository dient dazu, meinen Vortschritt zu versionieren und somit zu belegen, dass der gesamte Code von mir stammt Zudem bietet es mir die Möglichkeit, alle relevanten Pragrammdateien, inklusive des [Programmablaufplans](https://github.com/RedLion8399/Scratch_Hot_air_ballon/blob/master/PAP_1.04.pdf), kurz PAP an einem Ort zu sammeln und zu veröffenlicchen. Dieses sowie weitere Scratch Projekte finden sich im folgenden [Studio](https://scratch.mit.edu/studios/34356533).

Hier noch eine Kurze Zusammenfassung der wichtigsten Rahmendaten:

| Atribut | Wert |
| --- | --- |
| **Entwickler:** | Paul Jonas Dohle |
| **Schule:** | Europagymnasium Warstein |
| **Klasse:** | 9C |
| **Fach** | Informatik |
| **Lehrkraft** | D. Sina |

[![Google Heißluftballon](https://www.googlewatchblog.de/wp-content/uploads/google-play-store-hot-air-balloon-game-screensht.jpg)](https://scratch.mit.edu/projects/941453010 "Hot_air_ballon_1.04")

## Inspiration

Der ein oder andere erinnert sich vielleicht noch daran - Vor einigen Jahren hat Google ein Easter-Egg im Play Store hinzugefügt. Ähnilch wie beim [Chrome Dino](https://chromedino.com/) wurde dieses Spiel angezeigt, sobalt man den Google Play Store im offline Zustand aufrief.  
Offensichtlich wurde das Spiel nach einiger Zeit wieder entfernt, da es in den neusten Versionen des Play Stores nicht mehr enthalten ist. Wer sich eine Aufnahme des "Originalspiels" auf YouTube ansehen möchte, kann dies [hier](https://youtu.be/uBvwNVHg9Rs?t=29) tun.

> In einer der neueren Versionen scheint das Spiel wieder vorhanden zu sein, jedoch lässt es sich nicht si einfach aufrufen, wie bislang. Früher genügte es lediglich das WLAN am Getät zu deaktivieren. In der aktuellen Version hingegen muss das WLAN aktiviert sein, jedoch mit der Einschränkung, dass keine Internetverbindung bestehen darf.

Bis zur Version [0.10.1](https://github.com/RedLion8399/Scratch_Hot_air_ballon/blob/master/Hot_air_ballon_0.10.1.sb3) lag das Augenmerk Hauptsächlich darauf, das Originalspiel möglichst genau nachzubauen. Aufgrund einiger Einschränkungen durch [Scratch](#probleme) kommt diese Version dem "Original" am nächsten.

> Trotz der Ähnlichkeit ist das Spiel in keiner Weise mit Google verbunden, da der gesamte Code von mir als Eigenleistung geschrieben und in keiner Weise von dritten plagiiert wurde.

## Funktionen

Das Programm lässt sich in folgende Hauptfunktionen untergliedern:

### Einstellungen

In den Einstellungen lässt sich das Spiel nach belieben konfigurieren.  
Es besteht die Möglichkeit den Schwierigkeitsgrad nch belieben anzupassen. dazu stehen folgende Parameter zur Verfügung:

- Geschwindigkeit
- Leveldauer
- Boostermenge
- Hindernissmenge
- Boosterdauer

Durch Klicken auf den zurücksetzen Button werden diese auf den Standartwert zurückgesetzt.

---

Zudem kann der Nutzer sowohl die Hintergrundmusik, als auch Soundeffekte sepparat einstellen.  
Der verbliebene Menüpunkt schaltet die Entwicklereinstellungen frei. Diese sind zum Testen des Spiels gedacht. Deren Funktion wird unter [Spielablauf](#spielablauf) näher erläutert.

Außerhalb des Einstellungsfensters befindet sich am oberen Bildschirmrand das Symbol für den Steuerungsmodus. Dem Nutzer stehen insgesammt zwei Steuerungsmodi zur Auswahl. Standart ist die Maussteuerung, wo der Ballon dur das Bewegen der Maus oder das Wischen mit dem Fnger gesteuert wird.  
Der zweite Modus ist die Tastensteuerung. Hier erfolgt die Eingabe über eine Tastatur mittels der Pfeiltasten oder WASD. Zudem werden in der unteren rechten Ecke zwei Pfeile zur Steuerung eingeblendet.

### Spielablauf

Mit Klick auf Start beginnt das Spiel.  
Der Ballon bewegt sich scheinbar nach oben und vom oberen Bildschirmrand "fallen" die sog. "Blasen" und "Hindernisse" herrunter.
Wird eine Blase berührt, werden dem Score 5 Punkte gutgeschrieben und sie verschwindet. Beim berühren eines Hindernisses platzt der Ballon, das Spiel ist vorbei und kann nun durch klick auf "Spielen" neu gestartet werden.  
Etwas seltener können zudem die sog. Booster erscheinen. Diese existieren in zwei Formen, den Magneten und Superballons. Magnete vergrößern für einige Zeit den Einflussbereich des Ballons, dh. es werden Blasen aus einem größeren Umfeld angezogen.  
Durch den Superballon ist der Spieler vor Hindernissen geschützt. Er blinkt bunt und kann währenddessen durch Hindernisse hindurchgleiten.

Während des Spiels wird auf Basis der eingestellten Leveldauer und dem aktuellen Score das Level berechnet. Je höher das Level, desto schneller wird das Spiel im Verhällniss zum ersten Level.

> :bulb: **Tip:** Wenn die Entwicklereinstelungen aktiviert sind, kann ein Magnet durch Drücken der Taste "M" und ein Superballon dur die Taste "S" erzeugt werden.

### Spielende

Es gibt zwei Optionen, warum das Spiel vorbei ist.  
Entweder der Spieler hat verloren oder gewonnen.  
Verloren hat, wer ohne Superballon ein Hinderniss berührt.  
Gewinnen ist hingegen auf zwei Arten möglich. Ereicht der Spieler Level 50 hat er gewonnen. Bei Standerteinstellungen wird das Spiel nähmlich kurtz darauf zu schnell und unspielbar. Darum gibt es eine zweite Option um zu gewinnen. wurde die Geschwindigkeit erhöht, so ist die Grschwindigkeit aus Level 50 bereits früher erreicht. In diesen Fällen hat der Spieler gewonne, sobald er die Geschwindigkeit erreicht, die bei Standorteinstellungen für Level 50 gillt.

Sollte das Spiel aus einem der genannten Gründer vorbei sein, wird geprüft, ob der bisherige High Score an Score Punkten gebroche wurde. bei standarteinstellungen sind maximal 10000 nötig um zu gewinnen. Sollte diese Grenze erreicht sein, muss die Leveldauer erhöht werden um den Rekord zu überbieten.

## Instalation / Anwendung

Das Projekt befindet sich unter anderem als öffentliches Projekt auf [Scratch](https://scratch.mit.edu/projects/941453010). Dort kann es gespielt und auch abgespiechert werden. Jedoch lässt sich dort immer nur eine einzige Version gleichzeitig einsehen. Diese muss nicht immer der atuellsten Version entsprechen, sollte jedoch keine offensichtlichen Buggs beinhalten. Dort kann mit dem Spiel interagiert werden. Dort lassen sich Lieblingsprojekte markieren und mit einem Herz auszeichnen. Für Lob und Kritik gibt es dort eine Kommentarfunktion.
Die Vollständige Versionshistorie befindet sich hier auf GitHub. Hier sind alle Änderungen in jewails einem Commit dukumentiert. Da hier jede Version als einzelne Datei aufgeführ ist, besteht die Möglichkeit, eine einzelne Datei gezielt herrunterrunterzuladen und zu spielen / editieren. Diese Datei kann nun im [Browser](https://scratch.mit.edu/projects/editor "Faxgeräte gehen nicht") oder in der [Desktop Anwendung](https://scratch.mit.edu/download "Klicken zu Download") geöffnet werden.  
Besteht interesse am vollständigen Git Repository, so empfielt es sich, sofern [Git](https://git-scm.com/downloads "Auch das geht nicht mit einem Faxgerät") bereits installiert ist, das gesamte Repository zu Klonen. Dies ist am einfachsten mittels GUI, geht jedoch auch über die Komandoszeile.
dazu erst in den richtigen Ordner navigieren:

```sh
cd # Ordnername \ Unterordner Name
```

und dann den Befehl zum Klonen aufrufen:

```sh
git clone https://github.com/RedLion8399/Scratch_Hot_air_ballon.git
```

Um den Code zu verstehen sind einige Grundkentnisse in Scrstch erforderlich. Durch häufige Komentare  und sinvolle Bezeichner sollte er jedoch selbsterklärend sein.

## Probleme

### Speicherung und Versionierung

Wie eingangs angedeutet führt die Verwendung von Scratch als Programmiersprache zu einigen Problemen. Um Scratch Dateien zu eitieren gibt es zwei Methooden. Die simpeste Variante besteht darin, die Projekte im Browser zu editieren und bei Scratch zu speichern. Diese Variante bietet sich vorallem an, wenn das Projekt öffentlich ist, da solche ohnehin online gespeichert werden müssen. In diesem Fall kann es aber z.B. aufgrund einer schlechten WLAN Verbinding zu Absturtz der Seite kommen, was einen Verlust der Projetdaten zur Folge haben kann.
Aus diesem Grund empfielt es sich, vollständig in der App zu entwickeln, die keine Internetverbindung benötigt und  / oder das Projekt regelmäßig lokal in Form von sb3-Dateien abzuspeichern. Leider sind die Scratch-Anwendungen nicht dafür ausgelegt, eine bestehende Sratch Datei zu modifiziren. Stattdessen muss eine sb3-Datei im Scratch Editor geöffnett und nach beendigung unter neuem Namen abgespeichert werden.  
Diese Form der Dateinspeicherung erschwert eine Versionierung mittels Git deutlich und führt zu jeder Form, die in diesem Repository zu sehen ist.

### Eigenheiten Im Programmablauf

Anders als bei einfachen Programmen mit herkömmlichen, textbasierte Sprachen, werden Scratchbefehle nicht chronologisch nacheinander, sondern oft passraleel ausgeführt, sofern diese über identische Startparameter verfügen. Zudem übernimmt Scratch einige Komponente der Objektorrientierten Programmierung in Form von "Figuren".  
Leider haben diese Figuren untereinander nur sehr eingeschränkte Kommunikationsmöglichkeiten, denn obwohl es die Möglichkeit gibt, "Eigene Blöcle" - also Funktionen - zu erstellen, können diese nicht außerhalb der Figur genztzt werden.
Daraus resultiert, dass es für den folgenden Fall:

> - Es gibt zwei Figuren A und B
> - Für beide müssen zu dierekt beginn des Programms einige einstellungen vorgenommen werden
> - A muss vor B initialisiert werden, da sonst der restliche Programmablauf gestört würde

keine elegante und zugleich simple Lösung gibt, da beide Figuren initialisiert werden, sobald das Programm startet und es reiner Zufall ist, ob zuerst A oder B die kritische Stelle durchläuft.
Ähnliche Probleme zeichnen sich auch in diesem Projekt ab. z.B. werden bei der jewails ersten Interaktion oft Geräusche abgespielt, obwohl die Ton standartmäßig auf lautlos eingestellt ist.

## Danksagung

Die verwendeten Grafiken sind entweder dem Originalspiel nachempfunden und selbstgezeichnet oder sie stammen von [Font Awesome](https://fontawesome.com/ "Immernoch kein Faxgerät") und wurden farblich und qualitativ angepasst.  
▷ Musik von Ronald Kah, [Web](https://ronaldkah.de)

## Lizenz

Dieses Projekt ist mit der [MIT-Lizenz](https://github.com/RedLion8399/Scratch_Hot_air_ballon/blob/master/LICENSE) lizensiert.
