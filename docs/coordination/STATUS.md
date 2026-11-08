# Läge

Ögonblicksbild 8 november 2026 (Europe/Stockholm). Läs om Git och jämför fullständig SHA och commit-tid innan du använder innehållet. Ingång: [README.md](README.md). Märkningar: [README.md](README.md#markningar).

Texten samlar Davids överlämning samma dag. Prototyp-repot lästes inte om när filen skrevs. Molnets egen testrapport är inte ett oberoende godkännande och inte ett skäl att säga att arbetet är klart.

## Git för prototypen

Källa för grenen och PR-länken: [PROJECTS.md](PROJECTS.md). Fullständiga SHA:

| Vad | SHA | Märkning |
| --- | --- | --- |
| Förälder till timeout-committen | `0a7c1baa5e848f5bc1ef4691f581bda85438c93a` | Verifierat tidigare |
| Timeout-commit på prototypgrenen | `abaaaeae0cbe9e88f2d6a7ca3053f2cc961d8fe9` | Verifierat tidigare |
| Rapporterad integrations-HEAD | `40d3529cece4832cb540c6f2229eeb53890a1cbf` | Rapporterat |

Verifierat tidigare, för timeout-committen `abaaaeae0cbe9e88f2d6a7ca3053f2cc961d8fe9`:

- Föräldern är `0a7c1baa5e848f5bc1ef4691f581bda85438c93a`.
- Historiken skrevs inte om.
- Timeout har standard 300 sekunder och gränser 30–900 sekunder.
- Onödiga workspace-bilder utelämnades.
- Avbrott och svenska väntestatusar ingår.
- Befintlig startsyntax ändrades inte av den committen.

Rapporterat av 25 Designs projektledare omkring 20:22 Europe/Stockholm, inte omkontrollerat här:

- Integrations-HEAD `40d3529cece4832cb540c6f2229eeb53890a1cbf`.
- Förälder `abaaaeae0cbe9e88f2d6a7ca3053f2cc961d8fe9`.
- Pushen var fast-forward.
- PR är öppen och inte sammanslagen.

## Mål och rapporterat beteende

Målet som David godkänt står i [PROJECTS.md](PROJECTS.md). Det är riktning, inte ett intyg att HEAD redan uppfyller allt.

Rapporterat beteende för integrations-HEAD:

- `/tv` visar en simuleringsintro och går sedan till punkten.
- Punkten har status, stopp och en cirkel eller tom graf.
- `/skriv` använder samma session i minnet som `/` och `/tv`. Ingen beständig lagring.
- Grafen byggs från skript, validerade rumsfält och workspace. Den är inte full automatisk semantisk förståelse av samtalet.
- Rumsvalidering: mood som enum, antal personer 0–20, högst 8 objekt.
- En misslyckad eller avbruten tur ersätter inte kartan.
- Navigering bort avbryter förfrågan.
- Ändringen inför inte ny mikrofon, kamera, styrning, lagring eller nätverksklient.

Lucka: målet om ett träd som växer med mer samtal och information är vidare än den rapporterade grafen från skript och validerade fält.

## Tester

Rapporterat av den implementerande körningen, inte oberoende godkänt:

- backend: 55 godkända.
- demo: 8 godkända.
- surface: 5 godkända.
- session: 12 godkända.
- Typkontroll och bygge: godkända.
- Miljön är moln med mock, inte Davids dator och inte den lokala 7B-modellen.

Verifierat tidigare: ett genomgånget transkript visade godkänt backend-test och bygge före de sista grafändringarna. Det intyget omfattar inte det sista grafsteget.

Att ledaren sedan rapporterar att de slutliga testerna passerar är rapporterat. Skärmbilder finns enligt ledaren. Visuell kvalitet är ogranskad.

## Oberoende granskning

Enligt källa. 25 Designs Säkerhet och 25 Designs Testare är var för sig tilldelade hela intervallet från `0a7c1baa5e848f5bc1ef4691f581bda85438c93a` till `40d3529cece4832cb540c6f2229eeb53890a1cbf`. Beslut och resultat saknas.

Båda ska verifiera att start motsvarar befintligt Ollama-läge, med fil och rad i prototyp-repot. Fil och rad återges inte här. De ska läsas i källan.

Känt historiskt startkommando, oförändrat av timeout-committen: `bash start.sh --assistant-model --assistant-ollama-model qwen2.5vl:7b` med Python 3.13 på PATH. Det är inte ett nytt slutligt kommando för den här leveransen. `DISABLE_CAMERA=1 bash start.sh` är inte en verifierad motsvarighet.

David väntar på den oberoende granskningen och på slutliga kommandon innan pull. En självgranskning från molnkörningen räcker inte för att kalla leveransen klar.

## Specialister i 25 Design

Källa för avsnittet: rollernas egna statusar, samlade i överlämningen. Märkningen är rapporterat där inget annat står. Ingen av statusarna har oberoende kontrollerats här.

### Utveckling

Rollen är skapad. Ingen egen levererad kod, inget eget test och inget eget uppdrag. Koden kommer från ledflödet.

### UX

Ingen egen koncepttext, granskning eller test ännu. VISTION-konceptet är inte UX-acceptans.

### Testare

Inga egna körda tester ännu. Granskningen av intervallet ovan är tilldelad. Resultat saknas. Ingen direktåtkomst till Davids dator.

### Säkerhet

Granskningen omkring 15:11 Europe/Stockholm gällde bara Smart hem R3: dokument, schema och fixturer.

- 35/35 manifestfil-hashar.
- 7 fasta hashvektorer.
- 7 schemakontroller.
- 93/93 deklarerade formulärutfall.

Normativt dokumentgodkännande gäller B1–B4 och M1. Det är inte godkännande av körning, start, driftsättning eller prototypkod.

Rapporterat fynd: `result.schema` överaccepterar `parse_invalid` med normal `action` och `target`, i strid med null-regeln. Separat värdvalidering krävs. Olöst: atomicitet, nyckelmäklare (key broker), tid, anti-rollback, retention och körningsbevis.

Prototypgranskningen är väntande och är ett annat uppdrag än R3-dokumenten.

### AI och röst

Linux-toy omkring 1 MB. Det är inte 7B och inte Davids dator.

- R2-schema: 16 negativa fall avvisades.
- Flyttal, positiva: 6/7. Exakta decimaler: 7/7.
- Grammatiken i Ollama 0.12.3 och llama.cpp ignorerar decimalintervall och `multipleOf`.
- 13/300 toy-utdata var ogiltiga.
- Förslaget heltal plus förtydligande: 300/300 schemagiltiga. Det bevisar inte meningsfullt eller säkert beteende.
- Inga STT-tester och inga latenstester för 7B på Davids dator.

CPU-llama.cpp som huvudväg är ett förslag från specialist och ledare. Det är inte ett godkännande att ersätta den Ollama-väg som redan fungerar.

### Smart hem

Research och kontrakt R1–R3. Ingen implementerad mapper, gateway, fejkad adapter, riktig hubb eller automation.

- Hue: officiella lokala HTTPS- och push-vägar är dokumenterade. Exakt hårdvara, autentisering, certifikat och sensorexport är ogranskade.
- DIRIGERA: officiell Matter-brygga.
- Inget publikt IKEA REST-kontrakt hittades. Det är inte ett bevis för att inget kontrakt finns.
- Ett odokumenterat community-API som stänger av certifikatkontroll är blockerat och ska inte användas.
- PARASOLL: export från Matter till Home Assistant är ogranskad.
- FP1E är närvaro, inte dörrkontakt.
- Förslag: lokal 7B ger avgränsade heltalsförslag, ber om förtydligande eller avstår. En separat valideringsgateway står emellan. Sensorregler är deterministiska och utan LLM.
- Hårdvaruinventering är okänd.

Allt detta är dokumentnivå. Det är inte ett bygge och inte kontakt med hubb.

## Andra artefakter

Rapporterat och ogranskat. Ett infrastrukturpaket M1 samt ett opublicerat utkast M0 och M1 är inte installerade och ligger inte i prototypens Git. Publicering väntar på David. Dokumentgodkännandet av de normativa texterna B1–B4 och M1 är inte detsamma som att paketet eller utkastet är installerat. Blanda inte ihop dem med TV-prototypen, flytta dem inte och lansera dem inte.

## Lokal arbetsstation

Enligt källa, David. Maskinprofil och privat projektsökväg är utelämnade eftersom HOPESI är publikt. David ger dem i den lokala chatten när en inventering är godkänd. De ska inte skrivas tillbaka hit.

- David har bekräftat lokala rutter: `http://127.0.0.1:5173/` med `/skriv` och `/tv`, samt `http://127.0.0.1:8787/health` med `assistant_mode` ollama.
- Historiskt startkommando: se avsnittet om oberoende granskning. Inget nytt slutkommando är godkänt.
- Ollama 0.12.3 står sida vid sida med en äldre 0.40.15. Endpoint `127.0.0.1:11434`. Modell `qwen2.5vl:7b`, Q4_K_M, omkring 6 GB.
- Direkt text-API svarade 200 efter 127 sekunder.
- En tidigare UI-fråga med onödiga bilder fick timeout efter 121 sekunder. Det är inte ett bevis för att modellen är trasig.
- David har bekräftat att punktgrafens demo fungerade.
- Bevara befintlig klon, virtuell miljö, `node_modules` och Ollama. En första opencv-byggnad tog 55 minuter. Undvik ominstallation.
- Enligt källa har bottarna inte direktåtkomst till Davids dator. Påstå inte att den finns.

När David senare, efter granskningen, ber om uppdatering på datorn gäller [WORKFLOW.md](WORKFLOW.md). Gör inte det steget från den här ögonblicksbilden.

## Inte godkänt

Ny kamera, ny mikrofon, hemkontroll, kontakt med hubb, beständig lagring, kostnader, debitering, produktion, sammanslagning, driftsättning, force, rebase, reset, amend, historikomskrivning och juridiska åtaganden. Inte heller pull, ominstallation, omstart eller grenbyte förrän granskningen är klar och David ber om nästa steg.
