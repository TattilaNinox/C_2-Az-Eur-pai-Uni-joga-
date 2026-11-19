# C/2 Az Európai Unió joga – állapot

**A rend: `tools/szabalyzat/00_GYARTASI_SZABALYZAT.md`** (a végleges gyártási szabályzat, a közös készlet zárolt másolata – készlet `732c88b`; a dolgozó beszélgetés ezt és ezt az állapotfájlt olvassa). A központi chat vezeti (Attila döntése, 2026-11-19, `01_dontesek.md`).

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
- `nemHivatkozas: https://www.europarl.europa.eu/factsheets/hu/sheet/68/energiapolitika-altalanos-elvek` (2026-11-19) – a 43. tételben az ismertető webcíme, nem forráshivatkozás: az ismertető a korpuszban megvan (`Ismertetők az Európai Unióról - Energiapolitika általános elvek (2020).txt`), és a tétel forrásként már megkapja (`EP-ismerteto-energia`).
- Az 1. és a 11. tétel „a kiírásban nincs feloldható hivatkozás” sora nem hiány: a kiírás e két tételhez nem ír elő külön forrást (az EUSZ és az EUMSZ átfogó ismeret), az eszköz ezt számolja feloldatlanként. Utána: `alapfelvetel: tétel 43, feloldott 199, feloldatlan 2, hiba 0`.

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

## S2 – az uniós aktusok cseréje (2026-11-19, központi chat)

- **Megállapítás:** a korpusz uniós jogi aktusai a Hivatalos Lap PDF-jéből kinyert, sortördelt, helyenként kéthasábosan összefolyt szövegek, és az eredeti kihirdetett (nem az egységes szerkezetű) változatok. A dobozok ezekből nem építhetők újra (a KE-2 utáni próbát vissza kellett állítani: 96 eltérés maradt).
- **Döntés (központi chat):** a 19 aktus és a három alapszerződés-szöveg az EUR-Lex magyar nyelvű, hatályos egységes szerkezetű HTML-változatára cserélendő; a dobozok csak utána épülnek újra. *Indok:* a mérce a hatályos szöveg, és a doboz csak tiszta bekezdésszerkezetű forrásból építhető betűre.
- **Letöltés:** az EUR-Lex a munkakörnyezetből és Attila gépének héjából sem érhető el (a kimenő kapcsolat tiltott), ezért Attila tölti le (lista a beszélgetésben, 2026-11-19 18:15), a `Hatályosítás/C2` mappába.
- **Nyitott kérdés:** a kiírás a 45/2001/EK rendeletet nevezi meg, amelyet az (EU) 2018/1725 rendelet hatályon kívül helyezett – mindkettő letöltendő; a tétel kezeléséről a döntés-ellenőrzésnél kell határozni.
- A Be., a Pp. és az Alaptörvény a már ellenőrzött fájlra cserélendő (B/2, A/2) – a következő commitban.

## S2 – uniós aktusok cserélve (2026-11-19)

- **Cserélve (12) és új (1)** az EUR-Lex hatályos egységes szerkezetű magyar HTML-jéből (átalakító: `/home/claude/c2conv/eurlex.py`, a munkakörnyezetben): 98/5/EK (2013.07.01.), 1/2003/EK (2009.07.01.), 2004/38/EK (2011.06.16.), 139/2004/EK (2004.02.18.), 2005/36/EK (2025.10.29.), 2006/111/EK (2025.08.10.), 2006/123/EK (2006.12.28.), 864/2007/EK (2009.01.11.), 593/2008/EK (2008.07.24.), 1215/2012/EU (2015.02.26.), 2016/679/EU (2016.05.04.), 2020/1784/EU (2025.05.01.); új: `2018_1725_EU rendelet a személyes adatok uniós intézményi kezeléséről.txt` (2018.11.21.). A manifest frissítve (`darab` 118; a Storage-ba még feltöltendők).
- **Teljesség:** betű+szám karakter HTML 1 194 370 = TXT 1 194 370 (eltérés 0,000% mind a 13 fájlban); cikk HTML 650 = TXT 650; 28 betűnél hosszabb „szó” 3 (a 2005/36/EK mellékletének valódi német/svéd szakmanevei). Egy forráselírás javítva: 2018/1725 „8 l. cikk” → „81. cikk”. A táblázatsorok `| `-vel kezdődnek (a megfelelési táblák „1. cikk | 1. cikk” sora ne legyen cikkfej).
- **Preambulum:** a 98/5, 1/2003, 139/2004, 2005/36, 2006/111, 2016/679, 2018/1725 és 2020/1784 egységes szerkezete preambulumbekezdések nélküli; a régi (PDF-ből összefolyt) preambulum nem maradt meg. Emiatt a 35. tétel hét „2005/36/EK irányelv (n) preambulumbekezdés” doboza most eltér (a három 98/5-ös eddig is eltért).
- **Alapállapot előtte → utána:** `feloldatlan 2 → 3` (alapfelvétel; l. lent), `dobozok: 418, eltérés: 96 → 30`, `hiányos bekezdés: 172 → 31`; a doboz_javit 119 dobozból 97-et írt (`/home/claude/c2conv/doboz_javit_szurt.py`: a doboz_javit változatlan kódja, a hibás korpuszcikkek kihagyásával); utána `módosítandó doboz: 22`. Dobozszám tételenként változatlan.
- **Nyitva maradt 22 doboz (okkal):** EUMSZ 54., 70. (10., 28. t.), 77., 81. (9., 10. t.), 85. (10. t.), 88., 235. és EUSZ 1., 3. – a korpusz-cikkben szétvágott szó („következ őket”, „b űnmegelőzésre”), elválasztási maradvány („Amenynyiben”), összefolyt szöveg („továbMAGAS SZERZŐDŐ FELEK biakban”, lábjegyzet); Charta 8., 10., 12., 14., 15., 17., 54. – szétvágott szó, írásjel előtti szóköz, lapfej („C 202/396 HU …”), az 54. cikkhez csatolt záró megjegyzés; 98/5/EK 2., 6., 10. (35. t.) – a tétel saját „[helyesen: …]” betoldásai elvesznének, a 6. cikk (3) bekezdése kimaradna; EUMSZ 125. (39. t.) – eszközhiba (lent). Az EUMSZ/EUSZ/Charta további eltérései tördelésből (a tétel szövege PDF-ből szétvágott: „bekez désének”) és csonka idézetből (EUMSZ 292., 133., 157.) adódtak; ezek újraépültek.
- **A 45/2001/EK rendelet** (kiírás, 7. tétel) az EUR-Lex szerint már nem hatályos; helyébe az (EU) 2018/1725 rendelet lépett; a korpuszban mindkettő megvan. **Döntés (Attila, 2026-11-19 18:40; admin `01_dontesek.md`, commit `91a88c8`):** ahol a kiírás a 45/2001/EK rendeletet nevezi meg, a tétel az (EU) 2018/1725 rendeletre épül, és egy mondatban jelzi, hogy a kiírás a hatályon kívül helyezett 45/2001/EK-t nevezi meg. A `beallitas.json` módosítását (a 2018/1725 felvétele) a központi chat végzi a KE-3 készletjavítás után.

**Központi teendő (javaslat):**
1. `tools/alapfelvetel.py`, a `hatarozatok_altalanos` eredményét feldolgozó ciklus (`felold`): a `kiirasElirasok.kihagy` csak fájl nélküli megnevezésre hat. Az új GDPR-fájl első sora (teljes cím) tartalmazza „a 95/46/EK irányelv hatályon kívül helyezéséről” részt, így a kihagyott „95/46/EK” a GDPR-fájlra oldódik, a „(EU) 2016/679” ismétlés lesz, a forrás kódja `95/46/EK`-ra változik, és a GDPR 19 doboza eltűnik (dobozok 418 → 399), „GDPR) II. és III. Fejezet” feloldatlan. Ezért az alapfelvétel kimenetét (`tetelsor/tetelsor.json`, `tetelsor/forrasok.json`, `jelentesek/alapfelvetel.md`) nem commitoltam. Javaslat: `if nev in kihagy: continue` a fájlkeresés eredményétől függetlenül.
2. `tools/s5/doboz_javit.py`, `csoportok()`: a záró `while sorok and cimsor(sorok[-1]): sorok.pop()` a pont nélkül végződő utolsó bekezdés sorait címnek veszi és levágja (EUMSZ 125. cikk (2): „…konzultációt / követően … / … fogalmakat” → csak az első sor maradna).
3. `alapfelvetel.egyseg_sor` (`^(\d+)\. cikk\b`): a betűs cikkszámot („4a. cikk”) nem ismeri; a 2005/36/EK 19, az 1215/2012/EU 4, a 2020/1784/EU 1 ilyen cikke az előző cikk szövegéhez csapódik.
4. `kozos.jogszabaly_paragrafusok`: az azonos számú második cikkfejnél (az EUMSZ megfelelési tábláinak „288. cikk 340. cikk” sora) a sort az első cikkhez fűzi (a `doboz_javit.paragrafus_sorok` ilyenkor lezárja az egységet).

**Attila teendői:** nincs (a preambulum és a 45/2001 ↔ 2018/1725 kérdés lezárva, l. lent).


### S2, 2. kör – szerződések, Charta, preambulumok (2026-11-19)

- **Cserélve** (átalakító: `/home/claude/c2conv/eurlex_oj.py`, az `eurlex.py` sorbontójával): `EUMSZ - … (2016).txt` (CELEX 12016E), `EUSZ - … (2016).txt` (12016M), `Alapjogi Charta (2016).txt` (12016P), mind HL C 202., 2016.6.7. **Tartalmi kör:** a két szerződés-HTML (és a régi fájl is) a szerződést, a 37 jegyzőkönyvet, a mellékleteket, a Lisszaboni Szerződés zárónyilatkozatához csatolt nyilatkozatokat és a megfelelési táblázatokat tartalmazza (az EUMSZ-fájl a szerződés mellékleteit is); a régi fájl „AZ OLVASÓHOZ” szerkesztői bevezetője a HTML-ben nincs, ezért kimaradt. A Charta: tartalomjegyzék, preambulum, 54 cikk, záró megjegyzés.
- **Teljesség (a) HTML ↔ TXT:** EUMSZ 562 227 = 562 227, EUSZ 329 334 = 329 334, Charta 20 691 = 20 691 (0,000%); minden HTML-cikkfej (656 / 353 / 54) sorrendben megvan önálló sorként, más „N. cikk” sor nincs. Hosszú „szó”: a forrás elírása „BIZTONSÁGPOLITIKAIFŐKÉPVISELŐJÉT” (EUMSZ, EUSZ címsor) és „ezerkilencszázkilencvenkettedik”.
- **Teljesség (b) új ↔ régi, cikkenként** (csak betű+szám, kisbetűs; a szerződés-, ill. Charta-szöveg): EUMSZ 358 cikkből 349 betűre egyező, 9 eltér; EUSZ 55-ből 51 egyező, 4 eltér; Charta 54-ből 43 egyező, 11 csak a régi lapfeje miatt tér el. Szóhatárra is egyező (lapfej nélkül): 273 / 29 / 51 – a többi a régi fájl szóközzel szétvágott szava („következ őket”). Az eltérők oka a régi fájl hibája: lábjegyzetjel és -szöveg (EUMSZ 8., 11., EUSZ 1.), elválasztási maradvány („Amenynyiben”, „átalányöszszegnek”: EUMSZ 235., 260., 355., EUSZ 18., 55.), összefolyt szöveg (EUSZ 1. „továbMAGAS SZERZŐDŐ FELEK biakban”), cikkhatár („319. cikk értelmében…” sorkezdet a 318. cikkben: EUMSZ 318–319.), a záró „FENTIEK HITELÉÜL” helye (EUMSZ 358., EUSZ 55.). **Tartalmi (hatályossági) eltérés nincs.** Nem hatályossági, de tartalmi: az EUR-Lex HTML-ből hiányoznak a cikken belüli alcímek – EUMSZ 294. („Első olvasat”, „Második olvasat”, „Egyeztetés”, „Harmadik olvasat”, „Különös rendelkezések”) és EUSZ 48. („Rendes felülvizsgálati eljárás”, „Egyszerűsített módosítási eljárások”).
- **Preambulum pótolva:** a 98/5/EK (HL L 77., 1998.3.14., 36. o.; CELEX 31998L0005; 15 preambulumbekezdés) és a 2005/36/EK (HL L 255., 2005.9.30., 22. o.; CELEX 32005L0036; 44 preambulumbekezdés) korpuszfájljában a cím és az „Egységes szerkezet:” sor után „Preambulum (az eredeti kihirdetett szöveg szerint, …)” címsorral, preambulumbekezdésenként egy sorban; lábjegyzeteik a fájl végén. Karakterszám: 2005/36 21 680 = 21 680; 98/5 8 509 → 8 503 (a 6 számjegy a „[1]”–„[6]” lábjegyzetjel).
- **Dobozok:** a doboz_javit 98 módosítandó dobozából 92 íródott (a burkoló csak a lenti hatot hagyja ki); utána `módosítandó doboz: 6`. Dobozszám tételenként változatlan.
- **Alapállapot előtte → utána:** `feloldatlan 3 → 3` (az alapfelvétel kimenete a GDPR/95/46 hiba miatt most sincs commitolva), `dobozok: 418, eltérés: 30 → 15`, `hiányos bekezdés: 31 → 12`.
- **Nyitva maradt dobozok:** 98/5/EK 2., 6., 10. (35. t.: a tétel saját „[helyesen: …]” betoldásai, a 6. cikk (3) bekezdése); EUMSZ 125. (39. t.: ismert eszközhiba, utasításra kihagyva – az új, egysoros (2) bekezdéssel a doboz_javit most már teljes szöveget adna); EUMSZ 294. (9. t.: az alcímek elvesznének); Charta 54. (20. t.: a záró megjegyzés a cikkhez csapódna). Az `ellenorzes` további eltérései: EUMSZ 10. (19. t.) – a forrásban (EUR-Lex) nincs záró pont, a doboz_javit a pont nélküli egyetlen sort a `csoportok()` záró levágása miatt nem látja (2. központi pont); a 35. tétel hat 2005/36/EK- és három 98/5/EK-preambulumdoboza – a tétel dobozszövege PDF-ből szétvágott („értel- (1) mében”), a preambulumdobozt a doboz_javit nem építi újra.


## Közös készlet KE-3 (2026-11-19, központi chat)

- Szinkronizálva (admin-commit `9ceab3a`): új `tools/s5/doboz_beszur.py` (doboz beszúrása a korpuszból), a `kontroll.py` minden forrás §/cikk-hivatkozását ellenőrzi és termékek nélkül is fut, betűs cikkszám, táblasor nem cikkfej, kihagyott megnevezés, záró sor levágása javítva.
- `alapfelvetel: tétel 43, feloldott 199, feloldatlan 2, hiba 0` | `dobozok: 418, eltérés: 14; hiányzó forrás: []; lefedettségi hiány: 10 elem 2 tételben` | `hiányos bekezdés: 11`
- A 7. tétel a 45/2001/EK helyett az (EU) 2018/1725 rendelet VI. fejezetére (52–60. cikk) épül (`beallitas.json` `tetelForras`; Attila döntése 2026-11-19 18:40). Az EUMSZ 125. cikk doboza újraépítve.
