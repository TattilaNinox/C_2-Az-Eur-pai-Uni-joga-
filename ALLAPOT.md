# C/2 Az Európai Unió joga – állapot

A rend: `orlomed_admin_web/docs/szakvizsga_program/12_tetelsor_szabvany.md`. A központi chat vezeti (Attila döntése, 2026-11-19, `01_dontesek.md`).

## 2026-11-19 – előkészítés indul (ág: `elokeszites-2026-11-19`)

- **Kiírás:** `tetelsor/C2_kiiras_2026.pdf`, szövege: `tetelsor/kiiras_2026.txt` (Attilától, 2026-11-19).
- **Korpusz-felmérés (első, gépi; `jelentesek/korpusz_felmeres.md`):** `korpusz_felmeres: forrás 101, megvan 96, hiányzik 5, nem hivatkozott korpuszfájl 16`
- **Szakaszok:** S0 – kész (2026-11-19: közös eszközök szinkronban, `tetelsor/beallitas.json`); S1 – kész (2026-11-19: alapfelvétel `hiba 0`, munkaszöveg `eltérés 0`; a cikkre tagolt joganyag miatt a doboz- és lefedettség-ellenőrzés nem értékelhető, l. Központi teendő); S2 – a felmérés kész, a hatályossági összevetés (2026. december 9. utáni állapot) nem indult.

## S0–S1 (2026-11-19)

A tételszám 43 (a kiírás 1–43. tétele és a `jegyzetek/manifest.json` sorszámai 1..43; a korpusz-felmérés „tétel: 42” sora elszámolás, az alapfelvétel 43 tételt talál). Fő kódex: EUMSZ, `egyseg: cikk`.

Programok utolsó sora (szó szerint):

- `eszkoz_ellenor: fájl 63, eltérés 0`
- `alapfelvetel: tétel 43, feloldott 200, feloldatlan 2, hiba 0`
- `jegyzet_txt: tétel 43, rész 131, karakter 4688351, eltérés 0`
- `ellenorzes.py | tail -1`: `hiányos bekezdés: 0`; összegző sora: `dobozok: 3, eltérés: 0; hiányzó forrás: []; lefedettségi hiány: 197 elem 41 tételben`
- `doboz_teljesseg.py | head -1`: `hiányos bekezdés: 0`

**Valódi hiánylista:** nincs. A kiírás minden megnevezett forrása megvan a korpuszban. A két feloldatlan sor (1. és 11. tétel: „a kiírásban nincs feloldható hivatkozás”) nem hiány: e két tételhez a kiírás nem ír elő forrást (az EUSZ és az EUMSZ átfogóan előírt, `atfogo: true`).

**`kiirasElirasok` indokai:**

- `kihagy: 95/46/EK` – a 42. tételben a GDPR címének része („a 95/46/EK rendelet hatályon kívül helyezéséről”), hatályon kívül helyezett irányelv, nem önálló előírás (a kiírás „rendelet”-nek is írja).
- `megfeleltet: C-141/04 → C-144_04 Mangold-ügy.txt` – a Mangold-ügy száma C-144/04; a kiírás elírása (19. tétel).
- `megfeleltet: C-48/93 → C-46_93 Brasserie du Pêcheur-ügy.txt` – a C-46/93. és C-48/93. sz. egyesített ügyek ítélete egy fájl (26. tétel).
- `megfeleltet: C-26/83 → C-286_82 Luisi és Carbone egyesített ügyek.txt` – a 286/82. és 26/83. sz. egyesített ügyek (38. tétel).
- `megfeleltet: C-416/93 → C-358_93 Bordessa és társai egyesített ügyek.txt` – a C-358/93. és C-416/93. sz. egyesített ügyek (38. tétel).

**A beállítás kiírás-specifikus mintái (forrasok):** az EUMSZ második mintája a 16. tétel előtag nélküli „288. cikk” hivatkozását köti az EUMSZ-hez (a 13–15. és 17. tétel ugyanezt „EUMSZ 288. cikk”-ként írja). A 45/2001/EK rendelet azért forrás, mert a kiírás cikkre hivatkozik (7. tétel: 41–48. cikk). Az általános mód (`hatarozatMod: altalanos`) nem ismerte fel, ezért `forrasok`-ként (tipus megjelöléssel, teljes fájl) szerepel: „C-13-24/66. sz. Kampffmeyer ügy” (27.; korpusz: 5_7-24_66 Kampffmeyer egyesített ügyek), „Európai Bíróság 2/94. sz. és 2/13. sz. véleménye” (20.), „3/2005. (XI. 14.) LB PK-KK közös vélemény”, „1/2009. (VI. 24.) LB PK-KK közös vélemény”, „Legf. Bír. Kfv. I. 35.055/2007. (EBH 2008/1/1815)” (25.; korpusz: EH 2008.1815), a 43. tétel két ismertetője (EP-ismertető Energiapolitika, Consilium éghajlatváltozás). Ezek nélkül a 20., 25., 27. és 43. tétel forrásai csendben kimaradtak volna (sem feloldott, sem feloldatlan sorként nem jelentek meg).

**Kiinduló számok értelmezése:** a 197 lefedettségi hiány gépi műtermék, nem tartalmi hiány (89 „a tartomány határa nincs a korpuszban” – minden cikk-tartomány; 108 „a jogszabály nincs a korpuszban” – minden teljes fájlként előírt EUB-ügy, rendelet, AB-határozat). A 3 felismert doboz a 25. tétel két Pp. 130. §- és egy Be. 490. §-doboza; a jegyzetek ~437 dobozából ~360 cikkfejlécű (EUMSZ, EUSZ, GDPR, Alapjogi Charta, 45/2001/EK, 1/2003/EK, 2005/36/EK, 98/5/EK), ezeket a közös eszköz nem ismeri fel.

## A közös készlet KE-1 javítása után (2026-11-19, központi chat)

- `alapfelvetel: tétel 43, feloldott 199, feloldatlan 3, hiba 0`
- `dobozok: 408, eltérés: 91; hiányzó forrás: []; lefedettségi hiány: 1 elem 1 tételben`
- `hiányos bekezdés: 183`
- A korábbi „Központi teendő” pontok közül a hivatkozásfeloldás, a cikk-egység és a vegyes számozás javítva (admin-commit `d1c2925`). Az új feloldatlan sorok a maradékvizsgálatból jönnek (`jelentesek/alapfelvetel.md`): beállítást kérnek (`kiirasElirasok`), nem korpuszhiányt jelentenek.

## Attila teendői

## Központi teendő

A közös eszköz cikkre tagolt joganyagnál (S0–S1, 2026-11-19; a C/2-ben nem foltoztam):

1. `kozos.py`, `FEJLEC` (76. sor): a dobozfejléc-minta kötelezően `§`-ra végződik (`…PAR + r'\.\s?§'`), ezért az „EUMSZ 223. cikk”, „EUSZ 17. cikk”, „GDPR 5. cikk”, „Alapjogi Charta 1. cikk” fejlécű dobozokat a `kozos.dobozok`, az `ellenorzes.py` és a `doboz_teljesseg.py` nem látja (C/2: 3 doboz felismerve a ~437-ből). Javaslat: a `dobozRovidites` mellé egységet (`§`/`cikk`) adni, és a FEJLEC-et forrásonként `\.\s?§` vagy `\.\s*cikk` végződéssel építeni. A „2005/36/EK irányelv (1) preambulumbekezdés” alakú fejlécre (36 doboz) külön szabály kell.
2. `kozos.py`, `jogszabaly_paragrafusok` / `korpusz_jogszabalyok`: a korpuszt csak `^N. §` sorokra bontja; cikkre tagolt fájlból (EUMSZ, EUSZ, Charta, rendeletek) üres szótár lesz → `ellenorzes.py` 3. lépése minden cikk-tartományra „a tartomány határa nincs a korpuszban” (C/2: 89 elem). Javaslat: az `alapfelvetel.egyseg_index` cikk-szabályának (`^(\d+)\. cikk\b`, re.I) átvétele.
3. `ellenorzes.py`, lefedettség: az `alapfelvetel.py` minden előírásnál `'tol': None` kulcsot ír, ezért a teljes fájlként előírt forrás (EUB-ügy, rendelet, AB-határozat) az első ágba fut, és „a jogszabály nincs a korpuszban” hiányként jelenik meg (C/2: 108 elem). Javaslat: `e['tol'] is None` → a „teljes” ág (a tétel említi-e).
4. `kontroll.py`, `ptk_parok` és a norma-ellenőrzés (≈365. sor): „normánál a korpusz-§ kötelező”, a §-szám ellenőrzése `\.\s?§` mintával – cikkes normánál minden tétel hibát adna; `kontroll.paragrafusForrasok: ["EUMSZ"]` most üres halmazt ad. Az `elhatarolasPar` cikkes alakra (`EUMSZ \d+\. cikk`) állítva; az `elhatarolas_gyart.py` csak `findall`-t futtat vele, ez működik, de a további §-feltételezéseit nem vizsgáltam.
5. `korpusz_felmeres.py`, `valaszt` (az `alapfelvetel.hatarozatok_altalanos` hívja): több egyező fájlnál a névsor szerinti elsőt adja, ezért rossz fájl kerül a tételbe: C-106/89, C-12/86, C-374/87, C-5/88, C-344/87 → a „tárgyalási jelentés” fájl az ítélet helyett (az ítélet fájlja „nem hivatkozott” marad); C-583/11 → „C-583_11 Inuit Tapiriit Kanatami fellebbezés.txt” a „C-583_11 P Inuit Tapiriit Kanatami-ügy.txt” helyett; T-18/10 → szintén a fellebbezés fájlja (első sorában szerepel a T-18/10), a „T-18_10 Inuit Tapiriit Kanatami végzés (EN).txt” helyett. A `kiirasElirasok.megfeleltet` ide nem alkalmazható (nem elírás). Javaslat: EUB-kulcsnál minden egyező fájl felvétele, vagy a fájlnévbeli ügyszám elsőbbsége az első sorbeli előtt és az ítélet elsőbbsége a tárgyalási jelentés előtt.
6. `korpusz_felmeres.hivatkozasok`: nem ismeri fel a „C-13-24/66. sz.”, a „2/94. sz. … véleménye”, az „LB PK-KK közös vélemény” és a „Legf. Bír. Kfv. … (EBH …)” alakot; a fel nem ismert hivatkozás feloldatlanként sem jelenik meg (csendes kimaradás). C/2-ben `forrasok`-mintával pótolva.
7. `alapfelvetel.felold`, cím: a GDPR-hivatkozás (42. tétel) a tételcímben marad („Az adatkezelési elvek és az érintett jogai A természetes személyeknek …”), mert a cím csak `forrasok`-minta vagy „(PK|MK|szám/év” előtt vág.
