# Trantek - teknologi plattform for fagfolk

Versjon 0.1

Som en del av FoU programmet TRAN ble det utviklet metodikk og verktøy for analyse av trafikktekniske data. Dette settet med docker containere og script er bygd på resultatene av programmet. Trantek pakken er bare flere av verktøyene satt sammen til en pakke som gjør det enklere å installere nødvendige programmer på en enkel og grei måte. 

## Oppsett av docker containere
I hovedsak brukes docker compose for å styre containerene. Trantek bruker ikke docker på en kreativ måte for å gjøre dataanalyse og informasjons tilvirkning enklere. I noen tilfeller betyr dette at vi bryter med docker best practise, det gjøres for å få en så enkel dataanalyseplattform som mulig.

## Oppsett av apper
Enkelte program egner seg ikke som docker applikasjone og må følgelig installeres lokalt. I mappen **lenker_til_apper** finnes liste over programmer og tips til installasjon.




20180802 Tomas Levin