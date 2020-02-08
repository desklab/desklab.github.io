---
layout: post
title: Installation & Erste Schritte
date: 2020-01-16 21:41:00 -0400
category: getting-started
short-description: Beschreibung der ersten Schritte zur Installation der Photometer-Software
---

In diesem Artikel wird beschrieben, wie die Geräte der desklab gUG zusammen mit der Arduino-Entwicklungsumgebung und der bereitgestellten Software-Bibliothek programmieren zu können.

Bei Fragen oder Problemen, auf die Sie in den Hilfe-Artikeln dieser Seite keine Lösung finden, können
Sie uns gerne über das Kontaktformular auf unserer [Homepage](www.desk-lab.de) kontaktieren.

## Übersicht
1. Installation des Mikrocontroller-Treibers
2. Installation der Arduino Entwicklungsumgebung
3. Installation der benötigten Bibliotheken
4. Upload eines Beispiel-Programms

---
### 1. Mikrocontroller-Treiber: Download & Installation

Um den in den Geräten der desklab gUG verbauten Mikrocontroller mit der Arduino-Entwicklungsumgebung
programmieren zu können, benötigen Sie den Treiber
CH341SER.
Die zur Installation benötigten Dateien können Sie von unserer Homepage herunterladen. Sie benötigen dazu die Login-Daten, die Sie zusammen mit der Lieferung oder per E-Mail erhalten haben.

Führen Sie zur Installation des Treibers die folgenden Schritte durch:
1. Trennen Sie per USB angeschlossene desklab-Geräte
von Ihrem Computer.
2. Laden Sie die Installationsdatei
mc_treiber_CH341SER.zip ([Downloadlink](https://desk-lab.de/documents/7/mc-treiber_CH341SER.zip))
von unserer Website herunter.
3. Speichern und Entpacken Sie die heruntergeladene
Datei.
4. Führen Sie die Datei "Setup.exe" aus.
5. Wählen Sie im darauf erscheinenden Dialogfenster
“Install” aus und befolgen Sie eventuell erscheinende
Mitteilungen.

---
### 2. Arduino IDE (Entwicklungsumgebung): Download & Installation

Wir empfehlen, die Version 1.8.10 der Arduino-Entwicklungsumgebung zu installieren. Diese ist zum Zeitpunkt der letzten Überarbeitung dieses Dokumentes (01.01.2020) die aktuellste von Arduino® zur Verfügung gestellte Version. Die zur Installation benötigte(n) Datei(en) können unter [https://www.arduino.cc/en/Main/Software](https://www.arduino.cc/en/Main/Software) heruntergeladen werden. Befolgen Sie zur Installation die dort beschriebenen Schritte.

Die Kompatibilität der desklab-Bibliothek (s.u.) mit folgenden Versionen der Arduino Entwicklungsumgebung wurde von uns getestet und sichergestellt:

- Arduino 1.8.10 (Release 2019)
- Arduino 1.8.9 (Release 2019)
- Arduino 1.8.8 (Release 2018)
- Arduino 1.8.7 (Release 2018)
- Arduino 1.8.6 (Release 2018)
- Arduino 1.8.5 (Release 2017)

Falls Sie eine nicht aufgeführte Version der Arduino-Entwicklungsumgebung nutzen, können bei der Nutzung der Funktionen der desklab-Bibliothek Probleme und Fehler auftreten.

---
### 3. Arduino Bibliotheken
##### Installation in Arduino IDE
Zur Nutzung der desklab Geräte werden drei Arduino-Bibliotheken benötigt:
- ``desklab``
- ``Adafruit_SSD1306``
- ``Adafruit_GFX``

In der desklab Arduino Bibliothek werden Funktionen zur Nutzung und Programmierung der Geräte der desklab gUG bereitgestellt. Die Bibliothek kann in der Bibliotheksverwaltung der Arduino-Entwicklungsumgebung installiert werden.

Führen Sie zur Installation der Arduino-Bibliothek die folgenden Schritte durch:
1. Trennen Sie per USB angeschlossene desklab-Geräte
von Ihrem Computer.
2. Öffnen Sie die Arduino-Entwicklungsumgebung.
3. Öffnen Sie die Bibliotheksverwaltung über die
Menüleiste der Entwicklungsumgebung:
4. ...

![library manager]({{site.url}}/assets/screenshot-library-manager.png)

##### manuelle Installation

Wenn Sie die Bibliotheken manuell installieren möchten finden Sie die dazu benötigten Dateien unter folgenden Links:
- [desklab Arduino library](https://github.com/desklab/desklab-arduino-lib/releases)
- [Adafruit GFX library](https://github.com/adafruit/Adafruit-GFX-Library/releases)
- [Adafruit SSD1306 library](https://github.com/adafruit/Adafruit_SSD1306/releases)

---
### 4. Upload eines Beispiel-Programms
In der desklab Arduino Bibliothek sind drei Beispielprogramme enthalten, mit denen das
Photometer der desklab gUG zur Messung der optischen Dichte genutzt werden kann.

Um zu testen, ob alle Schritte erfolgreich durchgeführt wurden, kann ein Beispielprogramm auf den Mikrocontroller geladen werden. Dazu muss die Arduino IDE gestartet und der Mikrocontroller per USB Kabel angeschlossen werden.

Nach dem Start der Arduino IDE sollte zum Test ein Beispiel-Sketch der Bibliothek kompiliert und auf den Mikrocontroller geladen werden. Nach wenigen Sekunden sollte der Upload auf den Mikrocontroller abgeschlossen sein und das Programm wird automatisch gestartet.

Sollte das Display keine Anzeige starten oder die Arduino-Entwicklungsumgebung eine Fehlermeldung ausgeben, finden Sie in den folgenden Artikeln weitere Informationen zur Fehlerbehebung.

- [Fehlermeldungen der Entwicklungsumgebung](https://support.desk-lab.de)
- [Probleme mit dem Arduino-Modul](https://support.desk-lab.de)
