# EX-1 jelentés – C/2 Az Európai Unió joga élő export

- Ág: `elo-2026-11-21-0818`
- Commit azonosító: ebben a fájlban nem szerepelhet, mert a hash a fájlt tartalmazó commitból számolódik. A feltöltés utáni `git log --oneline -1` sora a válaszban és a távoli ágon van.
- Export indítása: `2026-11-21T08:18:35+01:00` (a szkript `exportIdeje` mezője)
- Tételsor: `JBrZP1FWSK16o7uFiCpM` — `C/2 Az Európai Unió joga`
- Firestore: projekt `orlomed-f8f9f`, adatbázis `jogedu`. Csak olvasás.

## 4.1 Azonosító

Elérési út: `/tmp/ex1_list_tetelsorok.js`. Kilépési kód: **0**. Húsz dokumentum.

A `C/2` jelzés és az `Az Európai Unió joga` szöveg, 43 szöveggel, pontosan egy dokumentumot jelöl: `JBrZP1FWSK16o7uFiCpM`. `status`: `ready`. `kidolgozottCount`: 43. A `targy` mező ugyanez a mondat.

Megnézve, de nem illeszkedik: `8kjcRd2zRjplcC2EnCEx`, cím `C/2 Az Európai Unio Joga_2`, szintén 43 szöveg. A név nem tartalmazza az `Unió` szót (ékezet nélkül `Unio`, és `_2` a végén). A `targy` mezője `Polgári jog`. Ez nem került exportra.

## 4.2 Munkafa és ág

A helyi klón a futás elején nem létezett. Létrehozva a feladatlap URL-jével: `git clone https://github.com/TattilaNinox/c_2-az-eur-pai-uni-joga-.git ~/Desktop/jogedu_tetelsor_repok/c_2-az-eur-pai-uni-joga-`. Ez lefutott. A munkafa előtt `git fetch origin` kilépési kódja: **0**.

Ágak: `origin/main`, `origin/elokeszites-2026-11-19`. `origin/tts-javitas` nincs. `origin/tartalom-javitas` nincs.

Ág: `elo-2026-11-21-0818`, worktree: `~/Desktop/jogedu_tetelsor_repok/c2_elo`, kiindulás: `origin/main` (`2005e01`). `worktree add` kilépési kód: **0**.

`git rm -r -q .` kilépési kód: **0**. A törlés után a rövid státusz 1367 sor. Az első három: `D README.md`, `D hezagpotlok/02/jEtTaObZcvvr9jVQSaQ5.json`, `D hezagpotlok/03/zCqlnpb2Md6ieQU9TjNB.json`.

## 4.3 Export

```
cd ~/Desktop/orlomed_admin_web && node functions/scripts/export_tetelsor_repo.js \
  --tetelsor=JBrZP1FWSK16o7uFiCpM \
  --repo="$HOME/Desktop/jogedu_tetelsor_repok/c2_elo" \
  --korpusz="jogforrasok/1.Jogszabályok/Korpusz/C2 tételsor/TXT/"
```

Kilépési kód: **0**.

Kategória: C/2 Az Európai Unió joga

```
STAT {"kihagyva":{"notes:status=Draft":86},"kotetlen":[],"vizsgalt":{"notes":{"talalat":300,"hiba":[]},"question_banks":{"talalat":86,"hiba":[]},"memoriapalota_allomasok":{"talalat":43,"hiba":[]},"tts_documents":{"talalat":44,"hiba":[]},"jogeset_items":{"talalat":0,"hiba":[]},"dialogus_fajlok":{"talalat":0,"hiba":[]},"sources":{"talalat":0,"hiba":[]},"temakorok":{"talalat":0,"hiba":[]},"egyetem_tetelsorok":{"talalat":0,"hiba":[]},"hangoskartyak":{"talalat":0,"hiba":[]},"deck_collections":{"talalat":1174,"kotott":43}},"kihagyottPontos":["jogforrasok/1.Jogszabályok/Korpusz/C2 tételsor/TXT/.placeholder"],"memoriaUtkozes":[],"darab":{"szovegek":43,"tanulokartyak":0,"kviz":86,"hezagpotlok":40,"memoriautvonal":43,"korpusz":117,"tts":44,"egyeb/tetel_html":43,"egyeb/notes":174,"egyeb/cloze_variants":160,"egyeb/deck_collections":43,"jogesetek":0,"dialogusok":0},"kartya":0,"kerdes":3025,"szegmens":494,"allomas":814,"chunkFiles":533,"ismertIdoallapot":0,"nullIdoallapot":117,"kotottLawDocId":17,"orphan":[],"mp3":[],"kategoria":"C/2 Az Európai Unió joga","exportIdeje":"2026-11-21T08:18:35+01:00","ag":"elo-2026-11-21-0818","extraUres":["sources","temakorok","egyetem_tetelsorok","hangoskartyak"],"eloSzuro":{"tetelsorok/tetelek":"a sor minden sorszama; ures txtContent nincs","notes deck":"status=Published es deletedAt ures; a gyujtemenybe tett pakli is, mert a kliens a gyujtemenyben megnyitja","notes cloze":"status=Published es deletedAt ures","notes egyeb":"status=Published es deletedAt ures; type nem deck es nem cloze","cloze_variants":"a publikalt cloze alkollekcioja, sajat allapotmezo nelkul","question_banks":"deletedAt ures, corpusGateLive nem false; status mezo nincs, vagy Published","memoriapalota_allomasok":"status=Published es deletedAt ures","tts_documents":"status=Published, vagy nincs status mezo, vagy publikalt jegyzet hangforrasa","jogeset_items":"status=Published vagy Public, deletedAt ures","dialogus_fajlok":"status=Published es deletedAt ures","deck_collections":"status=Published es a pakli-azonosito vagy a cimke koti a sorhoz","korpusz":"a Storage prefix minden fajlja"}}
```

Záró sor: `Kész. Szövegek 43, pakli 0, bank 86, gyakorlat 40, útvonal 43, korpusz 117, tts 44.`

## 5.1 Darabszámok

| Mi | Tájékoztató (feladatlap) | Most |
|---|---:|---:|
| Szövegfájl `NN.txt` | 43 | 43 (`01.txt`–`43.txt`) |
| Jegyzet, `type=text` | 132 | 131 |
| Jegyzet összesen, manifest nélkül | — | 174 |
| `tts/*/_meta.json` | nincs szám (–) | 44 |
| Tanulókártya / pakli | nincs külön szám | 0 |
| Kvízbank | nincs külön szám | 86 |
| Hézagpótló | nincs külön szám | 40 |
| Memóriaútvonal (mappa) | nincs külön szám | 43 |
| Korpusz `*.txt` | nincs külön szám | 117 |
| `EXPORT.json` | — | megvan |

A 174 jegyzet: 131 `text` + 43 `dynamic_quiz_dual`. Jegyzetmappák: `01`–`43`. A `tanulokartyak/` csak a `manifest.json`-t tartalmazza (0 pakli). A korpusz manifest 117 tétel, 117 egyedi fájlnév, lemezen 117 txt. Nincs névütközés.

Egyéb szkript-darabok: `egyeb/tetel_html` 43, `egyeb/cloze_variants` 160, `egyeb/deck_collections` 43, kártya 0, kérdés 3025, szegmens 494, állomás 814, chunk fájl 533. `deck_collections`: találat 1174, kötött 43.

## 5.2 Hang

- `tts/*/_meta.json`: **44**, mind `via: "audioSource"`
- `egyeb/notes/**.json` nem üres `audioPath`: **44**
- az első három `audioPath`, a jegyzetfájl útvonala szerint rendezve, változatlanul:
  - `audio/notes/i4Y5JpPPOOYIdaV6lA83.mp3` (`egyeb/notes/01/ngU7XF87KVWuSdCVylzJ.json`)
  - `audio/notes/mlOQe8Q0W0dcV9XVff0P.mp3` (`egyeb/notes/03/MsvR7ukMk2MxJwqxQWxw.json`)
  - `audio/notes/Z0I0hirZKUH5RephLu6q.mp3` (`egyeb/notes/04/9U3fyPIirRZKLAzBwYmQ.json`)

## 5.3 Tiltott fájlok

`find` (mp3, service-account, key, pem), `.git` kihagyva: **0**.

E-mail minta (`grep -rIl`), `.git` kihagyva: **0 fájl**. Kilépési kód: **1**.

## 5.4 Összevetés

- `origin/tts-javitas`: nincs ilyen ág
- `origin/tartalom-javitas`: nincs ilyen ág
- `origin/main`: megvan. Könyvtárai: `hezagpotlok jegyzetek korpusz kviz memoriautvonal tanulokartyak`. `tts` könyvtár ezen az ágon nincs.

Add előtt:

- `origin/main -- tts`: üres kimenet
- `origin/main -- jegyzetek egyeb/notes`: `132 files changed, 16925 deletions(-)`

`git add .` kilépési kód: **0**. Add után:

- `origin/main -- tts`: `580 files changed, 12242 insertions(+)`
- `origin/main -- jegyzetek egyeb/notes`: `307 files changed, 6461 insertions(+), 16925 deletions(-)`

## Figyelmeztetések és eltérések

- A `_2` végű dokumentum nem illeszkedett az `Unió` szövegre, ezért nem ez került ki. A kiírt kategória a feladatlap mondatával egyezik.
- Kihagyva: **86 jegyzet** `status=Draft`. Ezek nincsenek az ágon. A szkript élő szűrője a publikált jegyzetet írja ki.
- Jegyzet `type=text`: 131 a tájékoztató 132-höz képest. Az add előtti `jegyzetek` diff 132 fájlt törölt. Az egy publikált darab különbség oka nincs külön igazolva; a 86 piszkozat ettől független, azokat a szűrő hagyta ki.
- Tanulókártya / pakli: 0. A tájékoztató erre nem ad számot.
- Hangdokumentumra a feladatlap nem ad számot. Élő tts meta 44, mind `audioSource`, nem üres `audioPath` 44.
- Korpusz: a `.placeholder` kimaradt. 117 txt, mind időállapot nélkül (`ismertIdoallapot` 0, `nullIdoallapot` 117). Kötött lawDocId: **17** a 117-ből. Nincs kettős név.
- Üres vizsgálat, hiba nélkül: `sources`, `temakorok`, `egyetem_tetelsorok`, `hangoskartyak`. Jogeset 0, dialógus 0. Kötetlen: üres.
- Hangot nem generáltam, Firestore-ba és Storage-ba nem írtam, másik ágat nem módosítottam.

## Ami nem futott, vagy nincs futásidőben ellenőrizve

- A feltöltés és a 7. pont a commit után fut; az eredménye nincs ebben a fájlban.
- A hangfájlok lejátszása, a kliens és a Firestore felület nincs megnyitva.
- A 86 piszkozat jegyzet azonosítója nincs külön listázva: a szkript csak a darabszámot írta ki.
