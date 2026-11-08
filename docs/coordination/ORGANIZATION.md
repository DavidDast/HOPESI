# Organisation

Ögonblicksbild 8 november 2026 (Europe/Stockholm). Läs om Git och jämför SHA innan du använder innehållet. Ingång: [README.md](README.md). Märkningar: [README.md](README.md#markningar).

Enligt källa. Trädet är en dirigeringskarta som David angett. Det är inte en kontroll att varje roll är bemannad eller har pågående arbete. En skapad roll är inte aktivt arbete. Produktens informationsträd är ett annat träd och beskrivs i [PROJECTS.md](PROJECTS.md).

```
David
└── Första kontakt (intag och koordinering)
    ├── 25 Design
    │   ├── Utveckling
    │   ├── UX
    │   ├── AI och röst
    │   ├── Smart hem
    │   ├── Testare
    │   └── Säkerhet
    ├── VISTION
    │   ├── Idéer och research
    │   ├── UX och visualisering
    │   ├── Utveckling
    │   ├── Testare
    │   └── Säkerhet och integritet
    ├── Lampsajt
    ├── openmarket
    └── Vänprojekt Avtal
```

Första kontakt tar emot ett ärende och mappar det till en befintlig projektledare. De fem projektledarna är separata. Första kontakt uppfinner inte ett sjätte projekt. Lampsajt, openmarket och Vänprojekt Avtal har projektledare. Inga specialistroller är angivna för dem i den här kartan, och inga ska läggas till här utan att David angett dem.

Projektledaren äger prioritering av implementation. Specialisten äger den omfattning som blivit tilldelad. Oberoende test och oberoende säkerhet är skilda från den som implementerar.

## Vem som bygger prototypen

Enligt källa. Den rapporterade prototypkoden har tagits fram i 25 Designs ledflöde, en kodkörning i molnet. Rollen Utveckling under 25 Design har inte levererat egen kod, eget test eller eget uppdrag. Läs rapporterat läge i [STATUS.md](STATUS.md).

VISTION-koncept stöder 25 Design. De är inte en konkurrerande implementation och inte ett UX-godkännande för prototypen.

## VISTION-genomgång

Enligt källa. Idéer gås igenom var tredje dag. Första tillfället som redan är planerat är 11 november 2026 omkring 19:56 Europe/Stockholm, plus eller minus 15 minuter. Rutinen finns redan på annan plats. Skapa inte en ny rutin och schemalägg inte ett ytterligare tillfälle härifrån. Inget i den här filen startar den genomgången.

## Dirigeringsexempel

Exemplen visar bara vart ett ärende skulle peka. De är inte uppdrag. Starta inget av dem för att det står här.

| Om ärendet handlar om | Peka mot |
| --- | --- |
| UX-specifikation för 25 Design | 25 Design, UX |
| Ett reproducerbart testfel | Testare i rätt projekt, med berörd projektledare |
| Modelljämförelse som kräver lokala körningar | 25 Design, AI och röst, och bara efter Davids godkännande av de lokala körningarna |
| Kompatibilitetsresearch för smart hem utan kontakt med hubb | 25 Design, Smart hem |
| Nya idéer | VISTION, Idéer och research |

Smart hem-research inkluderar inte kontakt med hubb, riktig styrning eller automation. Se [WORKFLOW.md](WORKFLOW.md) för vad som kräver Davids godkännande i chatten, och [REQUEST-TEMPLATE.md](REQUEST-TEMPLATE.md) för hur ett förslag skrivs. Status på ett nytt förslag är `proposed`.

## Tillägg 8 november 2026 omkring 21:25

Trädet ovan står kvar. Statussvar samma kväll namnger fler roller hos Lampsajt och Vänprojekt Avtal, och målroller för openmarket i REQ-20261108-15 och REQ-20261108-16. De står i [rapporterna](reports/README.md) och i [förfrågningarna](requests/README.md). De skrivs inte in i trädet som om de fanns i den första ögonblicksbilden. Inget nytt uppdrag skapas åt dem utöver de redan villkorade textuppdragen. VISTION Utveckling får inget nytt uppdrag.
