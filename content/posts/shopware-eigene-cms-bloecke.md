---
title: "Shopware eigene CMS Blöcke"
date: 2022-02-26T13:32:23+01:00
draft: false
author: "Marcus"
authorTwitter: "buzigde"
cover: ""
tags: ["php", "shopware", "development"]
keywords: ["php", "shopware", "development"]
description: ""
showFullContent: false
readingTime: true
---

# Eigene CMS Blöcke für Shopware 6 

Dieser Blog-Eintrag ist im Grunde lediglich für mich die Erinnerung, Dinge nicht zu vergessen. :D 

Hintergrund ist recht simpel. Da ich privat an einem Windows-Rechner entwickle, habe ich unter Windows Docker und darin [Dockware](https://dockware.io/) im Einsatz. 
Das ist im Grunde auch total super. Leider hat Windows und Docker das Problem mit der Performance und des FileSyncs. 
Aufgrund dessen lade ich via S/FTP über meine IDE PHPStorm sämtliche Änderungen in Dockware hoch. 
Das funktioniert auch super. Allerdings vergisst man dann teilweise, dass hier weniger häufig Dateinamenänderungen gesynct werden. 
Will heißen im Dockware Image sammeln sich allerlei Dateien an. Das musste ich auch schon schmerzlich feststellen. 

Hierfür kann ich einfach `docker exec -it shopware /bin/bash` eintippern und schon bin ich im Container mit dem Namen Shopware eingeloggt. 
Bitte entsprechend anpassen. Hieran im Anschluß wird dann der src Ordner meines Themes oder Plugins gelöscht und via S/FTP erneut hochgeladen. 

Nun aber zum eigentlichen Problem ... 

## Administration und Frontend SCSS- und JS-Dateien ausliefern 

Während der Entwicklung führt man ja häufiger `./bin/build-administration.js` oder/und `./bin/build-storefront.sh` aus. 
Was hier im Hintergrund passiert ist, dass die Code-Schnipsel aus dem leserlichen Source-Code zu entsprechenden 
JS und SCSS Elementen für die Administration oder Storefront zusammen gebaut werden. 

Werden nun, wie bei mir, vom Entwicklungsrechner lediglich zum Docker-Container Änderungen published, 
werden die so generierten JS und SCSS Dateien allerdings nicht mit im Theme oder Plugin hinterlegt. 
Richtig doof wird es dann, wenn der Hoster kein NPM oder Ähnliches installiert ist. (looking at you Mittwald and Profihost)
Ein Aufrufen von `./bin/build-administration.js` oder/und `./bin/build-storefront.sh` also nicht geht. 

Die Lösung ist also schlichtweg die kondensierten JS und SCSS Dateien via Sync-Feature herunter zu laden und mit im Plugin oder Theme mit auszuliefern. 

Lessons learned. ;) 

Und ja, das steht in der [Dokumentation](https://developer.shopware.com/docs/guides/plugins/plugins/administration/add-custom-field#loading-the-js-files) von Shopware. Allerdings ... weißt du ja selbst, ... 

Achso, natürlich wäre das in einem richtigen Deployment mit entsprechendem rsync oder Ähnlichem nicht passiert, ich weiß. 
Hierzu folgt allerdings ein separater Blog-Post. 