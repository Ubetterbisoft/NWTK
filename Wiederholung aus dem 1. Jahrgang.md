# Wiederholung aus dem 1. Jahrgang

#### Fehlertolerant:

Fällt ein Device aus, muss der Datentransfer immer noch gewährleistet sein. Das kann durch redundante (mehrfach vorhandene) Verbindungen erreicht werden.



#### Skalierbarkeit

Kommen neue User oder ganze Netzwerke dazu, muss das ohne Änderung in der Grundstruktur möglich sein. 



#### Accesspoint

Er holt die Informationen vom Router und wirkt wie ein Wlan-Repeater oder Wlan Switch.



#### TCP / IP Modell

In der Praxis ist das TCP / IP Modell besser, in der Theorie hingegen das OSI Schichten Modell.

OSI Infos:

* Beim Session Layer werden Verbindungen mit einem Server hergestellt.

* Presentation Layer behandelt die Art wie Informationen dargestellt werden.

* Application Layer ist die fertige Anwendung

* Transport Layer transportiert die Informationen (TCP / UDP)



Auf Layer 4 sind Segmente und Daten

Auf Layer 3 sind Pakete

Auf Layer 2 sind Frames

Auf Layer 1 sind Bits

Bei Paritäts Bits geht es um die Synchronisation der Daten.

![1 YkbLfG73CiB4QviVTM6POg](https://user-images.githubusercontent.com/78872776/160997118-82c52c02-bcc1-464f-8549-4ed6f77fd2d1.png) 

| Layer 7 (Application)  | Mittels Anwendungssoftware werden Daten produziert           |
| ---------------------- | ------------------------------------------------------------ |
| Layer 6 (Presentation) | Die Formate der Daten wird festgelegt (ASCII, JPEG,...)      |
| Layer 5 (Session)      | Aufbau und Schließen von Sessions, Managen des Datenaustausches |
| Layer 4 (Transport)    | Gewährleistung der Kommunikation zwischen den Endgeräten; Segmentierung, Sequencing, Reassembling, allenfalls neu senden von Daten, Zuordnung der Daten zu Anwendungen |
| Layer 3 (Network)      | IP - Adressierung und Wegwahl der Pakete; logische Adressierung |
| Layer 2 (Data Link)    | MAC - Adressierung der Frames, Fehler-checking; physische Adressierung |
| Layer 1 (Physical)     | Festlegen Mechanischer, elektrischer und funktionaler Mittel für die bitweise Übertragung der Daten |

TCP und UDP haben nicht direkt etwas mit Portnummern zutun. Lediglich wird auf diesen Layern die Portnummer benötigt.

Layer 4 Transportiert Daten und zerteilt sie in Segmente. Die Daten kommen von der Anwendungs Schicht Layer 7.