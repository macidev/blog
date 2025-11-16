+++
title = "Gedanken Zur Edv Struktur"
date = "2025-11-15T21:52:39+01:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "Marcus"
cover = ""
tags = ["netzwerk", "homelab"]
keywords = ["network", "homelab"]
description = ""
showFullContent = false
readingTime = true
hideComments = true
+++

# Gedanken zur EDV-Struktur

In den letzten Jahren hat ich neben einer neuen Fritzbox bei mir in "Homelab" eher wengier bis nichts getan. 
Ich nutze immer noch eine Synology DS 110j aus dem Jahr 2010. Ja, wirklich so alt ist das Modell. 

Ein Single-Bay NAS von Synology mit einer USB HDD als Backup. So richtig Old-School. 

Ich dachte, es gibt meinerseits neue Anforderungen an ein leistungsfähiges NAS mit Truenas, 4-5 Festplatten und Docker-Containern darauf. 

Nachdem ich allerdings mit meinem Freund Steffen über das Für und Wider eines neuen NAS von Ugreen oder Ähnliches gesprochen habe, 
wurde mir nahe gelegt mal zu grundsätzlich zu überlegen, wie denn hier das Netzwerk und die Teilnehmer eben jenem aussehen soll. 

Vielleicht bringt dem geneigten Leser dies nachfolgenden Überlegungen ein Gedankeneinstoß. Mal schauen. 

## Zielbild & Wünsch dir was 

Anstatt mir nun das vorhandene NAS, den Router oder sonstige Hardware einfach zu ersetzen, sollten wir mal überlegen, 
was eigentlich benötigt wird. 

Wir gehen also mal daran und formulieren in Textform, was wir gerne haben würden. 

Netzwerk:
- gute WLAN-Abdeckung überall in der Wohnung/Haus
- WLAN im Keller und in der Nähe des Stromzählers
- In der Wohnung sämtliche Geräte verkabeln wo es irgend geht
- Unterschiedliche WLANs für Gast und Smarthome

Speichern
- Backups der Rechner abspeichern
- Bilder (RAW und Smartphone)
- Netzwerklaufwerke für den Austausch von Ordnern und Dateien
- Medieninhalte ablegen zum lokalen Streamen

Dienste & dergleichen
- Home Assistant
- Ad-Blocker
- Docker-Server
- virtuelle Server zum Spiele oder Testen

## EDV aktuell im Betrieb

Die aktuelle Bestandsaufnahme mit vorhandener EDV:

- Router: Fritzbox
- Switche: 
  - HP HP-2530-24G
  - diverse 5-8 Port Switche
- Fritz Powerline 1260E
- Synology DS 110j
- PiHole 
- Raspberry Pi mit HomeAssistant
- Rechner mit TrueNAS
- Smarthome
  - Steckdosen
  - Beleuchtung
  - Wetterstation

## Probleme
Warum mache ich das Ganze? Im Grunde gibt es aktuell ein paar Aufgaben und Probleme, 
die ich nur bedingt bis gar nicht umsetzen kann. 

Ein komplettes Trennen von Netzwerken ist mit der Fritzbox nicht ohne massives Umbauen möglich. 
Dann kann ich gleich ein System wählen, welches das komplett kann. 

Das NAS System aktuell mit dem DS110j ist doch etwas arg in die Jahre gekommen und wird auch nicht mehr von Synology unterstützt. 
Der TrueNAS Server ist im Grunde eine tolle Alternative, aber ist ein kompletter Rechner, welcher irgendwo stehen muss. 

Aktuell gibt es zudem kein Spielserver, worauf ich mal eben "einfach" eine Linux VM starten könnte, oder Windows ... 
Mal ganz von etwaigen Docker Containern abgesehen. 

Zusammengefasst: 
- aktuell unflexibles Netzwerk mit teilweise schlechter WLAN-Reichweite, bzw. keiner (im Keller).
- altes NAS System oder zu komplexes System
- keine Trennung von Diensten/EDV-Komponenten, bzw. nicht sinnvoll aufgebaut. 2 Raspberri Pies für 

## Zukunftspläne

Wie wird das nun in Zukunft gehen? Bisher macht die Fritzbox auch die Telefonie. 
Das soll allerdings nicht der Hinderungsgrund sein. Es gibt ja zum Glück noch VoIP Telefone. 

Ziel ist somit: 
- verbesserten WLAN-Empfang
- einfaches Management
- Dedizierte Geräte für dedizierte Aufgaben. 
- Datenspeicherlösung mit Backups im Netzwerk

Wie will ich das alles erreichen?

| Gerät              | Bisher                       | Zukünftig                                                                                        |
|--------------------|------------------------------|--------------------------------------------------------------------------------------------------|
| Router             | Fritzbox                     | Ubiquiti Cloud Gatway Ultra                                                                      |
| Wifi               | Fritzbox & Fritzbox Repeater | Ubiquiti U6+                                                                                     |
| Switch             | Netgear & HP                 | Netgear & HP plus Ubiquiti Ultra 60W                                                             |
| NAS                | Synology DS110j              | ?                                                                                                |
| Keller & Waschraum | Fritz Repeater via dLAN      | Keller: dLan Adapter von AVM Waschraum ggf. ebenfalls AVM Adapter oder Ubiquiti Swiss Army Knife |
| Telefonie          | 2x Telekom Handsets          | Grandstream WiFi-Handset WP816                                                                   |
| Spielserver        | TrueNAS PC                   | PC mit Proxmox                                                                                   |

### WLAN

- 1 Gast Wlan 
- 1 internes LAN
- 1 Smarthome Wlan