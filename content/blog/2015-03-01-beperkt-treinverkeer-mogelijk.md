---
draft: false
title: "Beperkt treinverkeer mogelijk"
author: Sander Dorigo
date: 2015-03-01 12:00:00
source: Blog
2015: "03"
categories:
- "self"
- "Internet"
postImage: images/blog/train.jpg
credit: https://www.ns.nl
---

Misschien herinner je je [de nieuwsberichten](http://www.theguardian.com/technology/2015/feb/27/samsung-voice-recording-smart-tv-breach-privacy-law-campaigners-claim) nog dat Samsung-televisies je zouden "bespioneren". De zogenaamde "smart"-functies zoals Netflix en spraakcommando's zouden allemaal terug naar Samsung worden gesluisd. Paranoide internetters begonnen al te protesteren en Samsung ontkende enige betrokkenheid bij zulke vuige streken. Het was allemaal uit liefde, aldus de Koreaanse fabrikant.

<!--more-->

Omdat ik er toch niet heel erg blij mee was dat mijn televisie die gekke jongens uit Seoul vertelde wat ik allemaal met mijn TV deed, ben ik eens lekker gaan nerden om daar verandering in te brengen. De benodigdheden? Een [Raspberry Pi](http://www.raspberrypi.org/) (een soort micro-computertje, zo groot als een pakje sigaretten) en wat geklungel met lange Linux-commando's.

Want wat blijkt nou? Zo'n Raspberry kan doen alsof-ie een router is. Net als dat ding van je internetprovider, maar dan zelfbouw. Je maakt je eigen wifi-netwerk, en je zegt tegen de televisie dat-ie met jouw zelfbouw-wifi moet verbinden. Omdat je dat netwerk zelf hebt gebouwd kan je precies zien wat er allemaal gebeurt.

Normale nerds doen dat niet om hun televisie terug te bespioneren. Die gebruiken dit trucje om advertenties te blokkeren. Zo'n zelfbouw-wifi-netwerk werkt namelijk precies zoals je gewone internet. Alles doet het. Netflix, internet, radio, alles. Maar op het moment dat je een advertentie probeert te kijken zegt het netwerk ineens "_huh? advertenties.nl? Nog NOOIT van gehoord. Geen flauw idee!_". Het prettige resultaat is surfen zonder advertenties.

Maargoed, je kan dus precies zien wat er gebeurt op zo'n netwerk. En zie hier het resultaat. Een selectie ([hier staat de hele lijst](http://pastebin.com/5irNG2DP)) sites waar mijn TV verbinding mee maakt, _als ik hem aan zet_:

```
api-hub.samsungyosemite.com
eu-api.samsungyosemite.com
gtrack.adform.net
guide.internetat.tv
lcprd2.samsungcloudsolution.net
rdedcdn.krxd.net
www.samsung.com
```

Als het je niks zegt, dat geeft niks. Maar is het niet vreemd dat een televisie zoveel websites moet bezoeken? Lijkt me nergens voor nodig! Wat blijkt? Advertenties, media-informatie, stem-commando's, alles komt en gaat van zo'n televisie. Via het wereldwijde web.

Inmiddels is dat verleden tijd. Want mijn zelfbouw-netwerkje blokkeert al die sites. Zodra de televisie naar al die advertentiesites probeert te surfen, doet mijn Raspberry PI ineens alsof-ie van niks weet. De televisie kan daar wel tegen. Die denkt, het zal wel even plat zijn, straks nog eens proberen. Maar wij weten wel beter!

Ook leuk: als je teveel blokkeert dan denkt je televisie dat het internet plat is. Want het internet is namelijk gelijk aan samsung.com. Als de site van Samsung plat is, dan is het hele web plat. Yep.

