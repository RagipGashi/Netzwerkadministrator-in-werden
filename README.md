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



---
## Resorces: 
[Linkedin Learning: Netzwerkadministrator:in werden](https://www.linkedin.com/learning/netzwerkgrundlagen/willkommen-zu-netzwerkgrundlagen?autoAdvance=true&autoSkip=false&autoplay=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A5996a3e6498e41bff67b4a79&resume=false)
