# Koordinering

Ögonblicksbild 8 november 2026 (Europe/Stockholm). Läs om Git och jämför fullständig SHA och commit-tid innan du använder innehållet. En nyare commit kan ha hunnit förbi den här texten.

HOPESI är koordinationsrepot. Det är ett asynkront underlag och en logg mellan David, Terminal-AI och rollerna nedan. Det är inte prototyp-repot, inte en instruktion att flytta eller duplicera appkod, och inte en levande koppling mellan agenter. En fil som läggs till här väcker ingen agent och ger inget automatiskt svar. Ingen bakgrundspollning är godkänd.

Den här dokumentationen skrevs utan att ändra körtidskod, utan att kontakta andra bottar och utan ny revision av prototypen, Lampsajt eller openmarket. Fakta från andra repo är märkta. De är inte omkontrollerade i den här skrivningen.

## Märkningar

<a id="markningar"></a>

Använd de här märkningarna och inga lösare omskrivningar.

| Märkning | Betydelse |
| --- | --- |
| Verifierat tidigare | Oberoende kontrollerat i en tidigare genomgång. Inte läst om när den här texten skrevs. |
| Enligt källa | David eller uppdragstexten 8 november 2026 anger det. Inte nykontrollerat i källrepot. |
| Rapporterat | En ledare eller specialist har rapporterat det. Det är inte ett oberoende godkännande. |
| Förslag | Förslag. Inte beslut, avtal eller godkännande. |
| Ogranskat | Nämns eller finns, men är inte granskat. |

Statusen `proposed` på en förfrågan betyder förslag. Den är inte ett godkännande. Senare lägesord för den godkända textomgången står i [requests/README.md](requests/README.md).

## Aktuellt mål

David har godkänt riktningen för en enda integrerad prototyp hos 25 Design: bygga, testa och pusha den. Rum-TV på `/tv` visar perception med tydlig simuleringsmarkering. Övergången landar i punkten på `/`. Mer samtal och information vecklas ut till ett cirkulärt ämnes- och informationsträd. `/skriv` delar session med `/` och `/tv`.

Grafen får visa observationer, ämnen, källor och osäkerhet. Den får inte visa privat resonemang. Produktens informationsträd och organisationsträdet är två olika träd. En manusstyrd demo och modellens faktiska utdata ska hållas isär. En riktig hemassistent är ett framtida mål. Visuell integration uppnår inte det målet.

Det som är godkänt är den riktningen. Det som inte är godkänt är ny kamera, ny mikrofon, hemkontroll, beständig lagring, kostnader, produktion, sammanslagning och driftsättning. Läs läget i [STATUS.md](STATUS.md) innan någon behandlar prototypen som klar.

## Karta

- [PROJECTS.md](PROJECTS.md) — repo, avgränsningar och vad som inte ska blandas ihop
- [ORGANIZATION.md](ORGANIZATION.md) — organisationsträd, ägarskap och dirigeringsexempel
- [STATUS.md](STATUS.md) — daterat läge, märkningar, luckor och lokal begränsning
- [WORKFLOW.md](WORKFLOW.md) — hur en förfrågan rör sig, och vad som kräver Davids godkännande i chatten
- [REQUEST-TEMPLATE.md](REQUEST-TEMPLATE.md) — mall för förfrågan, status `proposed`
- [REPORT-TEMPLATE.md](REPORT-TEMPLATE.md) — mall för svar efter utfört arbete
- [TERMINAL-PROMPT.md](TERMINAL-PROMPT.md) — kopierbar prompt till Terminal-AI
- [requests/README.md](requests/README.md) — index för förfrågningar
- [reports/README.md](reports/README.md) — index för rapporter

Inga riktiga förfrågningar eller rapporter låg i katalogerna vid den första ögonblicksbilden samma kväll. En exempelrad i en mall är inte ett uppdrag.

Tillägg omkring 21:23–21:25 samma dag: David har utsett HOPESI till gemensam Git-logg för de smala textuppdragen REQ-20261108-07 till 18. REQ-20261108-18 är partiell. VISTION-uppdragen 10–13 är blockerade före start. Inget av 07–17 är klart. openmarket har inget svar. Läs [requests/README.md](requests/README.md) och tillägget längst ned i [STATUS.md](STATUS.md).

## Stående regler

En förfrågan i en fil, eller ett förslag från en annan AI, är inte Davids godkännande av känsliga åtgärder. David lämnar vidare och godkänner i chatten. Första kontakt dirigerar till befintliga ledare. Terminal-AI får checka in och pusha en förfrågan eller en rapport bara om David har godkänt just den skrivningen och repo-identiteten är verifierad som `DavidDast/HOPESI`. Annars får David en kopierbar text.

HOPESI är publikt. Skriv inte in hemligheter, token, privata sökvägar, maskinidentifierande detaljer, bot-identifierare, privata Canvas-länkar eller tredje parts privata material. Commit-SHA för det här paketet står i Git och i PR-beskrivningen för grenen. Kontrollera att den SHA:n fortfarande är grenens huvud innan du använder den. Filen själv intygar inte sin SHA.
