# Rapporter

Första ögonblicksbilden 8 november 2026 (Europe/Stockholm) lämnade katalogen tom. Det gäller den incheckningen.

Ingång: [../README.md](../README.md). Förfrågningar: [../requests/README.md](../requests/README.md). Mall: [../REPORT-TEMPLATE.md](../REPORT-TEMPLATE.md).

Rapporter som ligger här nu är statusloggar för REQ-20261108-18, mottagna omkring 21:25. De är vidarebefordrade utsagor, inte oberoende granskning och inte bevis för underlagen. De stänger inget leveransuppdrag. En rapport väcker ingen agent och godkänner inte nästa steg. Jämför SHA och commit-tid innan du litar på texten.

Skriv inte hemligheter, privata sökvägar, maskinprofil, interna adresser eller avtalsvillkor i rapporter i det här publika repot.

## Index

| Rapport | Innehåll |
| --- | --- |
| [REQ-20261108-18-vistion.md](REQ-20261108-18-vistion.md) | Fem rollsvar. Uppdrag 10–13 blockerade före start. |
| [REQ-20261108-18-vanprojekt.md](REQ-20261108-18-vanprojekt.md) | Fem rollsvar. All teknik ostartad. |
| [REQ-20261108-18-25design.md](REQ-20261108-18-25design.md) | Bara ledarens utsaga. Rollsvar saknas. |
| [REQ-20261108-18-lampsajt.md](REQ-20261108-18-lampsajt.md) | Delstatus. Tre roller saknas. |

## Blockerat, 10–13

Dessa fyra filer är blockeringsrapporter. Uppdragen REQ-20261108-10 till 13 förblir `blocked`. De är inte klara sakuppdrag. Konceptversionen är inte verifierad. Samordningsreferensen i rapporterna är `03b261d8f566f8427196e3be85c0459c69f530c1` och är inte en koncept-SHA.

| Rapport | Innehåll |
| --- | --- |
| [RPT-REQ-20261108-10.md](RPT-REQ-20261108-10.md) | BLOCKERAT. Idéer och research. Inte en konceptjämförelse. |
| [RPT-REQ-20261108-11.md](RPT-REQ-20261108-11.md) | BLOCKERAT. UX och visualisering. Inte UX-acceptans. |
| [RPT-REQ-20261108-12.md](RPT-REQ-20261108-12.md) | BLOCKERAT. Testare. Kontrollerna är inte skrivna. |
| [RPT-REQ-20261108-13.md](RPT-REQ-20261108-13.md) | BLOCKERAT. Säkerhet och integritet. Inte en kodgranskning. |

## Procedur, separat från 10–13

[RPT-REQ-20261108-22.md](RPT-REQ-20261108-22.md) är procedurtexten för REQ-20261108-22 och REQ-20261108-09. Inget Mac-prov är utfört. REQ-20261108-05 är inte startad. Granskningsbeslutet är `unreviewed`.

## openmarket

[RPT-REQ-20261108-06.md](RPT-REQ-20261108-06.md) är en statusrapport om ett tidigare återgivet säkerhetsbesked för fyra exakta SHA. Den godkänner inte aktuell HEAD och inte lansering. Granskningsbeslutet är `unreviewed`.

[RPT-REQ-20261108-15.md](RPT-REQ-20261108-15.md) är BLOCKERAD. Ingen färdig fyndchecklista finns.

[RPT-REQ-20261108-16.md](RPT-REQ-20261108-16.md) är BLOCKERAD. Inga färdiga testfall finns.

[RPT-REQ-20261108-18.md](RPT-REQ-20261108-18.md) är en partiell openmarket-status. Sex roller väntar fortfarande på egna svar. Filen ersätter inte `REQ-20261108-18-vistion.md`, `REQ-20261108-18-vanprojekt.md`, `REQ-20261108-18-25design.md` eller `REQ-20261108-18-lampsajt.md`.

## Smart hem och UX

[RPT-REQ-20261108-14.md](RPT-REQ-20261108-14.md) är en färdig dokumentinventering. Granskningsbeslutet är `unreviewed`. Manifestets SHA-256 är en filhash, inte en Git-SHA. Ingen hubbstyrning och ingen ny research.

[RPT-REQ-20261108-20.md](RPT-REQ-20261108-20.md) är en statisk UX-lucklista mot `67feeb9f672cd76aad56f2db19d850df37b210b7`. Inget är kört. Den är inte runtime-acceptans. Den enda identifierade implementationsluckan i listan är L1. Granskningsbeslutet är `unreviewed`. Rapportens nästa åtgärd är inte en startorder för rapporten själv.

Leveransrapporter saknas fortfarande för 07, 08, 17 och 21. REQ-20261108-21 skapas inte här.
