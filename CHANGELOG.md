# Kiela pakeitimų istorija

Tobuliname Kiela filtrą, kad jis būtų kuo originalesnis, o jo kūrimas nesiremtų kitais filtrais. Išsaugome Kiela kainų rodymą, ROLL vertinimą, receptų pagalbą ir žaidėjui naudingas funkcijas.

Įrašai pateikti nuo naujausio. Ankstesnių versijų taisykles gali pakeisti vėlesni atnaujinimai.

## [v1.2.56](https://github.com/Melly87s/Kiela/releases/tag/v1.2.56) — Angliški profiliai ir trumpesnis kiekių rodymas

- Strict lygių pavadinimai ir aprašymai pakeisti į anglų kalbą. Iš profilių eilučių pašalintas Kiela pavadinimas ir versija, kad tekstas užimtų mažiau vietos.
- Kiekis ant žemės rodomas tik tikroms krūvelėms nuo 2 vienetų: `2x Key`, `5x Worldstone Shard`.
- Nuo pavienių ir nesikaupiančių daiktų bei pavienių potionų pašalintas `x1`.
- Goldo pavadinimas išlaiko įprastą sumos rodymą. Atrankos taisyklės ir PD2 specialių daiktų apsauga išsaugotos.

- Klasei rekomenduojami runeword ant žemės rodomi žaliai. Kai klasei tinkamos rekomendacijos nėra, `Possible RW` rodo kitus suderinamus runeword pavadinimus pilkai.

## [v1.2.55](https://github.com/Melly87s/Kiela/releases/tag/v1.2.55) — PD2 specialių daiktų apsauga

- Visuose strict lygiuose atskirai apsaugoti mapai, jų gerinimo medžiagos ir orbai, WSS, Puzzlebox, Puzzlepiece, Malus, crafting medžiagos, fragmentai, essences, boss raktai bei kiti kataloge esantys specialūs daiktai.
- Šiems daiktams netaikomi įrangos modų skaičiaus ar set roll atrankos reikalavimai.
- Patikrinta 180 žaidimo lentelių įrašų, įskaitant 42 mapus. Apsauga tikrinta visuose 0–11 lygiuose ir penkiose kokybės kategorijose.
- Mapai papildomai apsaugoti pagal žaidimo map tier požymį, net jei jų kodo dar nėra kataloge.
- Išsaugotas tolesnis kiekių, kainų ir pagalbos rodymas. Praėjo 131 automatinis testas.

## [v1.2.54](https://github.com/Melly87s/Kiela/releases/tag/v1.2.54) — Item level aprašymuose

- Galutinio daikto aprašymo apačioje pridėta paprasta eilutė `Item level: 85` su tikru daikto lygiu.
- Item level žyma nededama prie daikto pavadinimo.
- Išsaugotas kiekio, kainų, receptų ir ROLL rodymas.

## [v1.2.53](https://github.com/Melly87s/Kiela/releases/tag/v1.2.53) — Griežtesnė set atranka

- Nuo **Endgame – Strict**, 9 lygio, atpažinti žemesnės kategorijos set daiktai nebepraeina atrankos vien dėl +skill bonusų.
- Tai taikoma ir corrupted daiktams, kai jų žemesnės kategorijos set tapatybę galima nustatyti.
- Atrinktiems geresniems set daiktams paliktas 90% minimumas, kai jų roll palaikomas ir patikimai įvertinamas.
- Neaiškūs bendros bazės kandidatai ir nepalaikomi roll atvejai saugomi atsargiai. Inventoriaus daiktai neslepiami; unique rodymas išsaugotas.

## [v1.2.52](https://github.com/Melly87s/Kiela/releases/tag/v1.2.52) — Daiktų kiekiai ir goldo ribos

- Visi matomi daiktai ant žemės rodo kiekį: `x1` pavieniam daiktui arba tikrą krūvelės kiekį, pvz., `x5`.
- Kiekis išlieka prie WSS kainų, gemų, potionų ir pervadintų magic/rare daiktų. Pašalintas dvigubas gemų kiekio rodymas.
- Goldo suma rodoma vieną kartą. Nuo Farming Strict minimalios rodomos sumos yra:

| Lygis | Profilis | Goldo minimumas |
| --- | --- | ---: |
| 5 | Farming – Strict | 2 000 |
| 6 | Farming – Stricter | 3 000 |
| 7 | Endgame | 4 000 |
| 8 | Endgame – Stricter | 5 000 |
| 9 | Endgame – Strict | 6 000 |
| 10 | Endgame – Fast Mapping | 7 000 |
| 11 | Endgame – Minimal | 8 000 |

- HR/WSS kainos lieka vieneto kainų įverčiais; krūvelės kiekis jų automatiškai nepadaugina.

## [v1.2.51](https://github.com/Melly87s/Kiela/releases/tag/v1.2.51) — Naudingų savybių atranka

- Nuo Farming Strict identifikuotiems magic įrangos daiktams ir žiedams/amuletams reikia bent 2 naudingų savybių derinio.
- Identifikuotai rare įrangai ir žiedams/amuletams 5–11 lygiuose reikia atitinkamai **3 / 4 / 4 / 5 / 6 / 6 / 6** naudingų savybių.
- Skaičiuojamos naudingos savybės, o ne tikslus affixų skaičius. Keli skill laukai skaičiuojami kaip viena savybė; silpni atsitiktiniai bonusai nepadeda pasiekti ribos.
- Nuo Endgame, 7 lygio, slepiama įprasta magic įranga, įskaitant +skill daiktus. Charms, jewels, žiedams ir amuletams taikoma atskira atranka.
- Neidentifikuoti rare kandidatai paliekami pagal atskiras bazės taisykles, nes jų tikrų bonusų dar negalima įvertinti.
- Ant žemės prie identifikuotų magic/rare daiktų pridėti tikri skill ir stat bonusai, pvz., `+3 Bow skills` ir `+20% IAS`.
- Runeword rekomendacijoms naudojami pilni pavadinimai; klasei rekomenduojami receptai ir runų eilė aprašyme pažymėti žaliai.

## [v1.2.50](https://github.com/Melly87s/Kiela/releases/tag/v1.2.50) — Aiškesni profiliai ir 90% set roll

- Paskutiniuose trijuose lygiuose palaikomiems identifikuotiems set roll nustatytas vienodas **90%** minimumas.
- Žinomas mažesnis roll nepraeina vien dėl +skill bonuso. Fiksuotiems tinkamiems šablonams, neturintiems kintamo roll, procentas nepriskiriamas.
- Neaiškūs, neidentifikuoti ar modifikuoti kandidatai vertinami atsargiai.
- Profilių aprašymuose trumpiniai pakeisti pilnais kategorijų pavadinimais ir aiškesniais paaiškinimais.

## [v1.2.49](https://github.com/Melly87s/Kiela/releases/tag/v1.2.49) — Slėpimo pataisos ir runeword bazės

- Pataisyta taisyklių išplėtimo tvarka pagal tikrą PD2 filtro veikimą. Ankstesnė klaida galėjo palikti matomus slepiamus potionus, scrolls, mažas goldo krūveles ir silpnas bazes.
- Pridėtos patikros pagal žaidime pastebėtus Oil, HP, MP, Thawing, scrolls ir silpnų įrangos daiktų atvejus.
- Runeword bazių atranka nuo Farming palaipsniui griežtinama: ED/defense ribos 5–11 lygiuose yra **5 / 8 / 10 / 12 / 15 / 18 / 20%**, kartu griežtinami aktualūs klasės ir Paladin shield bonusai.
- Paskutiniame lygyje reikia maksimalių aktualių bazės bonusų ir tikrų receptui tinkamų socketų. Jau pagamintiems runewords šios bazių taisyklės netaikomos.
- Nuo Farming `Possible RW` rekomendacijos rodomos tik bazėms, praeinančioms pasirinkto profilio atranką.
- Susiaurinta paprastų magic daiktų ir identifikuotos juvelyrikos atranka. Pradėta set atranka paskutiniuose trijuose lygiuose; vėlesnės versijos ją patikslino.

## [v1.2.48](https://github.com/Melly87s/Kiela/releases/tag/v1.2.48) — Progresija ir mažiau nereikalingų daiktų

- Normal ir Nightmare rodo visus daiktus.
- Hell ir Baal Runs naudoja atsargias item level gaires bei naudingų savybių ir affix potencialo išimtis. Griežto ilvl 85 slenksčio nėra.
- Hell ir Baal Runs rodo Flawless bei Perfect gemus; nuo Farming — tik Perfect. Runos, unique ir Perfect gemai rodomi visuose lygiuose.
- Nuo Hell slepiami Stamina, Thawing, Oil potionai ir palaidi Identify/Town Portal scrolls. Tomes paliekami.
- Nuo Farming slepiami Freezing/cold throwing potionai.
- Grąžintas violetinis rejuvenation rodymas: **35%** ir **☺FULL☺**.

## [v1.2.47](https://github.com/Melly87s/Kiela/releases/tag/v1.2.47) — Pradinė skill daiktų apsauga

- Pridėta +2 ar didesnių all/class/tree/single skill ir oskill bonusų apsauga bei neidentifikuotos įrangos saugojimas.
- Apsauga leido tęsti kainų, ROLL ir pagalbos apdorojimą.
- Vėlesnės versijos šią bendrą apsaugą pakeitė konkrečiomis magic, rare, set ir runeword bazių atrankos taisyklėmis.

## [v1.2.46](https://github.com/Melly87s/Kiela/releases/tag/v1.2.46) — Originalus Kiela atrankos pagrindas

- Sukurtas naujas Kiela atrankos generatorius, nenaudojantis kitų filtrų kaip kūrimo įvesties ar taisyklių šablono.
- Runeword, crafting ir daiktų faktai imami iš PD2 žaidimo lentelių.
- Išsaugotas Kiela HR/WSS kainų rodymas, ROLL vertinimas, crafting pagalba, klasės rekomendacijos ir vaizdinės funkcijos.
- Pridėtas pasikartojančių taisyklių šalinimas generavimo metu, išsaugant jų apdorojimo tvarką.
- Dabartinio generatoriaus patikros fiksuoja 0 vienodų pasikartojančių ItemDisplay taisyklių ir 0 kitų filtrų kaip vykdymo įvesčių. Šios patikros savaime nėra viso projekto autorystės įrodymas.

## Viešo filtro licencijos ir platinimo sutvarkymas

- Iš viešo filtro pašalinti Kiela specifiniai naudojimo apribojimai ir atskira ribojanti Kiela licencija.
- Išsaugoti privalomi MIT teisių ir licencijos įrašai bei [trečiųjų šalių pranešimai](./THIRD-PARTY-NOTICES.md).
- Viešame repozitoriume platinamas paruoštas filtras ir dokumentacija; generatoriaus šaltiniai palaikomi atskirai.
- Leidimai platinami ZIP ir RAR archyvais. Pakeitimai taip pat diegiami į vietines žaidimo filtro kopijas ir tikrinamas jų sutapimas.

Kainų datos atnaujinamos tik atnaujinus pačius kainų duomenis. Dokumentacijos pataisa filtro versijos nekeičia.
