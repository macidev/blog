+++
title = "Why QA oder warum Qualitätssicherung wichtig ist"
date = "2023-02-22T15:22:51+01:00"
author = "Marcus"
authorTwitter = "" #do not include @
cover = "posts/why-qa/this-is-fine.jpg"
tags = ["qa", "software", "quality assurance"]
keywords = ["qa", "software", "quality assurance"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
color = "" #color from the theme settings
+++

## TL;DR
Weil es dir den Allerwertesten rettet!


## Aller Anfang
Als ich meine berufliche Laufbahn vom technischen Support hin zur Entwicklung vollzogen habe, ist mir einiges aufgefallen. 

Kommend vom Support einer Physiotherapiesoftware (Marktführer, wie der Chef immer betonte), wusste ich, dass Projektmanagement und das Testen wichtig ist. 
Nicht selten wurden Versionen zurückgezogen, da die Berechnungen nach dem Heilmittelkalatog nicht stimmte oder Programmfunktionen nicht aufrufbar waren, wenn die Auflösung zu groß oder klein waren. 
Natürlich waren immer die Entwickler Schuld und dass muss doch ... 

Nach einem Jahr bei der Shopware AG und anderthalb bei der Kellerkinder GmbH weiß ich, dass der Entwickler selten "Schuld ist". Man könnte das jetzt auf das Team münzen und hier allen die Verantwortung über helfen. 
Klar, im Grunde ist das Team verantwortlich, dass eine Funktion oder ein kompletter Programmteil funktioniert. 
Allerdings gibt es immer mehrere Komponenten und wenn man genauer hinschaut, kristallisiert sich heraus, dass die Qualitätssicherung (QA) und nicht selten auch das Projektmanagement eine Verantwortung trägt. 

Zu meiner Zeit in der technischen Hotline des Physiotherapiesoftwareherstellers war die einzige Qualitätssicherung das Projektmanagement selbst. 

### Das bisschen QA macht das Projektmanagement selbst
Ja, richtig gelesen. Diejenigen, die den Entwicklern die Aufgabe geben, etwas nach Vorgabe XY umzusetzen, haben auch die Arbeit kontrolliert. 
Das hieß, dass die Entwickler ein Update-Paket erstellt haben und das dem Projektmanager übergeben haben. So etwas wie eine Build-Pipeline, Smoke-Tests oder gar Integrationstests gab es nicht. 
Als ich wegging, wurde aufgrund neuer Programmteile und anderer technischer Notwendigkeiten mit der Verwaltung mit GIT gestartet. 2017 wohlgemerkt. 
Gut, ich muss ruhig sein, dank den Jungs vom CT-Admin-Team bei Shopware hat GIT bei mir so richtig erst 2022 gezündet. Verwendet hatte ich es allerdings schon weitaus früher. 

Zurück zum Punkt, welchen ich eigentlich machen wollte. Meiner bescheidenen Meinung nach, kann ein Projektmanager nur in sehr geringen Ausmaß die Qualitätssicherung für die von ihm erstellten Anforderungen leisten. 
Nicht, weil der Intelekt fehlt, sondern weil der Blick auf das was er oder sie gewünscht hat, verfälscht ist. 

> Ein kleines Beispiel: 
> 
> Du bestellst bei deinem Kumpel eine Kugel Zitroneneis. 
> Er kommt mit einer schönen glänzenden Kugel Eis in der Waffel zurück. Bist du dir sicher, dass es Zitrone ist, oder vielleicht nicht doch Joghurt, Vanille etc?
> Du musst daran riechen, es kosten, um sicherzugehen. **Das ist im Grunde QA**. :D

Ich weiß, das ist etwas gekünstelt, aber sollte auch nur grob veranschaulichen, was ich meine. Wenn du etwas bekommst, das nach Zitroneneis aussieht, gehst du davon aus, dass es im Grunde auch das ist. Logisch. 

Liebe Leserin, verstehe mich nicht falsch, manche Projektmanager in meiner Karriere waren hervorragend, manche allerdings mehr auf das Verkaufen beim Kunden oder dem Chef aus. 

## Was macht nun die Qualitätssicherung? 

_Im Grunde die ganze Zeit Eis essen ..._ 

Nein, im Ernst. Es ist ein vielschichtiges Aufgabengebiet und nicht per se zu verallgemeinern. Nachfolgend wird meine Meinung und Erfahrung wiedergegeben. 

Eigentlich fängt Qualitätssicherung vor dem Schreiben der ersten Code-Zeile an. Die Anforderung wird gelesen, etwaige Probleme erkannt und kommuniziert und die evtl. schon vorhandenen Akzeptanzkriterien werden verfeinert. 
Es wird im Grunde der Test für das geplante Feature/die Funktion erstellt und durchdacht. 

Folgende Fragen werden hier (grob) beantwortet: 

- Auf welchen Systemen wird das System/die Software eingesetzt?
- Welche Auflösung wird hier relevant sein
- Gibt es spezielle Anforderungen an den Nutzer und werden diese wirklich berücksichtigt
- funktioniert das Entwickelte wirklich? 
- Wie funktioniert das im Kontext des kompletten Programms?
- Chaos-Monkey: was passiert, wenn ich mich nicht erwartungsgemäß verhalte

> By the way: für Tests und Infos hierzu bezüglich des Shopware-Universums, kann ich [Ramonas Blog](https://www.ramona.codes/de/blog/) nur empfehlen. Mal ganz von ihren Talks abgesehen. 

Ach und ein wichtiger Satz ist auch: **Tests stellen Fehler fest, nicht die Abwesenheit eben Jener**. 

## Warum benötige ich nun die QA und warum wird das so selten genutzt?

Die Qualitätssicherung wird schlichtweg benötigt um die Produktqualität gleichbleibend (hoch) zu halten und vor Kundenkontakt etwaige Probleme zu sehen. 
Gute Qualitätssicherung kontrolliert sich selbst, einfach um sicherzugehen, dass nichts übersehen wurde. 

Der Grund, warum dies selten genutzt wird, ist recht simpel. Es kostet einfach Geld. Als Agentur kann ich meistens dem Kunden selten den Punkt "Testing und Qualitätssicherung" auf dem Angebot entsprechend erklären. 
Das wird dieser meist nicht bezahlen. Die Annahme, dass die Agentur ja schon korrekt liefern wird, liefert hier leider recht schnell das Problem mit. 

Gute und effiziente Qualitätssicheurng sorgt dafür, dass im Support weniger geleistet werden muss und das Produkt erwartungsgemäß funktioniert. 

Hast du Ergänzungen oder eigene Gedanken? -> Schreib mich auf [Mastodon](https://mastodon.social/@buzigde) an oder sende mir eine [E-Mail](https://buzig.de/page/kontakt). 
