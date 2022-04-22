---
draft: false
title: "Strijden om de crypto-titel"
author: Sander Dorigo
date: 2022-03-22
source: Blog
2022: "03"
categories:
- "self"
- Cryptografie
credit: https://www.esa.int/ESA_Multimedia/Images/2020/11/Interior_of_IBM_s_quantum_computer
postImage: images/blog/quantum-small.jpg
---

De quantumcomputer komt er aan! Online kan je van alles lezen over deze spannende nieuwe ontwikkeling. Voor mij is vooral de cryptografie interessant: een quantumcomputer is akelig goed in wiskunde, en dat is een risico voor veel van de cryptografie die we tegenwoordig gebruiken.

<!--more-->

Gelukkig is het nog niet zo ver. De huidige quantumcomputers nemen een gebouw en beslag en zijn niet heel erg snel, betrouwbaar of goed. Dat doet je misschien wel denken aan de computers van vroeger.

## Digitale versleuteling

Van alle coole dingen die je met een quantumcomputer is het breken van cryptografie nog wel het coolst. Of nou ja, het meest gevaarlijk. Want de cryptografie die we dagelijks online gebruiken (voor bijvoorbeeld WhatsApp) is in de toekomst te breken met zo'n quantum-apparaat. De wiskundige theorie is er al, en de eerste proefjes zijn geslaagd.

Gewone computers doen alles met nulletjes en eentjes. Bits en bytes. Een quantumcomputer rekent op een andere manier, met quantum bits. Deze "qubits" zorgen ervoor cryptografische algoritmes zoals RSA en ECC sneller te breken zijn. Het duurt nog even voor het zo ver is, maar het is een kwestie van wachten. Wil je daar meer over lezen of over zien? Lees dan eens [dit artikel](https://medium.com/swlh/quantum-computing-for-dummies-part-1-2686b9ba3c51) of bekijk [dit filmpje](https://www.youtube.com/watch?reload=9&v=QuR969uMICM).

De meeste cryptografie leunt op het gegeven dat bepaalde wiskunde makkelijk de ene kant op is (voor de encryptie) maar kei-moeilijk de andere kant op (tegen decryptie). Als je de sleutel hebt is het appeltje-eitje, maar zonder die sleutel\.\.\. wachttijden van 5000 jaar zijn niet ongewoon.

Dan is het nogal wat als een quantumcomputer die wachttijd kan terugbrengen naar drie minuutjes. Dat was mooi ff niet de bedoeling!

## De wedstrijd

Gelukkig zagen we dit met zijn allen al aankomen. Knappe koppen hebben nieuwe algoritmes bedacht die niet zo makkelijk door een quantumcomputer gekraakt kunnen worden. Voorbeelden daarvan zijn "[Classic McEliece](https://classic.mceliece.org/)", "[CRYSTALS](https://pq-crystals.org/)" en "[NTRU](https://ntru.org/)". Ze werken met hetzelfde trucje. Het is makkelijk de ene kant op (encryptie) maar zonder sleutel kei-moeilijk de andere kant op. Ook de quantumcomputer helpt niet!

Of ze ook echt werken? Dat moeten we nog zien.

De Amerikaanse organisatie NIST, het *National Institute of Standards and Technology* heeft een aantal jaar geleden [een wedstrijd](https://csrc.nist.gov/Projects/post-quantum-cryptography) uitgeroepen om te zoeken naar algoritmes die **quantumproof** zijn. Het doel is om algoritmes te vinden die niet te kraken zijn door een quantumcomputer én niet door een gewone computer. Zeker dat laatste is ook belangrijk. Ze noemen dit ook wel "postquantum cryptografie" (PQC).

De wedstrijd startte in 2016 met maarliefst 69 kandidaten. *Nice!* Hier zitten ook de voorgenoemde algoritmes bij. Er zijn nu twee rondes geweest waarin heel wat andere potentiële kandidaten alweer afgevallen zijn. 

## De verliezers

Sommige postquantum-algoritmes zijn te groot. De geheime sleutel is bijvoorbeeld een paar megabyte en dat is niet superhandig. Of het is niet te bewijzen dat ze echt veilig zijn, of de veiligheid blijkt gemakkelijk te kraken. Iedereen die een algoritme opstuurt moet alle wiskunde er bij doen en een stukje code schrijven om te bewijzen dat het werkt. Andere cryptografen gaan daar mee aan de slag.

Over het algemeen zijn alle algoritmes complexer en zwaarder dan de huidige algoritmes. De sleutels zijn langer en de wiskunde is complexer. Dat wordt nog een uitdaging voor IoT apparatuur en andere chips met weinig rekenkracht. Het optimaliseren van de algoritmes, en de discussie daarover gaat in alle hevigheid door. [Dit filmpje](https://www.youtube.com/watch?v=Z2RjZB6dVyw) legt meer uit.

## Complot

Uiteraard zijn er diverse uitdagingen rondom postquantum cryptografie. Het begint met Google. Jaren geleden deden zij [een succesvol experiment](https://security.googleblog.com/2016/07/experimenting-with-post-quantum.html) om te bewijzen dat postquantum cryptografie kan werken op het gewone internet. Chrome werd uitgerust met optionele quantumcryptografie en een select aantal websites kon daar ook daadwerkelijk mee omgaan. Die test was uitermate geslaagd. Computers konden prima omgaan met deze cryptografie, websites idem dito en de gebruiker merkte er niets van.

Toch is deze functie weer uitgezet. Hoewel Google zelf aangeeft dat niet alle tussenliggende systemen er mee om kunnen gaan, vermoeden andere mensen een complot en/of opzettelijke vertraging door de Amerikaanse overheid. Logisch. De NSA werkt al jaren aan het doorbreken en omzeilen van cryptografie en gaat zover dat ze zelfs bestaande protocollen met opzet onveilig proberen te maken. Als de NSA dan roept "*gebruik allen* `protocol X` *met de volgende parameters!*" dan kan je je wel voorstellen dat veel mensen [skeptisch](https://blog.cr.yp.to/20220129-plagiarism.html) zijn.

Nu de quantumproof race al gelopen lijkt te zijn voor de NSA goed en wel een quantumcomputer heeft, is het niet heel vergezocht om te denken dat de NSA de ontwikkelingen met opzet dwarsboomt.

## De volgende stap

Volgens anderen is het simpel: iedereen zit in de wachtstand, [de NSA](https://media.defense.gov/2021/Aug/04/2002821837/-1/-1/1/Quantum_FAQs_20210804.PDF) net zo goed. Als de wedstrijd van de NIST is afgelopen dan komt daar een gouden standaard uit die voor iedereen bruikbaar is. Tot die tijd voldoet de huidige cryptografie prima. 

Het is nu wel zaak om eens goed te kijken hoe diep cryptografie zich heeft genesteld in onze systemen. De huidige algoritmes zullen op den duur vervangen moeten worden. RSA, een van de bekendste en meestgebruikte algoritmes is kwetsbaar voor de komst van quantumcomputers. Dit algoritme werd in 1977 gepubliceerd en de meeste werkende mensen hebben nooit iets anders meegemaakt. 

Wij brave burgers wachten ondertussen op de uitslag van NIST en hopen maar dat ook banken deze quantum-race met argusogen volgen en onze centjes veilig houden. 
