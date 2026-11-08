# Mall för rapport

Ögonblicksbild 8 november 2026 (Europe/Stockholm). Ingång: [README.md](README.md). Flöde: [WORKFLOW.md](WORKFLOW.md). Förfrågan: [REQUEST-TEMPLATE.md](REQUEST-TEMPLATE.md).

Kopiera blocket när ett arbete faktiskt har utförts. En rapport är en logg över vad som gjordes, vad som testades och vad som inte testades. Den väcker ingen agent och är inte ett godkännande av nästa steg.

Skriv filen till [reports/](reports/README.md) bara om David har godkänt just den skrivningen och remote är verifierat som `DavidDast/HOPESI`. Annars ge David den kopierbara texten.

Namnförslag när en fil väl ska skapas: `reports/RPT-` plus förfrågans id och `.md`. Skapa ingen sådan fil i förväg.

SHA är den commit som arbetet faktiskt gällde, fullständig. Miljö är den miljö som användes, utan maskinidentifierande detaljer och utan hemligheter om rapporten ska till det publika repot. Sådana detaljer stannar i Davids lokala chatt.

Granskningsbeslutet `unreviewed` betyder att rapporten inte själv förklarar arbetet godkänt.

```text
Källförfrågan: (ID och sökväg eller chatthänvisning)
Miljö: (var arbetet gjordes, utan hemligheter och utan maskinprofil om texten ska in i HOPESI)
Exakt SHA: (40 tecken för det repo som ändrades eller lästes; ange också repo och gren)
Faktiska ändringar: (vad som ändrades, eller att inget ändrades)
Tester: (kommandon och resultat som faktiskt kördes)
Tester som inte kördes: (sådant som skulle vara relevant men inte kördes, och varför)
Bevis: (loggar, utdata eller filhänvisningar som får visas publikt)
Fynd: (vad som observerades, med märkning)
Gränser: (vad rapporten inte visar och vilken miljö den inte täcker)
Granskningsbeslut: unreviewed
Nästa åtgärd: (förslag till David; inte en startorder)
```

Ett granskningsbeslut får bytas från `unreviewed` bara när den oberoende granskaren faktiskt har bedömt underlaget. Implementerarens egen körning sätter inte beslutet till godkänt. Nästa åtgärd utförs inte förrän David sagt till i chatten.
