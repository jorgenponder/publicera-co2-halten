# publicera-co2-halten

Obs! Detta är alfa-kod. Och alfa-instruktioner.

Så här kan man göra för att publicera koldioxidhalten i sina lokaler. Fem steg som behöver göras en gång, inga löpande kostnader. Tanken är att ge ut en USB eller minneskort och det bara funkar, men just nu måste man vara bekväm med att installera python-kod på en dator.

Så här blir resultatet: https://mas.to/@koldio/109808222410697067

1) Skaffa en TFA Dostmann CO2-mätare, kostar runt 800 kronor. Denna mätare är bättre än nästan allt annat i prisklassen, då den inte behöver justeras (kalibreras) en gång om dygnet. Vilket gör att den även funkar bra i lokaler som inte vädras ut helt varje dygn. https://www.tfa-dostmann.de/en/product/co2-monitor-airco2ntrol-mini-31-5006/
Finns här att köpa t ex: https://www.pricerunner.se/pl/345-5201699/Elverktyg/TFA-AirControl-Mini-CO2-priser

2) Skaffa ett konto på en Mastodonserver, och registrera en applikation där och spara ner nycklarna för applikationen. En möjlighet är https://botsin.space som ska vara bot-vänlig, men det är fördröjning innan man blir godkänd. Läs reglerna för den server du reggar konto på.

3) Plugga in mätaren i en dator med en USB-kabel. Jag har använt Linux.

4) Installera koden från detta repository: https://github.com/jorgenponder/tfa-airco2ntrol-mini Det är en modifierad version av https://github.com/MathieuSchopfer/tfa-airco2ntrol-mini till att ge 24 timmars diagram, samt spara diagrammet till disk istället för att visa det i ett fönster. Det laddar upp bilden från steg 4, till ditt konto på en Mastodon-server, var fjärde timma. Eller det gör det om du lägger publish.py i ett cron-jobb som kör det var fjärde timma.

Efter detta så ska dina CO2-data publiceras på ett Mastodon-konto var fjärde timma.


