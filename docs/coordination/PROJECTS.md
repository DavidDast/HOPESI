# Projekt

Ögonblicksbild 8 november 2026 (Europe/Stockholm). Läs om Git och jämför SHA innan du använder innehållet. Ingång: [README.md](README.md). Märkningar: [README.md](README.md#markningar).

Ingen ny kod-, lanserings- eller driftkontroll gjordes när den här texten skrevs. Blanda inte ihop repon. HOPESI tar inte emot appkod och är inte en order att kopiera prototypen hit.

## 25 Design

Enligt källa. Prototypens källrepo är [DavidDast/25Project](https://github.com/DavidDast/25Project), grenen `cursor/camera-tv-prototype-d4f4`, PR [https://github.com/DavidDast/25Project/pull/1](https://github.com/DavidDast/25Project/pull/1). Grennamn och PR-länk är angivna i uppdraget. Att PR:en var öppen och osammanslagen omkring 20:22 är rapporterat, inte nykontrollerat här. Git-läget och SHA-värden står i [STATUS.md](STATUS.md).

David har godkänt en enda integrerad prototyp: bygga, testa och pusha den.

- `/tv` är Rum-TV och visar perception med tydlig markering att det är en simulering.
- Övergången landar i punkten på `/`.
- Mer samtal och information vecklas ut till ett cirkulärt ämnes- och informationsträd.
- `/skriv` delar session med `/` och `/tv`.
- Grafen visar observationer, ämnen, källor och osäkerhet, och visar inte privat resonemang.
- Manusstyrd demo och faktisk modellutdata hålls isär.
- Riktig hemassistent ligger senare. Visuell integration är inte den assistenten.

Enligt källa hör `docs/index.html` på `main` till den separata lampbutiken. Ändra inte den filen för prototypen.

Enligt källa har den rapporterade prototypkoden tagits fram i 25 Designs ledflöde. Den fristående rollen Utveckling har inte levererat egen kod. VISTION stöder med koncept och ska inte öppna en konkurrerande kodlinje. Roller: [ORGANIZATION.md](ORGANIZATION.md).

## Lampsajt

Enligt källa. Egen butik och egen lansering, skild från TV-prototypen. Namngivet sortiment: Bark, BlackEk och ALM1OF1. Områden som hör till ledaren: priser, betalningar, order, lager, frakt, villkor, hosting och domän. Inga prisuppgifter står här.

Framtida inbäddad AI för butiken är ett separat spår, inte den här prototypen. Enligt källa finns ingen verifierad lansering från CI eller förhandsvisning. Produktion behöver egen verifiering. Debitering kräver särskilt godkännande från David. Den här ögonblicksbilden har ingen ny livestatus.

## openmarket

Enligt källa. Repo [DavidDast/openmarket](https://github.com/DavidDast/openmarket), TypeScript. Funktionen Bevakningar ska vara komplett, testad och ingå i första releasen. Lansering, pipeline och krav ägs av den projektledaren. Ingen ny kod- eller lanseringskontroll gjordes här. Bevakningar i openmarket är en produktfunktion, inte en bevakningstjänst för Git.

## Vänprojekt Avtal

Enligt källa. Teknisk omfattning och avtal är inte bekräftade. Procentsatser som har nämnts för start och leverans är förslag, inte ett etablerat avtal. Siffrorna står inte i det här publika repot. Skapa inga juridiska åtaganden och skriv inget avtal här.

## VISTION

Enligt källa. Idé- och konceptresearch, med ett delat visuellt träd som inspiration. Ett första koncept finns. Det är inte kod och inte test. Implementation hör till 25 Design. Ingen egen ny kodsatsning ska startas från VISTION. Genomgång av idéer beskrivs i [ORGANIZATION.md](ORGANIZATION.md).

## HOPESI

Det här repot, [DavidDast/HOPESI](https://github.com/DavidDast/HOPESI). Koordinering, förfrågningar och rapporter. Inte prototypen, inte butiken, inte openmarket och inte ett avtal. Arbetsflöde: [WORKFLOW.md](WORKFLOW.md).

## Stående avgränsning

- Prototypändringar hör hemma i 25Project på prototypgrenen, efter godkännande och granskning.
- Lampbutikens `docs/index.html` på `main` lämnas orörd av prototyparbetet.
- Butik, betalning, lager och lansering stannar hos Lampsajt.
- openmarket ändras inte från ett 25 Design-uppdrag.
- VISTION skriver inte en parallell implementation.
- Opublicerade utkast och infrastrukturpaket som nämns i [STATUS.md](STATUS.md) flyttas inte, publiceras inte och behandlas inte som prototypen.

## Tillägg 8 november 2026 omkring 21:25

Den första projekttexten står kvar. Senare källor:

- Prototypens senare rapporterade SHA är `67feeb9f672cd76aad56f2db19d850df37b210b7` på `cursor/camera-tv-prototype-d4f4`. Den överspelar `40d3529cece4832cb540c6f2229eeb53890a1cbf` som aktualitet. Inte nykontrollerad här. Se [STATUS.md](STATUS.md).
- Lampsajtens granskade commit enligt ledaren är `ec5b0a7c59891e0b8657977b774f0a382a0da942`, PR https://github.com/DavidDast/25Project/pull/2. Grennamn är inte angivet. Publicering är inte godkänd.
- openmarket har fortfarande ingen exakt gren eller SHA i den här loggen.
- VISTION-konceptet har ingen etablerad Git-SHA. Ingen intern adress publiceras. Uppdrag 10–13 är blockerade.
- Vänprojektets repo, gren och SHA är okända. All teknik är ostartad.
