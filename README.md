# C/2 Az Európai Unió joga

Export ideje: 2026-11-21T08:18:35+01:00
Ág: elo-2026-11-21-0818

43 kidolgozott szöveges anyagrész, a belőlük készült termékek, és a kötött jogszabály-korpusz. A tartalom **változatlan** másolat: nincs trimmelés, nincs átírás, nincs összevonás.

| Mappa | Forrás | Darab |
|---|---|---|
| `01.txt`–`43.txt` | `tetelek.txtContent` | 43 szöveg |
| `egyeb/tetel_html/` | `tetelek.htmlContent` | 43 html |
| `tanulokartyak/` | `notes` `type=deck` `flashcards` | 0 pakli, 0 kártya |
| `kviz/` | `question_banks.questions` | 86 bank, 3025 kérdés |
| `hezagpotlok/` | `notes` `type=cloze` `items` | 40 gyakorlat, 494 szegmens |
| `memoriautvonal/` | `memoriapalota_allomasok` | 43 útvonal, 814 állomás |
| `korpusz/` | Storage TXT | 117 jogszabály |
| `tts/` | `tts_documents` chunkonként | 44 dokumentum, 533 chunk |
| `egyeb/notes/` | `notes` további típusok | 174 dokumentum |
| `egyeb/cloze_variants/` | `notes/*/cloze_variants` | 160 variáns |
| `egyeb/deck_collections/` | `deck_collections` | 43 gyűjtemény |

Egy Firestore-dokumentum = egy fájl (a darabolt anyagrészek külön pakliban/bankban maradnak). A kártyánál csak `front` / `back` / `explanation` került be; a `processed_*` elválasztó-másolat és a belső meta kimaradt. Az útvonal `utvonal.html` a `htmlTartalom` byte-azonos másolata, az `allomasok/*.json` a `tartalom` mezőé.

Az ellenőrző összegek: gyökér `manifest.json` (szövegek), a termék-mappák és a `korpusz/manifest.json`.

| Fájl | Cím | Karakter |
|---|---|---|
| 01.txt | Az Európai Unió alapszerződései. (Milyen jelentős intézményi (...) | 16375 |
| 02.txt | Az Európai Unió intézményei, főbb hatásköreik és egymáshoz való viszonyuk | 21335 |
| 03.txt | Az Európai Bizottság összetétele, működése és hatáskörei | 21243 |
| 04.txt | Az Európai Unió Tanácsának összetétele, működése és hatáskörei. Az (...) | 20665 |
| 05.txt | Az Európai Parlament összetétele, tagjainak választása, működése és (...) | 21828 |
| 06.txt | Az Európai Unió Bíróságának felépítése és működése | 44562 |
| 07.txt | Az Európai Ombudsman és a petíciós jog; az Európai Adatvédelmi Biztos | 31646 |
| 08.txt | Az Európai Unió hatáskörei. A hatáskör-átruházás elve; az Alaptörvény (...) | 25560 |
| 09.txt | Jogalkotási eljárás az Európai Unióban; a rendes jogalkotási eljárás és (...) | 39156 |
| 10.txt | A nemzeti parlamentek szerepe az uniós jogalkotási eljárásban | 37906 |
| 11.txt | Az Európai Unió elsődleges jogforrásai | 14047 |
| 12.txt | Az Európai Unió mint a nemzetközi jog alanya; az Európai Unió által (...) | 22650 |
| 13.txt | A rendelet joghatásai, jellemzői és viszonya a nemzeti joghoz; a (...) | 14063 |
| 14.txt | Az irányelv joghatásai, jellemzői és viszonya a nemzeti joghoz; az (...) | 15865 |
| 15.txt | A jogalkotási aktusok és a nem jogalkotási aktusok elhatárolása. Az (...) | 15895 |
| 16.txt | Az uniós jog autonómiája és elsőbbsége | 15326 |
| 17.txt | A közvetlen hatály; az Alapszerződések, a rendeletek, az irányelvek (...) | 16533 |
| 18.txt | Az uniós polgárság és az uniós polgársághoz fűződő jogok terjedelme; az (...) | 19406 |
| 19.txt | A diszkrimináció tilalma és az egyenlő bánásmód elve az uniós jogban (...) | 26911 |
| 20.txt | Alapjogvédelem az Európai Unióban; Az Európai Unió Alapjogi Chartája (...) | 14671 |
| 21.txt | Az Európai Unió Bíróságának ítélkezési gyakorlata az alapjogok terén (...) | 13770 |
| 22.txt | A tagállamokkal szemben indított kötelezettségszegési eljárás (...) | 13253 |
| 23.txt | Az uniós jogi aktusok megsemmisítése iránti eljárás (az eljárás (...) | 17909 |
| 24.txt | Az előzetes döntéshozatali eljárás (az eljárás kezdeményezésére (...) | 17417 |
| 25.txt | Az előzetes döntéshozatali eljárás és a magyar bírósági jogalkalmazás (...) | 16000 |
| 26.txt | A tagállam kárfelelőssége az uniós jog megsértéséért (általános alapelvek) | 14996 |
| 27.txt | Az Európai Unió intézményei vagy azok alkalmazottai által okozott kár (...) | 12011 |
| 28.txt | A szabadság, a biztonság és a jog érvényesülésén alapuló térség (...) | 25239 |
| 29.txt | Igazságügyi együttműködés büntetőügyekben; a kölcsönös elismerés elve (...) | 22781 |
| 30.txt | A közös kül- és biztonságpolitika elvei és céljai, intézményrendszere (...) | 33884 |
| 31.txt | A belső piac fogalma, kialakulása; jogalkotás – dereguláció a belső (...) | 15044 |
| 32.txt | A személyek szabad mozgása; kivételek a személyek szabad mozgása alól | 20030 |
| 33.txt | A munkavállalók szabad mozgása; a letelepedés szabadsága önálló (...) | 19188 |
| 34.txt | A letelepedés szabadsága vállalkozások esetében | 17829 |
| 35.txt | A diplomák és szakképesítések kölcsönös elismerése; az ügyvédi hivatás (...) | 16158 |
| 36.txt | Az áruk szabad mozgása; a vámok és azzal azonos hatású díjak tilalma; a (...) | 17744 |
| 37.txt | A szolgáltatások szabad mozgása, a szolgáltatás fogalma, az (...) | 16640 |
| 38.txt | A tőke szabad mozgása | 14607 |
| 39.txt | A monetáris unió fogalma és jelentősége | 63956 |
| 40.txt | Mi a versenyjog funkciója? Milyen jogforráson alapul? (antitröszt (...) | 29805 |
| 41.txt | Mi a Bizottság szerepe a versenyjogban (a Bizottság hatásköre (...) | 27039 |
| 42.txt | Az adatkezelési elvek és az érintett jogai | 51057 |
| 43.txt | Az Európai Unió klíma- és energiapolitikájának fő irányai | 18469 |

## Korpusz

| Fájl | storageFrissitve | Időállapot |
|---|---|---|
| 1215_2012_EU rendelet Brüsszel Ia.txt | 2026-08-18T11:57:11.778Z | ismeretlen |
| 1259_2010_EU rendelet Róma III.txt | 2026-08-22T08:15:29.624Z | ismeretlen |
| 139_2004_EK rendelet az összefonódások ellenőrzéséről.txt | 2026-08-18T11:57:04.633Z | ismeretlen |
| 143_2010. (VII. 14.) AB határozat.txt | 2026-07-07T03:38:41.865Z | ismeretlen |
| 1_2003_EK rendelet a versenyszabályok végrehajtásáról.txt | 2026-08-18T11:56:48.744Z | ismeretlen |
| 1_2009. (VI. 24.) PK-KK közös vélemény.txt | 2026-08-18T11:56:49.937Z | ismeretlen |
| 2004_38_EK irányelv a polgárok szabad mozgásáról.txt | 2026-08-18T11:57:04.380Z | ismeretlen |
| 2005_36_EK irányelv a szakmai képesítések elismeréséről.txt | 2026-08-18T11:56:48.406Z | ismeretlen |
| 2006_111_EK irányelv a közvállalkozások pénzügyi átláthatóságáról.txt | 2026-08-22T08:15:30.874Z | ismeretlen |
| 2006_123_EK irányelv a belső piaci szolgáltatásokról.txt | 2026-08-18T11:57:04.881Z | ismeretlen |
| 2016_679_EU rendelet GDPR.txt | 2026-08-22T08:15:31.229Z | ismeretlen |
| 2019_1111_EU rendelet Brüsszel IIb.txt | 2026-08-22T08:15:31.443Z | ismeretlen |
| 2020_1783_EU rendelet a bizonyításfelvételről.txt | 2026-08-18T11:56:49.519Z | ismeretlen |
| 2020_1784_EU rendelet iratkézbesítés.txt | 2026-08-22T08:15:31.804Z | ismeretlen |
| 22_2016. (XII. 5.) AB határozat az Alaptörvény E) cikk (2) bekezdésének értelmezéséről.txt | 2026-08-18T11:56:50.810Z | ismeretlen |
| 2_13 sz. EUB vélemény (EJEE).txt | 2026-08-18T11:57:17.147Z | ismeretlen |
| 2_2019. (III. 5.) AB határozat az Alaptörvény R) cikk (1) bekezdésének, 24. cikk (1) bekezdésének, valamint a XIV. cikk (4) bekezdésének értelmezéséről.txt | 2026-07-07T03:38:49.828Z | ismeretlen |
| 2_94 sz. EUB vélemény (EJEE).txt | 2026-08-18T11:57:15.610Z | ismeretlen |
| 30_1998. (VI. 25.) AB határozat.txt | 2026-07-07T03:38:51.925Z | ismeretlen |
| 32_2008. (III. 12.) AB határozat.txt | 2026-07-07T03:38:55.541Z | ismeretlen |
| 3_2005. (XI. 14.) PK-KK vélemény.txt | 2026-08-18T11:56:50.323Z | ismeretlen |
| 45_2001_EK rendelet a személyes adatok intézményi feldolgozásáról.txt | 2026-08-18T11:56:49.128Z | ismeretlen |
| 593_2008_EK rendelet Róma I.txt | 2026-08-18T11:57:05.357Z | ismeretlen |
| 5_7-24_66 Kampffmeyer egyesített ügyek.txt | 2026-08-22T08:15:33.433Z | ismeretlen |
| 650_2012_EU rendelet öröklési ügyek.txt | 2026-08-22T08:15:33.627Z | ismeretlen |
| 864_2007_EK rendelet Róma II.txt | 2026-08-18T11:57:05.117Z | ismeretlen |
| 98_5_EK irányelv az ügyvédi hivatás állandó gyakorlásáról.txt | 2026-08-18T11:57:04.128Z | ismeretlen |
| Alapjogi Charta (2016).txt | 2026-08-22T08:15:34.176Z | ismeretlen |
| Alaptörvény - Magyarország Alaptörvénye (2011. április 25.) - Hatályos Jogszabályok Gyűjteménye.txt | 2026-09-30T14:03:52.542Z | ismeretlen |
| Be. (új) - 2017. évi XC. törvény a büntetőeljárásról - Hatályos Jogszabályok Gyűjteménye.txt | 2026-09-30T14:51:20.984Z | ismeretlen |
| Bizottsági közlemény - közszolgáltatás ellentételezése (2012_C 8_03).txt | 2026-08-22T08:15:34.647Z | ismeretlen |
| C-106_77 Simmenthal-ügy.txt | 2026-08-18T11:57:13.791Z | ismeretlen |
| C-106_89 Marleasing-ügy tárgyalási jelentés.txt | 2026-08-18T11:56:51.938Z | ismeretlen |
| C-106_89 Marleasing-ügy.txt | 2026-08-18T11:56:51.532Z | ismeretlen |
| C-112_00 Schmidberger-ügy.txt | 2026-08-21T14:24:49.138Z | ismeretlen |
| C-11_70 Internationale Handelsgesellschaft-ügy.txt | 2026-08-22T08:15:35.469Z | ismeretlen |
| C-120_78 Cassis de Dijon-ügy.txt | 2026-08-18T11:57:14.058Z | ismeretlen |
| C-12_86 Demirel-ügy tárgyalási jelentés.txt | 2026-08-22T08:15:35.806Z | ismeretlen |
| C-12_86 Demirel-ügy.txt | 2026-08-18T11:56:53.057Z | ismeretlen |
| C-135_08 Rottmann-ügy.txt | 2026-08-18T11:57:09.325Z | ismeretlen |
| C-139_85 Kempf-ügy.txt | 2026-08-18T12:49:24.125Z | ismeretlen |
| C-144_04 Mangold-ügy.txt | 2026-08-22T08:15:36.439Z | ismeretlen |
| C-147_03 Bizottság kontra Ausztria-ügy.txt | 2026-08-18T11:57:02.872Z | ismeretlen |
| C-149_79 Bizottság kontra Belgium-ügy.txt | 2026-08-18T11:57:14.530Z | ismeretlen |
| C-150_05 Van Straaten-ügy.txt | 2026-08-22T08:15:36.931Z | ismeretlen |
| C-152_84 Marshall-ügy.txt | 2026-08-18T11:56:47.997Z | ismeretlen |
| C-187_01 Gözütok és Brügge-ügy.txt | 2026-08-18T11:57:16.626Z | ismeretlen |
| C-200_02 Zhu és Chen-ügy.txt | 2026-08-22T08:15:37.458Z | ismeretlen |
| C-208_00 Überseering-ügy.txt | 2026-08-18T11:57:16.369Z | ismeretlen |
| C-210_06 Cartesio-ügy.txt | 2026-08-18T11:57:08.533Z | ismeretlen |
| C-212_97 Centros-ügy.txt | 2026-08-18T11:57:15.854Z | ismeretlen |
| C-224_01 Köbler-ügy.txt | 2026-08-18T11:57:16.882Z | ismeretlen |
| C-24_68 Bizottság kontra Olaszország-ügy.txt | 2026-08-22T08:16:41.863Z | ismeretlen |
| C-25_62 Plaumann-ügy.txt | 2026-08-18T11:56:53.864Z | ismeretlen |
| C-26_62 van Gend en Loos-ügy.txt | 2026-08-18T11:57:12.251Z | ismeretlen |
| C-283_81 CILFIT-ügy.txt | 2026-08-18T11:56:54.277Z | ismeretlen |
| C-286_82 Luisi és Carbone egyesített ügyek.txt | 2026-08-18T11:56:54.669Z | ismeretlen |
| C-290_05 Nádasdi és Németh-ügy.txt | 2026-08-22T08:16:42.697Z | ismeretlen |
| C-294_83 Les Verts-ügy.txt | 2026-08-18T11:56:55.422Z | ismeretlen |
| C-297_07 Bourquain-ügy.txt | 2026-08-22T08:16:43.076Z | ismeretlen |
| C-29_69 Stauder-ügy.txt | 2026-08-22T08:16:43.282Z | ismeretlen |
| C-2_74 Reyners-ügy.txt | 2026-08-18T11:57:12.018Z | ismeretlen |
| C-328_04 Vajnai-ügy végzés.txt | 2026-08-18T11:56:55.799Z | ismeretlen |
| C-33_74 van Binsbergen-ügy.txt | 2026-08-22T08:16:43.766Z | ismeretlen |
| C-340_89 Vlassopoulou-ügy.txt | 2026-08-18T11:56:56.495Z | ismeretlen |
| C-344_87 Bettray-ügy tárgyalási jelentés.txt | 2026-08-22T08:16:44.166Z | ismeretlen |
| C-344_87 Bettray-ügy.txt | 2026-08-22T08:16:44.361Z | ismeretlen |
| C-358_93 Bordessa és társai egyesített ügyek.txt | 2026-08-18T11:56:57.345Z | ismeretlen |
| C-359_09 Ebert-ügy.txt | 2026-08-18T11:57:09.561Z | ismeretlen |
| C-364_10 Magyarország kontra Szlovákia-ügy.txt | 2026-08-22T08:16:44.836Z | ismeretlen |
| C-36_75 Rutili-ügy.txt | 2026-08-18T11:56:57.717Z | ismeretlen |
| C-374_87 Orkem-ügy tárgyalási jelentés.txt | 2026-08-18T11:56:58.600Z | ismeretlen |
| C-374_87 Orkem-ügy.txt | 2026-08-22T08:16:45.376Z | ismeretlen |
| C-379_87 Groener-ügy.txt | 2026-08-18T12:49:26.007Z | ismeretlen |
| C-415_93 Bosman-ügy.txt | 2026-08-18T11:57:15.091Z | ismeretlen |
| C-416_10 Križan-ügy.txt | 2026-08-22T08:16:45.909Z | ismeretlen |
| C-41_74 van Duyn-ügy.txt | 2026-08-18T11:57:13.267Z | ismeretlen |
| C-420_16 P Izsák és Dabis-ügy.txt | 2026-08-18T11:57:10.534Z | ismeretlen |
| C-436_04 Van Esbroeck-ügy.txt | 2026-08-22T08:16:46.483Z | ismeretlen |
| C-43_75 Defrenne II-ügy.txt | 2026-08-18T11:57:13.510Z | ismeretlen |
| C-44_79 Hauer-ügy.txt | 2026-08-18T11:57:14.294Z | ismeretlen |
| C-453_99 Courage-ügy.txt | 2026-08-18T11:57:00.337Z | ismeretlen |
| C-46_93 Brasserie du Pêcheur-ügy.txt | 2026-08-18T11:57:14.838Z | ismeretlen |
| C-473_93 Bizottság kontra Luxemburg-ügy.txt | 2026-08-18T12:49:27.583Z | ismeretlen |
| C-484_93 Svensson és Gustavsson-ügy.txt | 2026-08-18T11:57:00.576Z | ismeretlen |
| C-486_14 Kossowski-ügy.txt | 2026-08-18T11:57:10.301Z | ismeretlen |
| C-491_07 Turanský-ügy.txt | 2026-08-22T08:16:47.826Z | ismeretlen |
| C-493_17 Weiss-ügy.txt | 2026-08-18T11:57:11.043Z | ismeretlen |
| C-4_73 Nold-ügy.txt | 2026-08-18T11:56:59.718Z | ismeretlen |
| C-503_99 Bizottság kontra Belgium aranyrészvény-ügy.txt | 2026-08-18T11:57:16.117Z | ismeretlen |
| C-54_96 Dorsch Consult-ügy.txt | 2026-08-22T08:16:48.472Z | ismeretlen |
| C-55_94 Gebhard-ügy.txt | 2026-08-18T11:57:15.342Z | ismeretlen |
| C-57_65 Lütticke-ügy.txt | 2026-08-21T14:24:59.572Z | ismeretlen |
| C-583_11 Inuit Tapiriit Kanatami fellebbezés.txt | 2026-08-18T11:57:03.115Z | ismeretlen |
| C-583_11 P Inuit Tapiriit Kanatami-ügy.txt | 2026-08-21T14:25:00.032Z | ismeretlen |
| C-5_71 Schöppenstedt-ügy.txt | 2026-08-18T11:57:12.779Z | ismeretlen |
| C-5_88 Wachauf-ügy tárgyalási jelentés.txt | 2026-08-18T11:57:00.830Z | ismeretlen |
| C-5_88 Wachauf-ügy.txt | 2026-08-18T11:57:01.085Z | ismeretlen |
| C-617_10 Åkerberg Fransson-ügy.txt | 2026-08-22T08:16:49.790Z | ismeretlen |
| C-66_85 Lawrie-Blum-ügy.txt | 2026-08-22T08:16:50.012Z | ismeretlen |
| C-673_16 Coman-ügy.txt | 2026-08-18T11:57:10.796Z | ismeretlen |
| C-68_79 Hans Just-ügy.txt | 2026-08-18T12:49:30.030Z | ismeretlen |
| C-6_64 Costa kontra ENEL-ügy.txt | 2026-08-18T11:57:12.500Z | ismeretlen |
| C-6_90 Francovich és Bonifaci egyesített ügyek.txt | 2026-08-21T14:25:01.621Z | ismeretlen |
| C-83_76 Bayerische HNL-ügy.txt | 2026-08-22T08:16:50.931Z | ismeretlen |
| C-899_19 P Románia kontra Bizottság-ügy.txt | 2026-08-18T11:57:11.533Z | ismeretlen |
| C-8_74 Dassonville-ügy.txt | 2026-08-18T11:57:13.032Z | ismeretlen |
| Consilium - éghajlatváltozás politikája.txt | 2026-08-21T14:25:02.438Z | ismeretlen |
| EH 2008.1815 Kfv.I.35.055_2007.txt | 2026-08-18T11:56:51.083Z | ismeretlen |
| EUMSZ - az Európai Unió működéséről szóló szerződés (2016).txt | 2026-08-22T08:16:52.104Z | ismeretlen |
| EUSZ - az Európai Unióról szóló szerződés (2016).txt | 2026-08-22T08:16:52.287Z | ismeretlen |
| Ismertetők az Európai Unióról - Energiapolitika általános elvek (2020).txt | 2026-08-21T14:25:03.561Z | ismeretlen |
| Pp. (új) - 2016. évi CXXX. törvény a polgári perrendtartásról - Hatályos Jogszabályok Gyűjteménye.txt | 2026-09-30T14:54:15.062Z | ismeretlen |
| T-18_10 Inuit Tapiriit Kanatami végzés (EN).txt | 2026-08-21T14:25:04.002Z | ismeretlen |
| T-391_17 Románia kontra Bizottság Minority SafePack-ügy.txt | 2026-08-18T11:57:11.286Z | ismeretlen |
| T-529_13 Izsák és Dabis-ügy.txt | 2026-08-18T11:57:09.811Z | ismeretlen |
| T-646_13 Minority SafePack-ügy.txt | 2026-08-18T11:57:10.060Z | ismeretlen |
