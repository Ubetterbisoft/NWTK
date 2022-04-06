# Ping

Mit dem dem Kommando **ping** wird der TCP/IP Protokollstack von Layer 1 bis Layer 3 getestet. Verwendet wird dabei das ICMP- Protokoll, das verschiedene Typen von Meldungen liefert. Echo Response Echo Reply

# Traceroute

Mit dem Kommando **traceroute** auf Cisco-Routern und Switches und mit dem Kommando **tracert** auf Microsoft-OS-PC'S kann der Weg der Pakete von der Quelle bis zum Ziel verfolgt werden. Die erste Nachricht geht immer an das Gateway. Danach zu anderen Routern wie dem ISP [...].

Jeder Router, den ein Paket passiert, liefert seine IP-Adresse samt Zeit Stempel an die Quelle zurück. Ein "*" bezeichnet die Nichterreichbarkeit.

# ARP

Das Address Resolution Protocol (**ARP**) ist ein Netzwerkprotokoll, das zu einer IP-Adresse (Netzwerkadresse) der  Internetschicht die MAC-Adresse(physische Adresse, Hardware-Adresse) der  Netzzugangsschicht ermittelt und diese Zuordnung gegebenenfalls in den **ARP**-Tabellen der beteiligten Rechner hinterlegt.

Dieses Protokoll ordnet der IPv4-Adresse die Mac-Adresse zu (mapping) und verwaltet den ARP-Cache. Die Einträge können statisch oder dynamisch sein. Statische einträge müssen händisch gemacht werden und bleiben immer im Cache, dynamische Einträge werden mit einem Zeitstempel versehen und bleiben nur für kurze Zeit (2minuten bei Microsoft OS) im Cache. Mit dem Kommando `arp -a`  kann dies kontrolliert werden.

Ist eine Ziel mach nicht bekannt, so erfolgt ein Broadcast auf Layer 2(FF-FF-FF-FF-FF-FF) ins lokale Netz. Befindet sich das Ziel nicht im lokalen Netz, so antwortet der Gateway (Routerinterface) mit seiner MAC (Proxy-ARP) und die Gateway-IP wird zusammen mit der Gateway-MAC in die lokale ARP-Tabelle eingetragen.

ist das Routerinterface nicht erreichbar, ist auch der Zielnode nicht erreichbar

# DHCP

Wenn ein Client die IP-Adressierung auf "automatisch beziehen" gestellt hat, versucht er von einem DHCP-Server eine IP-Adresse zu beziehen, die er dann für die Netzwerkverbindung für eine bestimmte Zeit (lease time) verwenden kann.

Der Client nimmt Kontakt mit einem DHCP Server auf und sendet eine Anfrage. Der Server nimmt eine Adresse aus seinem Adresspool(am Server eingestellt) und bietet sie dem Client an. Der Client nimmt die Adresse per Request an, der Server bestätigt die Annahme (Acknolegment).
