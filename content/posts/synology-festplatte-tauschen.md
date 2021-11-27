+++
title = "Synology Festplatte Tauschen"
date = "2021-11-22T23:49:39+01:00"
author = "Marcus"
authorTwitter = "buzigde"
cover = ""
tags = ["synology", "upgrade"]
keywords = ["synology", "upgrade", "festplatte"]
description = "Aufgrund zu vieler Daten, die auf meiner 1 TB Festplatte in meiner DS110j schlummern, habe ich kurzerhand diese durch eine 3 TB ausgetauscht. Den Prozess erläutere ich in diesem Post."
showFullContent = false
readingTime = false
draft = false
+++

> **Wichtige Information** 
> 
> Der Blog-Post basiert auf der nicht mehr ganz so aktuellen DSM 5.2.X. ;) 

## Als Erstes: Datensicherung
Mach bitte eine Datensicherung und stecke diese auch nach erfolgreicher Sicherung bitte auch aus. ;) 
**wirklich, mach eine Datensicherung!**

Die Datensicherung der Einstellungen ist in meiner DSM 5.2.X dediziert separat durchzuführen. 
Es kann allerdings durchaus sein, dass die Datensicherung der Einstellungen zusammen mit der Sicherung der Daten einhergeht. 

## Durchgeführte Arbeiten

In meinem Beispiel gehe ich von einer Lösung aus, die lediglich eine Festplatte hat. Sollte deine Synology mehrere Festplatten 
haben oder gar Hot-Swappable sein, also im Betrieb ausgetauscht werden können, so gelten andere Verfahren. 

Im Grunde ist der Vorgang recht simpel. Natürlich ist nach der Datensicherung das NAS auszuschalten. 
Sobald das getan ist, gilt nachfolgende Liste: 

- Ausbau der alten Festplatte
- Einbau der neuen Festplatte
- Download der [Synology Assistent Software](https://www.synology.com/de-de/support/download/DS110j?version=5.2#utilities) für den Computer 
- Download der [DSM-Version](https://www.synology.com/de-de/support/download) vom Server
- Einstecken von Netzwerk und Strom
- Starten das NAS
- Konfiguration des NAS und Einspielen der Software (Ein Teil wird durch das spätere Einspielen der Einstellungsdatensicherung übernommen)
- Updates durchführen
- Datensicherung einspielen (Konfiguration und Daten)
- Datensicherung einrichten für die Zukunft

So, dann sind wir fertig und du kannst deine Synology wieder benutzen. :D 

Ernsthaft, im Grunde ist das wirklich so einfach. 

Vielleicht gibt es Rückfragen, lass mir dann doch einfach einen Kommentar da, ich antworte gerne. 