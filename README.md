# publicera-co2-halten

Så här kan man göra för att publicera koldioxidhalten i sina lokaler. Fem steg som behöver göras en gång, inga löpande kostnader. Tanken är att ge ut en USB eller minneskort och det bara funkar, men just nu måste man vara bekväm med att installera python-kod på en dator.

Så här blir resultatet: https://mas.to/@koldio/109808222410697067

1) Skaffa en TFA Dostmann CO2-mätare, kostar runt 800 kronor. Denna mätare är bättre än nästan allt annat i prisklassen, då den inte behöver justeras (kalibreras) en gång om dygnet. Vilket gör att den även funkar bra i lokaler som inte vädras ut helt varje dygn.

2) Plugga in mätaren i en dator med en USB-kabel. Jag har använt Linux.

3) Installera koden från detta repository: Det är en modifierad version av xx till att ge 24 timmars diagram, samt spara diagrammet till disk istället för att visa det i ett fönster

4) Skaffa ett konto på en Mastodonserver, och registrera en applikation där och spara ner nycklarna för applikationen

5) Installera koden från detta repository: https://github.com/jorgenponder/co2-data-publisher Det laddar upp bilden från förra steget, till ditt konto på en Mastodon-server, var fjärde timma. Eller det gör det om du lägger det i ett cron-jobb som kör det var fjärde timma.

Efter detta så ska dina CO2-data publiceras på ett Mastodon-konto var fjärde timma.


