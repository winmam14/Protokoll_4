# Protokoll 4
## Thema: Überstzen von Programmen(MakeTool)
**Professor:** SX  
**Übungsdatum:** 4.12.2018  
**Author, KNr.:** Winter Matthias, 17  
**Anwesend:** Sarah Vezonik, Alois Vollmaier, Patrick Wegl, Mercedes Wesonig, Winter Matthias  
**Abwesend:** Winter Thomas    
  
  
---

## Stundenübersicht
#### 1. MakeTool
##### 1.1 Grundlagen
##### 1.2 Makefile
#### 3. Übung
#### 4. Probleme und Lösungen

--- 

## 1. MakeTool  
Das MakeTool ist ein Tool welches bei der Übersetzung verschiedener Teilprogramm zu einem fertigen ausführbaren Programm hilft.  
Das MakeTool weis auch automatisch welche Datei neu kompiliert werden muss. Dies geschiet mit Hilfe von Zeitstempel die das System der Datei verleit.
### 1.1 Grundlagen  
Grundlägend muss man, um das MakeTool anwenden und verstehen zu können, wissen wie ein Programm aufgebaut ist und zusammen gebaut wird.
Wichtig ist, dass im 1.Schritt der Quelltext als ".c"-Datei Gespeichert wird. Danach wird der Quelltext mit dem Compiler kompiliert und zum Schluss mit dem Linker zusamen gebaut. Heraus kommt eine ausführbare Datei mit der Extention ".elf". Das fertige Programm kann auch  aus mehreren Objektdateien zusammen gelinkt werden. Das hat die Vorteile der Wiederverwendbarkeit, der besseren Übersicht und damit es Recourcen sparender ist. Zur Übersicht der einzelnen Schritte siehe das nachfolgende Bild.  
![alt text](http://new.c-howto.de/wp-content/uploads/2017/04/Makefiles.gif)     

### 1.2 Makefile
Das MakeTool benötigt ein Makefile, welches auch mit dem Namen "Makefile" gespeichert werden muss! Es wird mit einem Texteditor geschrieben und in diesem Makefile müssen dann die Informationen für das MakeTool stehen. Die Informationen setzen sich aus Ziele(targets), Abhängigkeiten(dependencies) und Befehle(commands).  
Das Prinziep eines Makefiles sieht so aus:  /  Hier noch ein Beispiel aus der Übung:
```
Ziel x: Abhängigkeiten             |             main.o: main.c monitor.h lcd.h
*tabulator* Befehl 1               |                     gcc -c main.c
*tabulator* Befehl 2               |
*tabulator* Befehl 3               |
                                   |
Ziel y: Abhängigkeiten             |             clean: 
*tabulator* Befehl 3               |                   rm *.o
*tabulator* Befehl 3               |                   rm *.elf
*tabulator* Befehl 3               |
``` 

### 2.Übung  

### 3.Probleme und Lösungen
Zeitstempel

