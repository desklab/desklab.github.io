---
layout: post
title: "Title of article"
date: 2019-11-05 08:44:38 -0400
category: using-library
short-description: description of article
---

## Troubleshooting


### xxxxxx.h: No such file or directory
**Fehler:**
```
In file included from C:\...\PhotometerDetailed.ino:13:0:

C:\.../desklab.h:35:10: fatal error:Adafruit_SSD1306.h: No such file or directory

#include <Adafruit_SSD1306.h>
          ^~~~~~~~~~~~~~~~~~~~

compilation terminated.

exit status 1
Fehler beim Kompilieren für das Board Arduino Uno.
```
**Erklärung:** Die Fehlermeldung `Adafruit_SSD1306.h: No such file or directory` bedeutet, dass ein **Fehler beim Einbinden der Adafruit_SSD1306 - Bibliothek** aufgetreten ist. Vermutlich ist diese Bibliothek nicht (oder nicht korrekt) installiert.


---
**Fehler:**
```
In file included from C:\.../desklab.h:35:0,

C:\.../Adafruit_SSD1306.h:41:10: fatal error: Adafruit_GFX.h: No such file or directory

#include <Adafruit_GFX.h>
          ^~~~~~~~~~~~~~~~

compilation terminated.

exit status 1
Fehler beim Kompilieren für das Board Arduino Uno.
```
**Erklärung:** Die Fehlermeldung `Adafruit_GFX.h: No such file or directory` bedeutet, dass ein **Fehler beim Einbinden der Adafruit_GFX - Bibliothek** aufgetreten ist. Vermutlich ist diese Bibliothek nicht (oder nicht korrekt) installiert.

### expected ';' before '...'

**Fehler:**
```
In C:\...\SketchName.ino:

SketchName:6:1: error: expected ';' before '...'

exit status 1
```
**Erklärung:** Die Fehlermeldung `expected ';' before '...'` bedeutet, dass ein **Semikolon fehlt**. Der Fehler tritt (in diesem Beispiel) in Zeile 6 auf, das bedeutet dass das Semikolon am Ende der Zeile 5 fehlt.

### undefined reference to '...'

**Fehler:**
```
C:\...: In function `main':

C:\.../main.cpp:43: undefined reference to `setup'

collect2.exe: error: ld returned 1 exit status

exit status 1
Fehler beim Kompilieren für das Board Arduino Uno.
```
**Erklärung:** Die Fehlermeldung `undefined reference to 'setup'` bedeutet, dass der **'setup'-Teil des Sketches nicht gefunden** wurde.

---
**Fehler:**
```
C:...: In function `main':

C:\.../main.cpp:46: undefined reference to `loop'

collect2.exe: error: ld returned 1 exit status

exit status 1
Fehler beim Kompilieren für das Board Arduino Uno.
```
**Erklärung:** Die Fehlermeldung `undefined reference to 'loop'` bedeutet, dass der **'loop'-Teil des Sketches nicht gefunden** wurde.





## IDE Fehler
### COM Port
```
Der Sketch verwendet 444 Bytes (1%) des Programmspeicherplatzes. Das Maximum sind 32256 Bytes.
Globale Variablen verwenden 9 Bytes (0%) des dynamischen Speichers, 2039 Bytes für lokale Variablen verbleiben. Das Maximum sind 2048 Bytes.
Beim Hochladen des Sketches ist ein Fehler aufgetreten
```
-> falscher COM Port ausgewählt

### Board
```
.
.
.
avrdude: error: programmer did not respond to command: exit bootloader
```
```
.
.
.
avrdude: stk500v2_getsync(): timeout communicating with programmer
Beim Hochladen des Sketches ist ein Fehler aufgetreten
```

-> falsches Board ausgewählt
