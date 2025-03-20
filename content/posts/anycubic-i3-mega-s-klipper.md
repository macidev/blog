+++
title = "Anycubic I3 Mega S Klipper"
date = "2025-03-20T18:03:47+01:00"
author = "Marcus"
authorTwitter = "" #do not include @
cover = ""
tags = ["3D Druck", "anycubic", "Klipper", "tuning"]
keywords = ["3D Druck", "anycubic", "Klipper", "tuning"]
description = "Blogbeitrag über das Installieren von Klipper auf dem Anycubic i3 Mega S mit einem Raspberry Pi Pico 2"
showFullContent = false
readingTime = true
hideComments = false
color = "" #color from the theme settings
+++

# Anycubic i3 Mega S mit Klipper und getuned

Durch einen Bekannten bin ich an einen 3D-Drucker gekommen. Im Grunde ein älteres Modell von Anycubic. Also kein Fancy-Schmänzie Bamboo Gerät.

Schnell habe ich gemerkt, dass hier vieles möglich ist und vor Allem man nicht nur Filament benötigt.
Nach der Bestellung von ordentlich Filament, kleinen Tools und neuer Druckerdüse, habe ich gemerkt, dass der Drucker irgendwie nicht ganz so toll ist. Klar, ist ja auch ein Drucker aus 2020/2021 und die erste Version vom i3 Mega S ist sogar schon aus 2018.

## Der Anfang

Durch einen [Toot](https://mastodon.social/@fribbledom/113981730211002419) von muesli auf Mastodon wurde ich nochmals darauf hin gewiesen, doch auf (m)einem alten Drucker mal Klipper zu installieren.

Da ich zu dem Zeitpunkt meinen Drucker nicht mehr mit dem normalen Weg mit Druckdateien versorgt habe, sondern auf einem Raspberry Pi Pico 2 Octoprint installiert hatte, war der Schritt nur ein Kleiner. Neue Mini-SD-Karte mit Klipper bespielen und los geht's, dachte ich.

### Was ist Klipper?
Klipper ist im Grunde ein Betriebssystem für 3D-Drucker. Er steuert die einzelnen Achsen, sodass Der Druckkopf mit dem geschmolzenen Filament die tollen Dinge drucken kann, welche wir uns vorgestellt haben.

## Vorarbeiten
Was wird nun für die Installation von Klipper benötigt?

1. ein Kompatibler Drucker Details unter [Github Config-Liste](https://github.com/Klipper3d/klipper/tree/master/config)
2. einen Raspberri-Pi mit USB-Kabel für den Drucker
3. Zeit
4. Spaß am Basteln und Grundkenntnisse mit Linux und der Kommandozeile

Bitte schau am Besten, welche Anforderungen noch benötigt werden, vielleicht habe ich etwas vergessen.

Die Linksammlung:
- [Klipper](https://www.klipper3d.org/)
- [Youtube Erklärung von JJ SHankles in englisch](https://www.youtube.com/watch?v=cAxEIdThDiQ)

Was ich hier nicht erklären werde, wie das genau funktioniert. Hintergrund ist hier schlicht, dass die offizielle Dokumentation von Klipper aktueller ist.


# Feedback
Du willst mir Feedback geben? Gerne am Besten auf [Mastodon](https://climatejustice.social/@buzigde)
