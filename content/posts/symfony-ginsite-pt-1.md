+++
title = "Symfony Ginsite Pt 1"
date = "2021-11-27T12:25:42+01:00"
author = "Marcus"
authorTwitter = "buzigde"
cover = ""
tags = ["php", "symfony", "development"]
keywords = ["php", "symfony", "development"]
description = "Seit einigen Wochen bin ich dabei mich mehr mit dem Thema Symfony tiefer zu beschäftigen. Was passt hier mehr, als Gin-Liebhaber eine Website zu programmieren, mit welcher Gin und Tonic entsprechend matchen kann? Im Ersten Teil schreibe ich, wie ich hier gestartet bin und direkt zweimal neu angefangen habe."
showFullContent = false
readingTime = true
+++

Seit einigen Wochen bin ich dabei mich mehr mit dem Thema Symfony tiefer zu beschäftigen. Was passt hier mehr, als Gin-Liebhaber eine Website zu programmieren, mit welcher Gin und Tonic entsprechend matchen kann? Im Ersten Teil schreibe ich, wie ich hier gestartet bin und direkt zweimal neu angefangen habe.

# Was bitte?
Ja, der geneigte Leser mag sich fragen, wovon ich hier rede. 
Im Grunde ist es ganz einfach. Beruflich habe ich mit [Shopware](https://www.shopware.com/) und einigen Plugins zu tun. 
Die aktuellste Version ist in PHP geschrieben und nutzt das Symfony Framework. Im beruflichen Alltag habe ich nicht allzu viel mit der Entwicklung und den tiefen des Symfony Frameworks zu tun. 
Aus diesem Grunde habe ich mir privat nach einer Möglichkeit geschaut, meine Programmier- und Symfonykenntnisse auszubauen. 

Zudem trinke ich mit Freunden gerne in einer geselligen Runde einen guten Gin. Dadurch kam die Idee, hier ein Portal zu programmieren, welches die einzelnen Gins nebst dazu passendem Tonics matched. 
Natürlich gibt es hier bereits passende Apps und Empfehlungen der Gin-Hersteller. Leider weiß keiner, wie gut die sind, es gibt keine Bewertung und natürlich gibt es unterschiedliche Geschmäcker. 

# Und jetzt?
Soweit so gut. 

Man nehme also PHP, installiere Symfony, haut da einige Module dazu und schon hat man das Grundgerüst. Oder? 
**Leider nein**. 

Mein Ziel war es von Beginn an mit einem möglichst modernen "bleeding edge" Technologiestack zu arbeiten. Das heißt in meinem Fall: 
- PHP 8
- Symfony 5.X
- Bilder auf einem CDN abgelegt
- kein jQuery, sondern vanillaJS ;) 
- Für das Styling SASS 
- kein Bootstrap sondern TailwindCSS
- Codestyle-Checks
- PHPStan zur Qualitätskontrolle
- sauberes Deployment
- Für die Zukunft entsprechendes Caching nebst schnellere Informationen mit vorgeschaltetem Redis

Das bringt natürlich wiederum ein paar Nettigkeiten und größere Herausforderungen mit sich. Mein Vorteil ist allerdings, dass ich Kollegen habe, dir mir diesbezüglich gerne helfen und Fragen beantworten. 

Was ich zu Beginn nicht bedacht habe ist die Tatsache, dass ich mich mit User-Management, Authentifizierung Autorisierung und entsprechendem Datenbankdesign auseinandersetzen muss. 

## Beginn der Entwicklung 
Zu Beginn habe ich schlichtweg Symfony installiert, [Symfony-Casts](https://symfonycasts.com/) Tutorials geschaut und recht schnell ein vermeintlich passendes System aufgebaut. 
Leider hat sich heraus gestellt, dass ich mich in eine Sackgasse begeben hatte. Auch weil ich Symfony nicht beibringen konnte das Aussehen mit TailwindCSS zu erstellen, bzw. überhaupt TailwindCSS zu installieren. 
Ich habe das Projekt also wirklich zweimal weggeworfen und neu aufgesetzt. 

# Der jetzige Stand
Aktuell ist es möglich sich zu registrieren, sich einzuloggen und grundsätzlich vorhandene Gins und Tonics anzuschauen. Das Hinzufügen funktioniert aufgrund der Abhängigkeiten zwischen unterschiedlichen Entitäten noch nicht. 

Interessiert dich hier mehr dazu? Hinterlasse einen Kommentar. Like and Subscribe ... ;) 