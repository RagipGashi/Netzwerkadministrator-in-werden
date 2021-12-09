# Netzwerkadministrator-in-werden


# About

## Wie sind Netzwerke aufgebaut? Wie funktioniert die Datenübertragung? Was macht die IP-Adresse genau? Solche und viele weitere Fragen werden in diesem Training beantwortet. Dieses Training basiert auf den Grundlagen der Netzwerktechnik und zeigt anhand vieler Beispiele, wie Netzwerke aufgebaut sind und wie sie in der Praxis funktionieren.
---


# 1. Netzwerke: Eine Einführung

## Was sind Rechnernetze?
- Rechnernetze haben letztlich die Aufgabe Daten zu übertragen oder ewas abstrakter **Rechnernetze übertragen Informationen**


### Welche Komponenten gehören genau zu einem Netzwerk?
- Abstrakt betrachtet, besteht ein Netzwerk aus folgenen Komponenten:
  - Information (Die Information ist definitif unser höchstes Gut).
  - Sender (Das ist die Komponente, die die Information versenden möchte).
  - Empfänger (Ein oder mehrere Empfänger an die die Inormationen übertragen werden soll).
  - Und wir benötigen natürlich ein **Medium** über das die Information letzten Endes dann übertragen werden soll.
    - Das Medium muss nicht zwingend ein Kabel sein. Wir können aud mit Funk übertragen, das Medium Luft verwenden. Wir können Kupfer Kabel verwenden, oder Glasfaserkabel. Das alles wird unter dem Begriff **Medium** zusammengefasst.

- Unsere Aufgabe ist alles beretis einwandfrei funktionieren.
![IT Aufgabe](https://user-images.githubusercontent.com/44840806/139865863-26080897-ee09-48ed-b099-428cfc3fa601.png)


### Was sind die Netzwerktopologien?

- Eine Netzwerktopologie beschreibt den Aufbau und die Struktur eines Netzwerkes. 

- Netzwerktopologie ist unterteilt in:
  - Logische
  - Physische (meist die physische betrachtet wird).

- **Punk zu Punk** Topologie: zwei Geräte, die direkt miteinander verbunden sind (z.B. Cross-Kabel oder ein Ad-Hoc-Netzwerk).
![Punkt zu Punkt](https://user-images.githubusercontent.com/44840806/139869667-1349c6e1-98d9-4930-8847-e428436868cf.png)

- **Bus** Topologie. Alle Geräte an einer Linie verbunden. Diese muss an den enden mit einem Widerstand terminiert werden.
![Bus](https://user-images.githubusercontent.com/44840806/139869781-c824b141-3c34-4fee-b83e-dc6beab19243.png)

- **Ring** Topologie. Bei der Ring-Topologie, wirkt jedes Gerät als Verstärker und kann die vollle Bandbreite benutzen. Vorteil: hohe Ausfallsicherheit.
![Ring](https://user-images.githubusercontent.com/44840806/139870018-7f8f62a0-4c02-4e14-a181-f4f9dbada754.png)

- **Stern** Topologie. Die meinst verwendete Topologit. In der Mitte befindet sich ein Verteiler, an dem jedes Gerät einzeln angeschlossen ist. Mehr verkabelung aber ein Ausfall eines Geräts keinen Auswirking an den anderen hat.
![Stern](https://user-images.githubusercontent.com/44840806/139870100-5800d0f6-c293-49b9-890a-0d7a4510ecaf.png)
 
- **Vermaschte** Topologie. Hier sind alle Geräte miteinander in verschiedenen Wege verbunden. Die Ausfallsicherheit wesentlich erhöht. 
  - **Vollvermaschte** Topologie. Jedes Geräte mit jedem verbunden ist. Verkabelung Aufwand ist erhöht. 
![Vermascht](https://user-images.githubusercontent.com/44840806/139870214-828e409c-d2bf-4c22-baa7-e32c2be02ab8.png)
![Vollvermascht](https://user-images.githubusercontent.com/44840806/139870279-7193e1a1-f9c2-449e-8b0a-fd5d49712dbc.png)


- Es gibt auch die Kombinationen von Topologien:
  - Baum (Stern - Stern)
  - Ring - Stern
  - Vermascht - Stern
  ...


### Netzwerkausdehnung

- **BAN - Body Area Network**
  - Direkt am Körper
  - Medizinische Geräte, wie Pulsmesser, etc.
  - Auch schnurlos: WBAN.
  
- **PAN - Personal Area Network**
  - Headsets, Freisprecheinrichtung, etc. 
  - Auch schnurlos: WPAN
  - WPAN meist mit Bluetooth.
  
- **LAN - Local Area Network**
  - Privates Netz zuhause
  - Kleines Firmennetz
  - Allgemein ein lokal begrenztes Netz, meistens in einem Gebäude
  - Auch schnurlos: WLAN. 
  
- **CAN - City/Campus Area Network**
  - Vernetzung mehrerer LANs einer Stadt/Uni
  
- **MAN - Metropoitan Area Network**
  - z.B. Vernetzung von Telekommunikationsanbietern innerhalb einer Metropole
  - Auch schnurlos: WMAN
  
- **WAN - Wide Area Network**
  - Erstreckt sich über ein Land/Länder oder Kontinente
  - Auch schnurlos: WWAN (sehr bekannte über LTE)
  
- **GAN - Global Area Network**
  - Ein weltumspannendes Netzwerk
  - Internet ist ein GAN
  - Weltumspannendes Netzwerk einer Firma.   


## 1.1 Übertragungsarten

### Duplex
- Es ist eine Methode, wie Sie mit anderen kommunizieren können.
- Gibt es drei Varianten:
  - **Simplex** -> Datenübertragung nur in eine Richtung möglich. Beispiel: Radio oder TOSLINK.
  - **Halb-Duplex** -> Abwechseld in beide Richtungen. *Nicht gleichzeitig*, sonst Kollisionen entstehen.
  - **Voll-Duplex** -> In Beide Richtungen gleichzeitig übertragen. Bestes Verfahren für Geschwindigkeit. (Beispiel: Telefon).


## Verschiedene Übertragungsszenarien

- In der Netzwerkkomunikation existieren unterschiedliche Übertragungsszenarien zur Verfügung.
- Die beziehen sich darauf, wie Kommunikationskanäle zwischen Sender und Empfänger aufgebaut werden.

- **Unicast** -> Eins zu Eins Verbindung: Ein Sender baut einen exklusiven Kommunikationskanal zu einem Empfänger auf.

![Unicast](https://user-images.githubusercontent.com/44840806/140041789-5da0b8cc-0359-40d5-a9c1-124e9cf86e7b.png)


- **Broacscast** -> Eins zu Alle Verbindung: Mit einem Sender alle Empfänger im Netzwerk zu erreichen.

![Broadcast](https://user-images.githubusercontent.com/44840806/140042344-f2adce25-2747-46bf-924e-b148920bcc7a.png)


- **Multicast** -> Eins zu Einige Verbindung: Mit einem Sender nicht alle Empfänger adressieren, sondern ein ganz bestimmten Host adressieren möchte, ein ganz bestimmten Empfänger. Die jenigen, die mitmachen wollen.

![Multicast](https://user-images.githubusercontent.com/44840806/140043352-b490c5ef-abca-4c52-9578-0fd12e95dc13.png)


- **Anycast** -> Ist ein Spezialfall einer Verbindung, eine Eins-zu-Nächstgelegenden Ziel Verbindung.
  - Wir haben nich nur ein Zeil-IP sondern zwei Ziel-IPs die sind auch noch identisch. Das was bei **Unicasting** verboten ist, wiel IP Konflikt ist, das ist bei **Anycasting** Programm.

![Anycast](https://user-images.githubusercontent.com/44840806/140050510-b7e0ee3f-855b-4d1c-b524-d5abf8c94df7.png)


## 1.2. Kommunikation visualisieren

### Schichtenmodell
- Um den gesamten Kummunikationsfluss zu visualisieren, benutzen wir ganz unterschiedliche Modelle - **Schichtenmodell**.

- **Warum Schichtenmodelle?**
  - Abstaktion der Kommunikation (vereinfahend der Kommunikation)
  - Ablauf visualisieren
  - Fachsprache (das macht leichter die Fehlersuche oder Fehlerbehebung).


### Schchtenarchitekturen
- OSI-Modell
- DoD / TCP/IP-Modell
- Betriebssystem-Modell


## Das OSI-Modell

### Der Aufbau des OSI-Modells

1. **Bitübertragungsschicht / Physical Layer
	- Reine Signalübertragung
	- Elektrische Signale, Licht, Wellen
	- Kabel, Stecker, Spannung
	- Repeater, Hub


2. **Sicherungsschicht / Data Link Layer**
    - Zugriff auf das Medium
    - Adressierung auf Hardwareebene (MAC-Adresse)
	- Flusskontrolle
	- Layer 2 Switch


3. **Vermittlungsschicht / Network Layer**
	- Logische Adressierung
	- Wegewahl
	- Router / Layer 3 Switch

4. **Transportschicht / Transport Layer**
	- Zugriff auf anwendungsorientierte Schichten
	- Verbingungsorientierung
	- Paketfilter

5. **Sitzungsschicht / Saisson Layer**
	- Aufbau, Aufrechterhaltung und Abbau von Sitzungen
	- Remote Procedure Call (RPC)
	- ![RPC-OSI-Modell](https://user-images.githubusercontent.com/44840806/140494981-1d0d9305-8342-409a-8c77-f8264cffad7f.png)

6. **Darstellungsschicht / Presantation Layer**
	- Unabhängige Darstellung von Daten (System unabhängige Datenübertragung. Von einem System zu anderen, die Daten ohne Informationsverlust übertragen werden können. z.B. eine System kann nur ANSII, das andere kann nur ASCII, in diesem Fall benötigen wir in der Mitte ein Format, das beide Kommunikationspartner lesen können).
	- Abstract Syntax Notation One (ASN.1)
	- ![ASN.1-OSI-Modell](https://user-images.githubusercontent.com/44840806/140496114-614d5587-0f83-49cf-81a8-0b5cf39d7991.png)

7. **Anwendungsschicht / Application Layer**
	- Anwendutsprotokolle (Hier handelt es sich um die Protokolle, die Anwendung selber liegt nicht in Schicht 7, sondern sie nutzt nur ein Protokoll auf Schicht 7, um mit einer andreren Anwendung zu kommunizieren).
	- ![HTTPS-OSI-Modell](https://user-images.githubusercontent.com/44840806/140496671-9c8ba952-c3ab-4f5b-9070-644514f58979.png)


# 2. Physischer Weg durchs Netz

## Strukturierte Verkabelung

### Primäre Verkabelung
  - Verkabelung zwischen Gebäuden/Hallen
  - Glasfaser: weite Strecken und galvanische Trennung. (Es kann kein Austausch von Strom mehr erfolgen, somit ist auch kein Potentialasgleich über das Netzwerk möglisch).
	
![Strukturierte Verkabelung-Primäre Verkabelung](https://user-images.githubusercontent.com/44840806/140767195-fe313172-7d54-4073-8baa-b00b8b847863.png)


### Sekundäre Verkabelung
  - Vertikale Verkabelung
  - Nach DIN nur Glasfaser; in der Praxis auch Kupfer
  
  ![Sekundäre Verkabelung](https://user-images.githubusercontent.com/44840806/140942146-6084ffba-4ed3-4aa8-98b8-b091edeb7a0b.png)
 

### Tertiäre Verkabelung
  - Horizontale Verkabelung
  - In der Regel Kupfer; in der Praxis manschmal auch Glasfaser
  
  ![Tertiäre Verkabelung](https://user-images.githubusercontent.com/44840806/140943008-e284f897-f519-400b-9cd0-782318d1c4a7.png)


## Verschiedene Kabelarten

### Kabel
  - Verlegtekabel - werden zu festen Verkabelung zwischen den Patch-Panels genutz
  - Patchkabel - den PC anzuschließen oder den Anschluß am Switch mit dem Patch-Panel zu patchen. 
  

### Twisted Pair
  - CAT1-4:	kaum mehr anzutreffen, eher Telefon
  - CAT5:	100MBit/s
  - CAT5e:	100MBit/s - 1GB/s 
  - CAT6:	1GB/s
  - CAT7:	10GB/s 

### Es gibt auch noch wietere Bezeichnungen für diese Kabel:
  - UTP: 	Unshielded Twisted Pair - keine Abschirmung
  - FTP:	Foiled TP - Adernpaar mit Alufolie geschirmt
  - STP:	Shielded TP - Adenpaar mit Kupfergeflecht geschirmt
  - S/UTP:	Screned UTP - Ader ungeschirmt, Kabel geschirmt
  - S/STP:	Screned STP - Adernpaar geschirmt, Kabel geschirmt
  
### Kabelstecker:
  - Bis CAT6: RJ45 (Western-/Ethernet-Stecker), 8P8C-Stecker
  - CAT7: GG45-Stecker
  - Reichweite 100m von aktivem zu aktivem Gerät
  
  ![Aktivem zu aktivem Gerät](https://user-images.githubusercontent.com/44840806/140952652-a2162cea-7179-461c-a36f-57dc417e9173.png)
  
  
### LWL - Lichtwellenleiter (Glasfaser)
  - Multi-Mode (Reichweite von circa 300 bis 500 Metern)
  
  ![Multi-Mode LWL](https://user-images.githubusercontent.com/44840806/140953369-c95cc8a6-bbeb-4895-9f16-30964500898b.png)

  - Mono-Mode (Reichweite über mehreren Kilimetern)
  
  ![Mono-Mode LWL](https://user-images.githubusercontent.com/44840806/140953796-04a0d3eb-d2e5-4788-be09-e84290f8b38f.png)
  
 
### LWL Kabeltypen und Stecker
  - OM1 und OM2: Standard für bis 1GBit/s
  - OM3 und OM4: für höhere Geschwindigkeiten wie 10GBit/s 
  
  - **Stecker:**
  - **LC-Stecker** den man meisten an dem Gerät, wie z.B. dem Server finden werden:
  
  ![LC-Stecker](https://user-images.githubusercontent.com/44840806/140954875-738d8e0e-b4c8-432f-bc36-7f05583e2c0d.png)
  
  - **SC-Stecker** den man am meisten an Patch-Panel findet.
  
  ![SC-Stecker](https://user-images.githubusercontent.com/44840806/140955196-6355545b-ff33-4624-a7ff-3621b972226a.png)



## Drahtlose Übertragung

  - Bluetoth (IEEE 802.15.1)
  - WLAN (IEEE 802.11)
  - Wi-Fi
  - LTE


### Bluetoth
  - Reichweite in der Regel mehrere Meter
  - Reichweite je nach Technik bis zu 100 Meter
  - Nutzung hauptsächlich für Mobilgeräte

### WLAN
  - 2,4 GHz
    - Weit verbreitet, Kanalüberlappung, Frequenz teilen mit Bluetoth, Mikrowellen, Babyphones, ...
  - 5 GHz
    - Klare Kanaltrennung, wenig Geräte (Es gibt täglich mehr Geräte, die 5 GHz unterstützen).

### WLAN - 2,4 GHz
  - 11 verfügbare Kanäle, in Europa bis 13, in Japan bis 14 Kanäle.
  - 802.11	2MBit/s
  - 802.11b	11MBit/s
  - 802.11g	54Mbit/s
  - 802.11n	~300Mbit/s

  ![2.4GHz WLAN](https://user-images.githubusercontent.com/44840806/140958609-c4aab2ee-e1fe-4ada-959b-4e0bffa74070.png)


### WLAN - 5 GHz
  - Je nach Land bis zu 26 Kanäle
  - 802.11a	54Mbit/s
  - 802.11h	54-108MBit/s
  - 802.11n	600MBit/s

  ![5Ghz WLAN](https://user-images.githubusercontent.com/44840806/140959182-be8157bc-3ac0-46b8-b0e5-c71edb69e651.png)


### WLAN - Reichweite
  - Reichweite i.d.R. 30-100m auf freie Fläche, mit sep. antenne bis 300m.
  - Besonderheit Richtfunk, bis zu mehreren Kilomenter
  - Einschränkung hauptsächlich durch:
    - Wasser (z.B. Nasse Außernwände an einem Haus oder das Badezimmer).
	- Metall (z.B. besonders Stahlbeton oder Schnellbauwände schränken die Reichweite sehr stark ein).


### WLAN - Verschlüsselung
  - **WEP**
    - Unsicher, veraltet
  - **WPA**
    - Basiert auf WEP, gitlt wieterstgehend als unsicher
  - **WPA2**
    - Heutiger Standard. Es arbeitet mit dem Verschlüsselungsmechanismus AES (Advanced Encryption Standar).
	- Bis jetzt noch nicht geknackt. Trotzdem, empfohlen ist ein langes Passwort zu benutzen.
  - Alternative, **VPN** über **WLAN** zu machen, mit z.B. IPSEC oder SSL.


### Wi-Fi
  - Oft synonym zu **WLAN** verwendet.
  - Eigentlich nur ein Markenname.
  - Geräte, die Standard der "Wi-Fi Alliance" entsprechen. **WLAN** ist die Technik, und **Wi-Fi** ein gewisser Standard.


### LTE - Lont Term Evolution
  - Bis zu 300 Mbit/s
  - 4G-Standard erst ab LTE-Advanced
  - 4G bis zu 1Gbit/s


### Weitere
  - WiMAX/WiMAX2 bis zu 1GBit/s
  - HSPA+ bis zu 42MBit/s
  - HSDPA bis zu 7MBit/s Down/ HSUPA bis zu 6MBit/s -> HSPA
  - UMTS bis zu 384kBit/s
  - EDGE bis zu 220kBit/s
  - GPRS bis zu 53kBit/s



## Netzwerke mit einem Hub/Repeater verbinden

- Die Unterschied zwischen einem Hub und einem Repeater:
  - Ein **Repeater** hat in der Regel zwei Anschlüsse und wird genutzt, um eine Leitung zu verlängern. 
  - Ein **Hub** hat mehrere Anschlüsse. 

- **Details**
  - Die arbeiten auf ISO7OSI Schicht 1
  - **ALLE** Daten werden an **ALLE** Teilnehmer weitergeleitet
  - Somit keine Begrenzung der Broadcastdomäne. (Beduetet, dass ein Broadcast-Packet, z.B. auf der Suche nach DHCP-Server, begrenzt wird. **HIER DEFINITIV NICHT**.
  
  
### Hub/Repeater

- Vorteile:
  - Günstig
  - Einfach
  
- Nachteile:
  - Hoche Netzlast
  - Mithören (sniffen) möglich.


# 3. Daten strukturiert übertragen


## Paketbildung / Framing

- Eine Kommunikation durchläuft ihren Weg durch die Schichten, und bekommt diverse Steuerungsinformationen angefügt.
- Die Steuerungsinformationen nennen wir **Header** und **Trailer**.
- Die Desamtheit aus **Header** und **Trailer** ohne Nutzdaten, das nennt man **Overhead**.


## Ethernet-Frame

- Wenn wir in einem kabelgebundenen Netzwerk arbeiten, wir haben mit einem **Ethernet-System** zu tun. 
- Ein **Ethernet-Frame** ist das letzt Paket, das gebildet wird, bevor es dann letzten Endes als reiner Bitdatenstrom aufs Kabel geht. 


## Aufbau:

![Ethernet-Frame](https://user-images.githubusercontent.com/44840806/143895218-824b8370-d736-4a2b-ad4d-5cc34ba1fb9e.png)

- Quell-MAC-Adresse, die MAC-Adresse, die Hardware-Adresse, mit der wir Systeme auf der Schicht 2, auf der Sicherungsschicht ansprechen können, 
  - Das besteht auf zwei Teilen, einmal die Quell-MAC und einmal die Ziel-MAC, 
- Danach ist ein Typenfeld, das beschreibt das nächsthöhere Protokoll,
- Dann sind die Daten, beziehungsweise nicht die Nutzdaten, sondern die Daten, die hier eingefasst sind, da stecken auch schon die Header von den höheren Schichten mit drin, 
- Zum Schluss ist eine Prüfsumme, der **Cyclic Redundancy Check**, mit der ein Empfänger prüfen kann, ob das Paket auch wirklich korrekt versendet wird.


### Die MAC-Adresse

![Mac-Adrese in CMD](https://user-images.githubusercontent.com/44840806/143896479-ebf56f17-8736-44d1-8589-a8fe10f0106c.png)

- **MAC-Adresse** steht für **Media Access Control**, und das ist die Hardware-Adresse von einem Netzwerk-Interface.
- Liegt auf der **Sicherungsschicht**.
- **MAC-Adresse** ist 6 Byte lang, also 48 Bit, und die wird direkt von den Hardware- oder Netzwerk-Interface-Herstellern vergeben.


### Aufbau:

![MAC-Aufbau](https://user-images.githubusercontent.com/44840806/143900094-1ccf050b-5c33-4952-8818-24c7e786cf29.png)

- Die **MAC-Adresse** besteht auf zwei Teilen:
  - **OUI (Organisationally Unique Identifier)** - 3 Byte -> Herstellernummer, die von **IEEE** an die einzelnen Hersteller vergeben wird.
  - Die nächste 24 Bits, die können dann die Hersteller in ihrer Organistaion vergeben. 
  -*Es gibt auch noch einen kleineren Adressblock für kleinere Organisationen und für Privatpersonen. Das ist der Individal Address Block, und der umfasst dann 4096 individuelle Adressen*.

  
### Das Typenfeld

- Kennzeichnet das Protokoll der nächsthöheren Schicht
- 0x0800 IP4
- 0x0806 ARP
- 0x0809b AppleTalk  


### Das Datenfeld

- Hier kan ein Ethernet-Paket insgesamt max **1518 Byte** lang sein.
- **Header**, also **Quell-MAC** plus **Ziel-MAC** plus **Typenfeld** und die **CRC Prüfsumme** insgesamt 18 Bit wegfallen, beträgt die Nutzlast, die so ein Paket, ein Ethernet-Frame aufnehmen kann, **Max 1500 Byte**.
- Die Nutzlast, wird als **MTU** oder **Maximum Transmission**


### Maximum Transmission Unit

![MTU](https://user-images.githubusercontent.com/44840806/144588993-c1373b54-aca5-436f-8bf0-9d33c9fcde00.png)

- Wenn der Ethernet-Header erweitert wird, schrumpft dann diese MTU, weil er kann eben nicht mehr aufnehmen als diese 1518 Byte. 
- Das passiert z.B. bei Point to Point over Ethernet (PPPoE).


### Padding Feld 

![Padding Feld](https://user-images.githubusercontent.com/44840806/144605303-db8e1804-88df-43ba-ba0b-8541db82947b.png)

- Wenn wir jetzt diesen Ethernet-Frame betrachten, und wir haben in dem Beispiel hier eine reine Datenmenge von 10 Byte, dann können wir das ja jetzt mal zusammenrechnen: 
  - Also, die Quell-MAC hat 6 Byte, plus TMAC nochmal 6 Byte, und das Typenfeld plus die 10 Byte Daten, da sind wir dann bei 24 Byte, plus die Prüfsumme, da sind wir dann bei 28 Byte, 
  - Jetzt haben wir das Problem, 28 Byte, die reichen nicht aus, die sind zu groß für einen Ethernet-Frame, und deswegen gibt es ein sogenanntes **Padding-Feld**.
  - Dieses Padding-Feld, damit werden dann die Ethernet-Frames einfach so lange aufgefüllt, bis mindestens 64 Byte erreicht sind, und somit hat dann der Ethernet-Frame auch seine Minimalgröße. 
  - Wenn das Ethernet-Paket soweit fertig ist, dann kann's auch schon losgehen auf das Medium.


### MAC-Adresse auffinden

- Wir haben hier also das Address Resolution Protocol, mit Hilfe des ARP-Protokolls ordnen wir MAC-Adressen IP-Adressen zu.
- Der Ablauf gliedert sich in zwei Teile: 
  - dem **ARP-Request**, wo ich nach der MAC-Adresse frage, und 
  - im besten Fall der **ARP-Reply** mit der korrekten MAC-Adresse das MAC-IP-Adress-Pärchen, wird dynamisch in einem lokalen Cache abgespeichert, und auch dynamisch wieder herausgelöscht,
- **WICHTIG** So lange das Pärchen in diesem Cache drinsteht, muss kein neuer ARP-Request erfolgen.
- Der Ping hätte nicht funktioniert, wenn nicht im Vorfeld das ARP-Protokoll gute Dienste und erfolgreiche Dienste geleistet hätte.


### Netzwerke mit einem Switch/Bridge verbinden

- Der Switch arbeitet auf **ISO/OSI Schicht 2** Model, und kann somit die MAC-Adresse auslesen. 
- Mithilfe dieser MAC-Adresse erstellt sich der Switch eine Tabelle, an welchem Anschluss welche MAC-Adresse angeschlossen ist, und besitzt damit die Möglichkeit, die Daten nicht mehr an alle, sondern gezielt an einen Empfänger zu senden.
- Er begrenzt keine Broadcast-Domäne, aber dafür die Kollisionsdomäne.


### Switch-Sat

- Source Address Table (SAT).
  - Beinhaltet die MAC-Adresse und den dazugehörigen Anschluss. Versendet nun jemand ein Datenpaket, empfängt der Switch dieses und speichert sich die Absender-MAC-Adresse in der SAT zusammen mit dem Anschluss. 
- Speichern der Absender-MAC beim Empfangen eines Pakets.
- Broadcast-Adressen werden nicht gespeichert
- Multicast-Adressen werden nicht gespeichert/ nur an Ziel-MAC's 


### Switch-Modus

- **Cat-through**
  - Weiterleiten des Pakets nach dem Empfang der Ziel-Adresse.
    - Sehr schnell, allerdings kann hier keine Fehlerüberprüfung mehr erfolgen und somit könnten defekte Pakete weitergeleitet werden.  
- **Fragment-Free**
  - Hier wird das Paket einfach auf einen konsistenten Paket-Header überprüft und erst dann weitergeleitet.  
- **Store-and-Forward**
  - Hier wird erst das komplette Datenpaket empfangen, die Prüfsumme kontrolliert und dann erst anhand der MAC-Adresse weitergeleitet. 
    - Sehr sichere, aber auch sehr langsame Methode.
  
- **Adaptive**
  - Beim moderneren, aber nicht von jedem Switch unterstützten Adaptive-Modus, wird als Standard "Cut-Through" verwendet. Und bei erkannten Fehlern heruntergeschaltet bis zum "Store-and-Forward-Modus".


### Switch-STP (Spanning Tree Protocol)

- Vermeiden von Schleifen
  - Schleifen sind deshalb schlimm, weil z. B. ein Broadcast-Paket an alle gesendet wird. Passiert das auf allen Geräten in einer Schleife, wird man also zugemüllt mit diesem Broadcast-Paket und überlastet somit das Netzwerk.
- Anschluss blockieren, prüfen, freigeben
  - Nach einem gewissen Time-out wird der Anschluss freigegeben. Das kann natürlich teilweise zu Problemen führen. da dieser Zeitraum unter Umständen sehr lange dauert.
- Portfast
  - Es wird direkt der Anschluss freigeschaltet, und erst im Nachhinein überprüft, ob eine Schleife entstehen könnte.
  - Diesen Modus sollte man aber nur an Anschlüssen verwenden, an denen definitiv nur ein Gerät angeschlossen wird.
- RSTP(Rapid Spanning Tree Protocol), MSTP(Multiple Spanning Tree Protocol).
  - Die entscheidende Verbesserungen bezüglich Geschwindigkeit und VLANs mit sich bringen.
  
### Switch-Stacking

- Stackkabel
  - Extra Switches benötigt, die dies explizit unterstützen. 
  - Da es hierfür meist einen speziellen Anschluss und ein spezielles Stack-Kabel gibt, das die Daten- und Managementinformationen mit Highspeed überträgt.
- Logische Einheit
  - Dazu müssen die Switches in der Regel vom gleichen Hersteller und der gleichen Produktreihe kommen.
- Performanter und besser verwaltbar als Uplink.
  - Es ist wesentlich performanter und besser verwaltbar, als ein normaler Uplink zwischen zwei Switches.
- Mal ganz davon abgesehen, dass der Uplink mir weitere Anschlüsse blockieren würde. 
- Ein Stack ist also ideal, um die Anzahl der Anschlüsse zu erweitern und eine gewisse Auswahlsicherheit herzustellen. 



# 3.1. Zugriffsverfahren auf das Medium


## CSMA/CD: Definition

- **C**arrier **S**ense: Abhören der Leitung
  1. Zunächst hört ein senderwilliger Client die Leitung ab.
  2. Falls die Leitung frei ist, darf er senden.
  3. Wenn nicht, dann muss er sich zurückhalten, und wartet eine bestimmte Zeit ab, bis er es wieder probiert. Im besten Fall, bekommt er dann sein Datenpaket abgesetzt, und die Übertragung war erfolgreich.
- **M**ulticast **A**ccess: potenziell gleichteitiger Zugriffsverfahren.
  - Multiple Access, das heißt, während der eine Client sendet, oder der eine Client gerade ein leeres Medium entdeckt und anfängt zu senden, dann kann es natürlich einem anderen Client ganz genauso gehen.
  - Beide können gleichzeitig auf das Medium zugreifen. In diesem Fall muss es einen Mechanismus geben, der die Kollision, die dann eben auftritt, erkennt(Collision Detection).
- **C**ollision **D**detection: Erkennen einer Überlagerung.
  - Erkennen einer Kollision, beziehungsweise das Erkennen einer Überlagerung auf dem Strang.

- **Backoff Time** - Zeit nach der Kollision. Alle PCs warten einige Zeit nach der Kollision, bevor sie nochmal mit dem Datenübertragung anfangen.


## CSMA/CA: Definition.
- Im Vergleich zu CSMA/CD geht es bei CSMA/CA nicht um die Kollisionserkennung, sondern um die Kollisionsvermeidung.

- CS: **C**arrier **S**ense.
  - Eine sendewillige Station muss zunächst am Medium lauschen, wenn das Medium frei ist, dann darf sie senden, wenn das Medium belegt ist, muss die Station warten, und es dann später noch einmal probieren.
- MA: **M**ultiple **A**ccess.
  - Auch beim CSMA/CA können Kollisionen nicht vollständig vermieden werden, man kann die Wahrscheinlichkeit nur minimieren, deswegen ist prinzipiell auch bei CSMA/CA ein Multiple Access, also ein gleichzeitiger Zugriff, möglich.
- CA: **C**ollision **A**voidance.
  -  Zunächst hört die Station das Medium, also inm Fall vom WLAN, die Luft, ab, und das Medium muss für den Zeitraum eines **DIFS** zunächst frei sein, dann interpretiert der Sender das als frei.
    - DIFS (Distributed Coordination Function Interframe Spacing). Entspricht praktisch der Zeitspanne, der vordefinierten Zeitspanne, die der Sender warten muss.
  1. Dann kommt nochmal eine Zeit obendrauf, eine Zufallszeit, das ist die Backoff-Zeit, und nach diesem Gesamtzeitraum darf die Station dann senden.
  2. Sollte das Medium belegt sein - die Station zunächst warten, bevor sie einen neuen Versuch startet, und zwar gibt es auch hier wieder diverse Zeiträume, die gewartet werden muss, da haben wir zunächst den Network Allocation Vector.
    - Network Allocation Vector - eine Tabelle, pflegt jeder Client für sich selbst - in MAC-Layer Frame von einem Wireless-Packet gibt einen kleinen Abschnitt (Duration).
	- In Duration steht drin, wie lange ich jetzt ungefähr das Medium beanspruche.
	- Andere Clients mitbekommen, die pflegen also aus dieser Information ihren eigenen NAV. Die warten dann bis das Medium frei ist.
  - Dan haben wir:
    - Backoff-Time -> DIFS (nochmal Zufallszeitraum)-> dann kann ich nochmal versuchen, das Medium abzuhören.
	- Das Medium ist jeztz frei, und wir können unsere Daten los senden.
  - Was passiert jetzt?
    - Daten werden direkt in einem Rutsch zum Empfänger geschickt.
	- Empfänger wartet den Zeitraum eines SIFS (Short Interframe Spacing),
	- Nachdem SIFS, Empfänger schickt ein Acknowladge-Paket zurück. (Der Sender weißt jetzt, dass ein Paket im Vorfeld angekommen ist).
  - Ein zusätzlicher Sicherheitsmechanismus in CSMA/CA ist folgender:
    - Ein Sender beziehungsweise der Empfänger nutzen die Ready-to-Send beziehungsweise Clear-to-Send Möglichkeiten.
	- Der Empfänger im Vorfeld bekommt ein Ready-to-Send -> er schickt ein Clear-to-Send zurück wenn das Medim frei ist.
	- **Dieses Ready-to-Send und Clear-to-Send System bekommen natürlich auch alle anderen Stationen in der Umgebung mit, ja, und die wissen dann eben, dass sie jetzt in diesem Zeitraum nicht mehr versuchen müssen zu senden.**



## Token Passing: Ablauf

- Ein Freitoken kreist im Netz:

![Token-Frei](https://user-images.githubusercontent.com/44840806/145174614-c2772445-d15f-42e0-b6a6-69ad08f8e97c.png)

- Sendewillige Station hängt Daten an:

![Token-Belegt](https://user-images.githubusercontent.com/44840806/145174865-e7f728ea-808d-4c24-a195-6f3d72b7b618.png)

- Empfangsstation kopiert die Daten:

![Token-Empfangen](https://user-images.githubusercontent.com/44840806/145175075-d4b24d4b-b289-471f-9392-5fb8263d0b32.png)

- Sendestation wandelt den Token wieder um:

![Token-Wieder Frei](https://user-images.githubusercontent.com/44840806/145175167-ad99f4e6-e05c-4e5c-a76f-07710920979f.png)



# 4. Vergabe der IP-Adressen


## Layer-3-Switch

- Switch, der auf Schicht 3 arbeitet, also der Schicht des Routers.
- Wird benötigt, um verschiedene IP-Netzwerke zu verbinden.
- Laut ISO/OSI kennt er max. die IP.Adressse.
- In der Praxis auch TCP/UDP-Ports der höheren Schichten.

### Layer-3-Switch oder Router?

| L3 Switch   | Router |
| ----------- | ----------- |
| Schneller | Mehr Funktionen |
| Günstiger | Weniger Ports |
| Eher Backbone | Eher Standortverbindungen |

- Somit gehört der Layer 3 Switch i.d.R. eher in das Backbone-Netz, um die verschiedenen VLANS und Netze performant zu verbinden. 
- Den Router würde eher benutzen, um Standorte zu verbinden oder für den Weg ins Internet.


## VLAN

### Netzwerk

- Alle Clients in einem Netzwerk.
- Hohe Broadcast.
- Keine Beschränkungen.


### VLAN
 
- Ein physisches Netzwerk in viele logische Netzwerke auftrennen.
- Jedes Netzwerk kann beschränkt sein. (z.B. nicht jeder kann Zugriff auf Geschäfts VLAN haben).
- Verkleinern der Broadcastdomäne.

- TAG
- Port am Switch
- TCP/UDP-Port
- MAC-Adresse 
- IP-Adresse


![VLAN-Konzept](https://user-images.githubusercontent.com/44840806/145230950-aba54926-976c-403b-aa75-92ccb8c1000f.png)



# 4.1. IPv4-Adressen definieren


## Dezimale in binäre Zahlen konvertieren

### Basis 10 - Dezimalzahlen

![Dezimale Zahlen](https://user-images.githubusercontent.com/44840806/145231893-bc90ee0f-3549-4f6d-8400-20b89d0b65b9.png)


### Basis 2 - Dual nach Dezimale

![Binäre Zahlen](https://user-images.githubusercontent.com/44840806/145232663-3e1e471d-cee6-413b-86a7-57fbafa5ef9f.png)


### Basis 10 - Dezimal nach Binär

![Dezimal zu Binär umwandeln](https://user-images.githubusercontent.com/44840806/145235098-68df20c5-2ece-429f-81e9-aa0070723f2f.png)


## Aufbau einer IPv4-Adresse

- z.B. 192.168.100.2 ist eine IPv4-Adresse
- Der Computer sieht diese Zanl als Binärzahl.
- Diese Zahlt hat insgesamt 32-Bit Länge. 2 ^ 32 = rund 4 Milliarden IP-Adressen. Damals ausgereicht, heute aber nicht mehr. 

![IPv4](https://user-images.githubusercontent.com/44840806/145380180-4a704e50-1839-48ab-bce0-39da739d4d85.png)


#### **Spezialfälle**

- Alle Bits auf 0 = reservierte Adresse
- Alle Bits auf 1 = globaler Broadcast
- Alle Bits im Hostanteil auf 0 = Netzwerkadresse
- Alle Bits im Hostanteil  auf 1 = Broadcast des Netzwerk 


---
## Resorces: 
[Linkedin Learning: Netzwerkadministrator:in werden](https://www.linkedin.com/learning/netzwerkgrundlagen/willkommen-zu-netzwerkgrundlagen?autoAdvance=true&autoSkip=false&autoplay=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A5996a3e6498e41bff67b4a79&resume=false)
