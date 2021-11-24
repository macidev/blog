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

// 2do: Erklären der Sicherung der Einstellungen

## Durchgeführte Arbeiten

In meinem Beispiel gehe ich von einer Lösung aus, die lediglich eine Festplatte hat. Sollte deine Synology mehrere Festplatten 
haben oder gar Hot-Swappable sein, also im Betrieb ausgetauscht werden können, so gelten andere Verfahren. 

Im Grunde ist der Vorgang recht simpel. Natürlich ist nach der Datensicherung das NAS auszuschalten. 
Sobald das getan ist, gilt nachfolgende Liste: 

- Ausbau der alten Festplatte
- Einbau der neuen Festplatte
- Download der Synology Software für den Computer 
- Download der DSM-Version vom Server
- Einstecken von Netzwerk und Strom
- Starten das NAS
- Konfiguration des NAS und Einspielen der Software
- Updates durchführen
- Sicherung einspielen (Konfig und Daten)
- Datensicherung einrichten



