# Trantek - teknologi plattform for fagfolk

Versjon 0.1

Som en del av FoU programmet TRAN ble det utviklet metodikk og verktøy for analyse av trafikktekniske data. Dette settet med docker containere og script er bygd på resultatene av programmet. Trantek pakken er bare flere av verktøyene satt sammen til en pakke som gjør det enklere å installere nødvendige programmer på en enkel og grei måte.

## Oppsett av docker containere

I hovedsak brukes docker compose for å styre containerene. Trantek bruker ikke docker på en kreativ måte for å gjøre dataanalyse og informasjons tilvirkning enklere. I noen tilfeller betyr dette at vi bryter med docker best practise, det gjøres for å få en så enkel dataanalyseplattform som mulig.

## Porter og oppkobling
- Jupyter lab: **http://localhost:9999/lab**
- Jupyter notebook **http://localhost:9999**
- NodeRed: **http://localhost:1899**
- Postgresql: 7432 på localhost - 5432 internt i dockernettverket
- Mongodb: 27017 på localhost 
- Mongodb express 8081 på localhost

Default brukernavn og passord:
Brukernavn: trantek
Passord: svv123svv

**NB**, dette er ikke sikre passord og er kun beregnet for kjøring på localhost. Sett opp brannmur til å blokkere 9999, 1899, 7432 og 27017 for andre enn localhost. For en serverinstans bruker SSH tunnel for å koble opp mot localhost.

## Oppsett av apper

Enkelte program egner seg ikke som docker applikasjone og må følgelig installeres lokalt. I mappen **lenker_til_apper** finnes liste over programmer og tips til installasjon.

20180828 Tomas Levin