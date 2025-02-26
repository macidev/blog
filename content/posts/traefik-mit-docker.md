+++
title = "Traefik Mit Docker"
date = "2025-02-26T22:59:15+01:00"
author = "Marcus"
authorTwitter = "" #do not include @
cover = ""
tags = ["docker", "traefik"]
keywords = ["docker", "traefik"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
color = "" #color from the theme settings
+++

# Traefik mit Docker
## Einführung
Kurz und knapp vorneweg erklärt: Traefik ist ein Reverse Proxy. Also unter anderem ein Webserver, 
der als Eingang für Webanwendungen oder Ähnliches fungieren kann. 
Damit ist es beispielsweise möglich relativ einfach unterschiedliche Dienste wie ein Wiki, 
Websites und Anwendungen mit einem SSL Zertifikat und entsprechender Weiterleitung zu installieren. 

Ohne Reverse Proxy muss ich den Webserver entsprechend konfigurieren. Habe ich aber in einem Docker Container ebenfalls ein Webserver, 
wird das ganze schwierig bis unmöglich. 

Da ich gerne mit dem ein oder anderen Tool herumspiele, habe ich eine einfache Möglichkeit gesucht. 
Durch diverse Gespräche mit einem Kumpel aus der DevOps-Szene bin ich dann auf Traefik gestoßen. 

Anfangs war das alles Andere als einfach. Damit ich das nicht vergesse, wie ich das zusammengebastelt habe, gibt es diesen Blog-Beitrag. 

Die Quellen und Docker-Files findest du im Repo zum Beitrag auf [Codeberg](https://codeberg.org/buzigde-blog/traefik-mit-docker). 

## Annahmen
Da wir hier unter Umständen mit SSL Zertifikaten arbeiten, ist ein über das Internet erreichbarer Host (Spielserver) eine Empfehlung. 
Auf der Arbeit habe ich den Luxus nicht, hier habe ich lediglich die SSL-Zertifikatsgenerierung deaktiviert. 

Ich gehe weiter davon aus, dass bereits schon einmal mit Docker gearbeitet wurde. 

Du hast Docker bereits eingerichtet und der Service läuft. 

## Hinweis

> Ich übernehme keinerlei Haftung oder Verantwortung über den Betrieb oder Verwendung der im Blogpost oder Code Repository erwähnten 
> Tools oder Lösungen. Denke bitte immer selbst nach, bevor Dienste im Internet an bietest. 
> Wenn du dir nicht sicher bist, dann ist es ein gutes Zeiten, dies nicht zu tun. 

## Erste Schritte

Neben einer docker-compose.yml wird auch eine Konfigurationsdatei für Traefik benötigt. Man kann das zwar alles in der docker-compose Datei hinterlegen, 
allerdings ist das irgendwann etwas unübersichtlich und 