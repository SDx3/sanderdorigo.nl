---
draft: false
title: "Gelieve niet te hacken"
author: Sander Dorigo
date: 2020-12-15
source: Blog
2020: "12"
categories:
- "self"
credit: https://twitter.com/xwolf/status/1193799290646409217?lang=de
postImage: images/blog/coffee.jpg
---

Het is stil, op het gebied van digitale weerbaarheid. Althans, dat vertelde ik een collega van de week. Stilte voor de storm ben ik bang. Er gebeurt genoeg in het nieuws hoor. Maar als FireEye gehackt wordt en het toegeeft weet je dat het ernstig is. Voor elke Goliath die omvalt, hoeveel Davids zijn er wel niet?

<!--more-->

Dat bedrijven en overheden stil zijn op dit gebied snap ik. Maar ik krijg niet goed naar boven of dit een soort corporate stoerdoenerij is (vooral niet falen) of dat men het echt niet weet. Op zich snap ik wel dat ze hun weerbaarheid (of gebrek daar aan) liefst in stilte oppakken. Maar als het gaat om de weerbaarheid van kritische infrastructuur bijvoorbeeld heb ik het gevoel dat het er slecht voor staat.

### Legacy

Kijk naar onze netbeheerders en stroomleveranciers. Er gebeurt veel hippe shit in dat segment. Smart cities, smart grids, smart life! Maar blijf met je tengels van onze oude stroomverdeelkastjes af, want dat is kritische infrastructuur. Die monitoren we op afstand met een PLC uit de jaren 80, hoezo? Dat klopt van geen kanten natuurlijk.

Als je ergens in een weiland een anoniem gebouw ziet staan met een hek van drie meter er omheen en geen logo op de gevel: dan is het iets met kritische infrastructuur. Let op: ook hun stroomverdeelkast staat waarschijnlijk buiten het hek. Goede symboliek, want daar waar het risico echt ligt is vaak niemand te vinden. Wie heeft er geen `legacy` in huis? En je weet vast ook dat geen product owner of DevOps team zich geroepen voelt om die ouwe zooi op te ruimen. Die zijn veel liever in Azure CI/CD pipelines aan het bouwen dan dat ze ASP.NET 3.2 applicaties onderhouden op een Windows 2000 machine. Maatregelen tegen hackers zijn ook kletskoek want "*deze oplossing is slechts tijdelijk*." Alsof de hacker dat interesseert.

### Spul

Als je maar lang genoeg met dure dingen werkt wordt het vanzelf gewoon. Het wordt spul. Dure horloges, auto's, sieraden. Ik kende ooit iemand die dure BMW's verkocht. Hij ging er mee om alsof het derdehands Kia's waren. Het wordt spul.

Ook zo'n mooi verhaal trouwens. Geen idee of het waar is hoor. Tijdens de omwisseling van de gulden naar de euro lag er een gigantisch warenhuis vol met geld in het groene hart. Superbeveiligd, overal hekken en camera's. Maar waar gehakt wordt, vallen spaanders, en ook in dit warenhuis is weleens een vorkheftruckje door een pallet heen gereden. Wat doen ze? Bezem pakken en een vuilniszak en gauw de rommel opruimen voor de baas het ziet. Twintig miljoen over vloer en *nobody cares*. Het wordt spul. 

### Gelieve niet hacken

Dat is denk ik het grootste risico met onze kritieke infrastructuur. Onze ouwe `legacy` servers en de gaten in ons netwerk. Het wordt spul. We weten het, we vergeten het. Daar loop je risico. Monteur laat de deur open staan van een verdeelstation. En alle PLC’s zitten direct op het internet want dat is handig. De NS heeft overal glasvezel want het koper werd gejat, maar de kabels liggen nog steeds langs het spoor ready om te tappen.

In die context en de "koude oorlog" waar we ons in bevinden met landen als Rusland en China, zou ik me als "staatsactor" vooral nestelen in de kritische infrastructuur van een ander land. Waarom *live* iets hacken zoals op TV en in films? Als je  al een backdoor hebt hoef je hem alleen nog maar aan te zetten als de nood aan de man is. Nestel je in de legacy die elke organisatie heeft en je hoeft alleen maar te wachten tot de *Krieg* begonnen is. Vergis je niet hoeveel geduld een hacker kan hebben. Denk maar aan de IRA: "*we only have to be lucky [once](https://en.wikipedia.org/wiki/Brighton_hotel_bombing) -- you will have to be lucky always.*"

Inmiddels ben ik door het nieuws ingehaald, want zo'n [18 duizend klanten](https://arstechnica.com/information-technology/2020/12/18000-organizations-downloaded-backdoor-planted-by-cozy-bear-hackers/) zijn potentieel de pineut van de bug in SolarWinds waarmee FireEye werd gehackt.