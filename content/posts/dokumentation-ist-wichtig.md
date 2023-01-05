+++
title = "Dokumentation ist wichtig"
date = "2022-04-06T21:48:28+02:00"
author = "Marcus"
authorTwitter = "buzigde" #do not include @
cover = ""
tags = ["entwicklung", "dokumentation"]
keywords = ["entwicklung", "dokumentation"]
description = ""
showFullContent = false
readingTime = true
+++

# Dokumentation ist wichtig

In meinem letzten [Blog-Post über Fehler in der Entwicklung](https://www.buzig.de/posts/fehler-in-der-entwicklung/) habe ich darüber geschrieben, dass man nicht in Featureitis versinken sollte. 

Getreu gem Motto: Get the sh*t done

In diesem Beitrag möchte ich darüber schreiben, warum Dokumentation so wichtig ist. 

## Was kann man unter Dokumentation verstehen?

Gut geschriebener Code sollte doch im Grunde genug sein oder? Einfach nicen Code schreiben und fertig ist die Laube. 
Im Grunde ja, aber leider auch ein **ganz großes Nein**. 
Code, den du vor Tagen oder Wochen geschrieben hast, war zu dem Zeitpunkt der "richtige" Code. Du hast im Zweifel den genauen Kontext nicht. 

Jetzt stelle dir vor, dass du eine super formulierte Dokumentation hast, die in sich geschlossen beschreibt, wie du eine Funktion des Programms nutzen kannst. 

Beide Dokumentationen haben ihre Probleme. Nicht ohne Grund haben einige große Firmen und OpenSource Projekte teilweise massive Schwierigkeiten 
ihre Dokumentation sinnvoll und verständlich zum richtigen Zeitpunkt zur Verfügung zu stellen. 
Im ersten Beispiel haben wir das Problem, dass das Ziel im Zweifel nicht klar ist und somit der Code selbst vielleicht super aussagekräftig ist, 
nicht aber im Kontext des Projektziels oder dem Plan, der zum Entstehungszeitraum im Kopf war. 
Beim Zweiten haben wir eine Dokumentation, es wird aber nicht beschrieben, wie du Teile deines Codes in anderen Bereichen deines Programms wiederverwenden kannst. 

Während der Entwicklung meines Gin-Portals habe ich mehrfach das Problem, dass ich Dinge über den Haufen werfe und den Code mit etwaigen Kommentaren wegwerfe. 
Doof, wenn hier dann das eigentliche Ziel formuliert war. 
Für das zweite Beispiel habe ich auch direkt den Grund, warum ich diesen Beitrag schreibe. 
Im speziellen Fall habe ich die Möglichkeit gesucht, mit Symfony 6 Daten aus einem Controller in einem anderen auszugeben. 
Es ist hervorragend dokumentiert, wie ich mit Doctrine Datenbankabfragen erstelle, nicht aber wie ich das erreiche, was ich wollte. 

Am Ende war die Notwendigkeit eines Services gegeben. Danke Steffen für die Erklärung und die Vorgabe der Richtung. 

# Und jetzt? 

Ja, das fragt sich der geneigte Leser an dieser Stelle vielleicht. 

Naja, Gitlab und Github liefern nicht umsonst Funktionen wie Wiki und Static Site Hosting mit im Projekt an. 
Nutze das um das Projekt und die Ziele zu dokumentieren. 
Besuche zudem Meetups für Entwickler und tausche dich aus. 

**Ich bin dazu über gegangen, mir wichtige Komponenten entsprechend zu dokumentieren und das Ziel aufzuschreiben und einige Menschen in meinem Umfeld Wissen zu entlocken.** 

Du hast Ergänzungen? Ab in die Kommentare damit. 