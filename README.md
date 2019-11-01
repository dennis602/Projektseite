# Projektseite

## Inhaltsverzeichnis

[Vorwort](#1)

[Der Arduino](#2)

  [Der Sketch](#3)
  
[Projektentwicklung](#4)

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






## Quellen
https://asset.conrad.com/media10/isa/160267/c1/-/de/616724_GB_00_FB/set-arduino-uno-platine-usb-2-0-anschlusskabel-steckplatine-616724.jpg

