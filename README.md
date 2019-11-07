# Projektseite

## Inhaltsverzeichnis

[Vorwort](#1)

[Der Arduino](#2)

  [Der Sketch](#3)
  
[Projektentwicklung](#4)

[Unser Projekt](#5)

[Unsere Hardware](#6)

### <a name="1"></a>Vorwort

Vor dem Informatikunterricht hatten wir beide keine Vorkenntnisse. Deshalb waren wir gespannt was auf uns zukommt. Als es dann darum ging, eine Projektidee zu finden und wir uns einen Überblick über alle Möglichkeiten verschafft hatten, entschieden wir uns für ein praktisches Projekt. Das Programmieren an etwas Praktischem zu erlernen erschien uns sehr sinnvoll. Somit kam für uns der sehr anfängerfreundliche Arduino in Frage. Da es im Internet sehr viele fertige Projekte inklusive Anleitungen gibt, wir aber ein eigenständiges und neues Projekt umsetzten wollten, mussten wir uns erst einmal etwas eigenes ausdenken. Relativ schnell kamen wir auf die Ideen ein Parkhaus zu bauen, dessen Schranke nur so lange aufgeht, wie Parkplätze frei sind. Ein großer Vorteil daran war, dass wir das große Projekt aus mehreren kleineren aufbauen konnten. So ist es möglich, auf funktionierenden Zwischenschritten aufzubauen. Wenn ein kleinerer Schritt nicht funktioniert, ist nicht gleich das ganze Projekt gescheitert. Dieses Prinzip war die Grundlage unserer gesamten Arbeit.

### <a name="2"></a>Der Arduino

Ein Arduino ist eine Physical-Computung-Plattform, die aus Soft- und Hardware zusammengesetzt ist. Hierzu benötigt man das Arduino-Programm auf dem Computer für die Software und einen Mikrocontroller für die Hardware. In der Software schreibt man einen sogenannten "Sketch", den man anschließend auf den Mikrocontroller übertragen kann. An den Mikrocontroller kann man verschiedene Geräte wie Sensoren, LEDs oder Servos anschließen und per Sketch auslesen bzw. steuern. Die Stromversorgung liefert der Computer oder man schließt einen Akku an. Um mehrere angeschlossene Geräte gleichzeitig mit Strom und Daten zu versorgen bzw. auszulesen, nutzt man ein sogenanntes "Breadboard", über das man die 5V des Microcontrollers an die Geräte weiterverteilen kann.   
![Arduino_Mikrocontroller und Breadboard](https://github.com/dennis602/Projektseite/blob/master/Arduino%20Bild%20Internet.jpg)

### <a name="3"></a>Der Sketch

Die zwei Bestandteile eines Sketches sind das "void setup()" und das "void loop()". Im Setup werden alle Ausgangsbedingungen definiert, wie zum Beispiel, welche Geräte benutzt werden und an welchen Pins auf dem Mikrocontroller diese angeschlossen sind. 
Beispiel: 

![Sketch Beispiel](https://github.com/dennis602/Stundenprotokoll/blob/master/1.%20Sketch.PNG)

Dies war unser erster Sketch, der eine LED am Pin 13 zum blinken bringt. Das "delay(...)" bestimmt die Zeit, die die LED "HIGH" (also an) oder "LOW" (also aus) ist.
 
### <a name="4"></a>Projektentwicklung

Wir haben unser Projekt damit begonnen, im Internet grundlegende erste Schritte im Umgang mit dem Arduino zu recherchieren. Sobald wir diese verinnerlicht hatten, haben wir uns komplexeren Sachverhalten gewidmet. Diese Vorgehensweise hat unsere gesamte Arbeitsweise bestimmt. Schritt für Schritt von Einfach zu Schwer. Wir haben also damit begonnen, einfache LEDs zum leuchten zu bringen, Servos zu steuern oder Sensoren einzusetzten. Anschließend ging es darum, all diese Schritte zu verknüpfen.

Dieses Verknüpfen lief natürlich nicht problemlos ab, sodass die zentrale Herausforderung das Lösen dieser Probleme war. Mit jeder dieser Lösungen wuchs auch unser allgemeines Verständnis für das Programm Arduino. Wir haben gelernt, einzelne Abschnitte des Sketches genauer auf die Funktionalität zu untersuchen, indem wir einzelne Zeilen deaktiviert haben. Sehr geholfen hat uns auch der "Serial Print" als Möglichkeit, den aktuellen Status des ablaufenden Sketches nachzuvollziehen.

Da wir die einzelnen Anleitungen der Schritte im Internet recherchiert haben (Quellen s. Protokoll), lag unsere Eigenleistung darin, all diese kleinen Skechte zu einem großen zu verbinden. Ziel war von Anfang an das Parkhaus und jeder Fortschritt, den wir erzielt haben, brachte uns diesem Ziel näher. 

Angefangen haben wir mit einem einfachen Sketch, um einen Servo zu bewegen. Den Sketch haben wir uns aus dem Internet kopiert und mit der dazugehörigen Hardware aus dem Unterricht haben wir alles ausprobiert. Wenn dann alles so funktioniert hat, wie wir wollten und wir auch den Sketch verstanden hatten, ging es weiter. Nun haben wir uns mit einem Bewegungsmelder auseinandergestzt. Den einfachen Sketch haben wir kopiert, dann die Hardware zusammengebaut und ausprobiert. Sobald alles funktioniert hat und wir den Sketch verstanden hatten, haben wir diesen eigenständig mit dem Servosketch verbunden. Nachdem das funktioniert hat, konnten wir einen Servo durch Bewegung steuern. Dann haben wir uns mit Ultraschzallsensoren auseinandergesetzt. Einen ursprünglichen Sketch haben wir kopiert, die eine vereinfachte Hardware mit LEDs zur Kontrolle zusammengebaut und alles ausprobiert. Sobald alles funktioniert hat und wir den Sketch verstanden hatte, haben wir diesen Sketch eigenständig in den Bewegungsmelder-Servo-Sketch eingefügt. Nun konnten wir einen Servo durch Bewegung steuern, aber nur wenn nichts den Ultraschallsensor blockiert.

#### Quellen:

https://funduino.de/anleitung#1Vorwort_zur_Arduino_Anleitung

https://www.youtube.com/watch?v=G4ZlfsbDtQo

https://funduino.de/nr-12-servo-ansteuern

https://funduino.de/nr-8-bewegungsmelder

https://www.mymakerstuff.de/2016/05/24/arduino-tutorial-der-ultraschallsensor/



### <a name="5"></a>Unser Projekt

Wir haben nun also ein Parkhaus entwickelt, das auf Bewegung seine Schranke öffnet. Ist jedoch der Parkplatz besetzt, öffnet sich die Schranke nicht. Ob sie sich bei Bewegung öffnen wird oder nicht, erkennt man an einer rot bzw. grün leuchtenden LED.


### <a name="6"></a>Unsere Hardware

Hier sieht man unsere Hardware vor dem Einbau in das Parkhaus.

![Aufbau mit Nummern](https://github.com/dennis602/Projektseite/blob/master/Aufbau_fertig_nummern.PNG?raw=true)

#### Erläuterungen:

1. Mikrocontroller: Er ist das Herzstück von Arduino, da er Software mit Hardware verbindet. Auf ihn wird der Sketch geladen und an ihn angeschlossen sind alle externen Geräte. Siehe [Der Arduino](#2)

2. Breadboard: Es bildet eine Erweiterung für den Mikrocontroller, da es für uns die Möglicheit bietet alle anderen Geräte mit Strom zu versorgen, obwohl der Mikrocontroller nur einen 5V Anschluss hat. Dazu verbindet man einfach den 5V Anschluss mit der Plus-Leiste des Breadboards und die Minus-Leiste mit GND (Groundpin am Mikrocontroller). Anschließend konnten wir alle weiteren Geräte an diese beiden Leisten anschließen und mit Strom versorgen.

3. Verbindungskabel mit USB-Anschluss: Dieses verbindet den Mikrocontroller mit dem Computer und somit mit dem Arduino-Programm. Es ermöglicht also das Übertragen des Sketches. Außerdem wird über diesen Anschluss die Stromversorgung gewährleistet.

4. Servo: An dieser Stelle wird ein Servo angeschlossen (Servo ist noch nicht verfügbar). Der Servo öffnet und schließt die Schranke. Vom Servo gehen drei Kabel ab: Das rote Kabel geht an die Plus-Leiste vom Breadboard und versorgt so den Servo mit Strom. Das braune Kabel schließt den Stromkreis, indem es zur Minus-Leiste des Breadboards führt. Das gelbe Kabel sorgt für die Datenversorgung des Servos, indem es zu einem digitalen Pin am Mikrocontroller führt. So weiß der Servo, wann er die Schranke öffnen und schließen soll.

5. Bewegungssensor: Er registriert Bewegungen und sendet daraufhin ein Signal. In unserem Fall sendet er auf Bewegung ein Signal an den Servo, sich zu öffnen.



## Quellen
https://asset.conrad.com/media10/isa/160267/c1/-/de/616724_GB_00_FB/set-arduino-uno-platine-usb-2-0-anschlusskabel-steckplatine-616724.jpg

