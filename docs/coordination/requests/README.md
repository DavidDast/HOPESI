# Förfrågningar

Första ögonblicksbilden 8 november 2026 (Europe/Stockholm) lämnade katalogen tom. Det gäller den incheckningen. Tillägget samma kväll, omkring 21:23–21:25, är det här indexet.

Ingång: [../README.md](../README.md). Mall: [../REQUEST-TEMPLATE.md](../REQUEST-TEMPLATE.md). Flöde: [../WORKFLOW.md](../WORKFLOW.md). Rapporter: [../reports/README.md](../reports/README.md).

En fil här väcker ingen agent, startar ingen körning och ger ingen rätt utöver den text David redan godkänt för just den filen. Skrivrätt i HOPESI ger inte rätt till appkod eller till att skicka meddelanden. Ingen pollning läser katalogen.

## Lägesord

| Ord | Betydelse |
| --- | --- |
| `proposed` | Förslag i mallen. Inte de här uppdragen. |
| `awaiting-status` | Smalt textuppdrag godkänt. Utförande inte bekräftat. Inte klart. |
| `partial` | En del statussvar inne. Inte klart. |
| `blocked` | Leverans inte startad. Källa saknas. Inte klart. |
| `completed` | Används inte. |

## Prominens 21:25

REQ-20261108-18 är `partial`. VISTION 10–13 är `blocked` före start. Inget av 07–17 är klart. openmarket har inget svar.

## Index

| ID | Projekt och roll | Status | Förfrågan | Rapport |
| --- | --- | --- | --- | --- |
| REQ-20261108-07 | 25 Design, Säkerhet | `awaiting-status` | [07](REQ-20261108-07.md) | Ingen leverans. [Ledstatus](../reports/REQ-20261108-18-25design.md) |
| REQ-20261108-08 | 25 Design, Testare | `awaiting-status` | [08](REQ-20261108-08.md) | Ingen leverans. [Ledstatus](../reports/REQ-20261108-18-25design.md) |
| REQ-20261108-09 | 25 Design, AI och röst | `awaiting-status` | [09](REQ-20261108-09.md) | Ingen leverans. [Ledstatus](../reports/REQ-20261108-18-25design.md) |
| REQ-20261108-10 | VISTION, Idéer och research | `blocked` | [10](REQ-20261108-10.md) | Ingen leverans. [VISTION-status](../reports/REQ-20261108-18-vistion.md) |
| REQ-20261108-11 | VISTION, UX och visualisering | `blocked` | [11](REQ-20261108-11.md) | Ingen leverans. [VISTION-status](../reports/REQ-20261108-18-vistion.md) |
| REQ-20261108-12 | VISTION, Testare | `blocked` | [12](REQ-20261108-12.md) | Ingen leverans. [VISTION-status](../reports/REQ-20261108-18-vistion.md) |
| REQ-20261108-13 | VISTION, Säkerhet och integritet | `blocked` | [13](REQ-20261108-13.md) | Ingen leverans. [VISTION-status](../reports/REQ-20261108-18-vistion.md) |
| REQ-20261108-14 | 25 Design, Smart hem | `awaiting-status` | [14](REQ-20261108-14.md) | Ingen leverans. [Ledstatus](../reports/REQ-20261108-18-25design.md) |
| REQ-20261108-15 | openmarket, Auth och data | `awaiting-status` | [15](REQ-20261108-15.md) | Ingen |
| REQ-20261108-16 | openmarket, Testare | `awaiting-status` | [16](REQ-20261108-16.md) | Ingen |
| REQ-20261108-17 | Lampsajt, Testare | `awaiting-status` | [17](REQ-20261108-17.md) | Ingen leverans. [Delstatus](../reports/REQ-20261108-18-lampsajt.md) |
| REQ-20261108-18 | Alla roller utan verifierat läge | `partial` | [18](REQ-20261108-18.md) | [VISTION](../reports/REQ-20261108-18-vistion.md), [Vänprojekt](../reports/REQ-20261108-18-vanprojekt.md), [25 Design](../reports/REQ-20261108-18-25design.md), [Lampsajt](../reports/REQ-20261108-18-lampsajt.md) |
| REQ-20261108-19 | Första kontakt | `awaiting-status` | [19](REQ-20261108-19.md) | Gemensam rätt att påbörja redan skriven omfattning och pusha |
| REQ-20261108-20 | 25 Design, UX | `awaiting-status` | [20](REQ-20261108-20.md) | Startar lucklistan i 03. Bara rapport |
| REQ-20261108-21 | 25 Design, Utveckling | `awaiting-status` | [21](REQ-20261108-21.md) | Kodpush bara efter lucklistan. Ingen merge |
| REQ-20261108-22 | 25 Design, AI och röst | `awaiting-status` | [22](REQ-20261108-22.md) | Procedur. Den igångsatta Ollama är inte provet av 67feeb9 |

## Loggade utan start

REQ-20261108-06 är inte startad. 03 påbörjas genom 20. 04 påbörjas genom 21 först när lucklistan finns. 05 påbörjas inte.

| ID | Projekt och roll | Status | Förfrågan | Start |
| --- | --- | --- | --- | --- |
| REQ-20261108-03 | 25 Design, UX | `proposed` | [03](REQ-20261108-03.md) | Påbörjas genom 20. Bara en lucklista. |
| REQ-20261108-04 | 25 Design, Utveckling | `proposed` | [04](REQ-20261108-04.md) | Kod bara genom 21, efter lucklistan. Ingen merge. |
| REQ-20261108-05 | 25 Design, AI och röst | `proposed` | [05](REQ-20261108-05.md) | Ska inte startas. Smutsig kopia. Proceduren är 09 och 22. |
| REQ-20261108-06 | openmarket, Säkerhet | `proposed` | [06](REQ-20261108-06.md) | Inte startad. Bara läge för en redan begärd granskning. Ingen SHA är påhittad. |
