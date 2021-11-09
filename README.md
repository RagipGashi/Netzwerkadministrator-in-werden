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


---
## Resorces: 
[Linkedin Learning: Netzwerkadministrator:in werden](https://www.linkedin.com/learning/netzwerkgrundlagen/willkommen-zu-netzwerkgrundlagen?autoAdvance=true&autoSkip=false&autoplay=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A5996a3e6498e41bff67b4a79&resume=false)
