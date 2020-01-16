---
layout: post
title: "Welcome to desklab"
date: 2020-01-16 21:41:00 -0400
category: getting-started
short-description: A quick overview to get you started
---

## Erste Schritte
1. Installation des MC-Treibers
2. Installation der Arduino IDE
3. Installation der benötigten Bibliotheken
  - Installation in der Arduino IDE
  - manuelle Installation
4. Upload eines Programms

### Mikrocontroller-Treiber: Download & Installation

[Link zu MC Treiber](https://desk-lab.de/)

### Arduino IDE (Entwicklungsumgebung): Download & Installation

[Link zu Arduino IDE](https://www.arduino.cc/en/main/software)

### Arduino Bibliotheken
##### Installation in Arduino IDE
Zur Nutzung der desklab Geräte werden drei Arduino-Bibliotheke benötigt:
- ``desklab``
- ``Adafruit_SSD1306``
- ``Adafruit_GFX``

![library manager](screenshot-library-manager.png)

##### manuelle Installation
[Link zu desklab Arduino library](https://github.com/desklab/desklab-arduino-lib/releases)

[Link zu Adafruit GFX](https://github.com/adafruit/Adafruit-GFX-Library/releases)

[Link zu Adafruit SSD1306](https://github.com/adafruit/Adafruit_SSD1306/releases)

##### Upload eines Beispiel-Programms
Um zu testen, ob alle Schritte erfolgreich durchgeführt wurden, kann ein Beispielprogramm auf den Mikrocontroller geladen werden. Dazu muss die Arduino IDE gestartet und der Mikrocontroller per USB Kabel angeschlossen werden.

Nach dem Start der Arduino IDE sollte zum Test folgender Code eingegeben und danach der Sketch (Bezeichnung für ein Programm) gespeichert werden.

```c++
// Minimalbeispiel zum Test der Installation der Bibliothek
#include <desklab.h>

setup(){
  StarteDisplay();
}

loop(){
  TextAusgabe("Hallo!", 2);
}
```
Danach kann der Sketch Kompiliert und auf den Mikrocontroller geladen werden. Nach wenigen Sekunden sollte der Upload auf den Mikrocontroller abgeschlossen sein und das Programm wird automatisch gestartet. Erscheint jetzt auf dem Display ``Hallo!``, wurden die Entwicklungsumgebung und die Bibliotheken erfolgreich installiert.
