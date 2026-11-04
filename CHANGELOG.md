# Kiela Changelog / Pakeitimų istorija

[English](#english) · [Lietuviškai](#lietuviškai)

## English

We are developing Kiela to be as original as possible, with a build process that does not rely on other loot filters. We preserve Kiela's price displays, ROLL ratings, recipe guidance and useful player features.

Newest entries appear first. Later releases may supersede earlier selection rules. This documentation update does not change the filter version.

### [v1.2.56](https://github.com/Melly87s/Kiela/releases/tag/v1.2.56) — English profiles and compact stack labels

- Strictness names and descriptions are now in English. Removed the Kiela name and version from profile lines to save space.
- Ground quantities appear only for stacks of two or more: `2x Key`, `5x Worldstone Shard`.
- Removed `x1` from single items, nonstackable equipment and single potions. Gold retains its usual amount display.
- Class-appropriate runeword ground recommendations are green. If no class recommendation matches, `Possible RW` lists compatible generic runeword names in gray.
- Item selection and PD2 special-drop protections are preserved.

### [v1.2.55](https://github.com/Melly87s/Kiela/releases/tag/v1.2.55) — PD2 special-drop protection

- Added explicit protection at every strictness for maps, map-upgrade materials and orbs, WSS, Puzzlebox, Puzzlepiece, Malus, crafting materials, fragments, essences, boss keys and other cataloged special items.
- Equipment modifier-count and set-roll requirements do not hide these items.
- Checked 180 game-table records, including 42 maps, at levels 0–11 across five qualities. Native map-tier detection also protects map codes outside the catalog.
- Quantities, prices and help continue processing. All 131 automated tests passed.

### [v1.2.54](https://github.com/Melly87s/Kiela/releases/tag/v1.2.54) — Item level in descriptions

- Final item descriptions end with plain text such as `Item level: 85`, using the item's actual level.
- Item level is displayed in the description rather than beside the item name.
- Quantity, price, recipe and ROLL information is preserved.

### [v1.2.53](https://github.com/Melly87s/Kiela/releases/tag/v1.2.53) — Stricter set selection

- From Endgame – Strict, level 9, known lower-tier sets no longer bypass selection through skill bonuses.
- This also covers corrupted lower-tier items when their set identity can be determined.
- Selected higher-tier sets retain a 90% minimum where their variable roll is supported and can be evaluated reliably.
- Ambiguous shared-base candidates and unsupported rolls remain conservative. Inventory items remain inspectable; unique visibility is preserved.

### [v1.2.52](https://github.com/Melly87s/Kiela/releases/tag/v1.2.52) — Ground quantities and gold thresholds

- Introduced a ground quantity label for every visible item: `x1` for single items and the actual stack quantity, such as `x5`. Version 1.2.56 later replaced this with stack-only labels in the `5x` format.
- Quantities survive WSS prices, gem and potion labels, and identified-equipment name changes. Removed duplicate gem counts.
- Gold amounts are displayed once. Farming and higher profiles use these minimums:

| Level | Profile | Minimum gold |
| --- | --- | ---: |
| 5 | Farming – Strict | 2,000 |
| 6 | Farming – Stricter | 3,000 |
| 7 | Endgame | 4,000 |
| 8 | Endgame – Stricter | 5,000 |
| 9 | Endgame – Strict | 6,000 |
| 10 | Endgame – Fast Mapping | 7,000 |
| 11 | Endgame – Minimal | 8,000 |

- HR/WSS estimates remain per-item estimates; stack size does not automatically multiply them.

### [v1.2.51](https://github.com/Melly87s/Kiela/releases/tag/v1.2.51) — Useful-property selection

- From Farming Strict, identified magic equipment, rings and amulets require a combination of at least two useful properties.
- Identified rare equipment, rings and amulets require **3 / 4 / 4 / 5 / 6 / 6 / 6** useful properties at levels 5–11.
- This counts useful property categories, not exact affix slots. Multiple skill fields count once; weak incidental bonuses do not satisfy the thresholds.
- From Endgame, level 7, ordinary magic equipment is hidden, including skill items. Charms, jewels, rings and amulets have separate selection rules.
- Unidentified rare candidates retain separate base-selection checks because their actual bonuses cannot yet be evaluated.
- Identified magic/rare ground labels show actual bonuses, such as `+3 Bow skills` and `+20% IAS`.
- Runeword recommendations use full names; class recommendations and ordered rune recipes are highlighted in green in descriptions.

### [v1.2.50](https://github.com/Melly87s/Kiela/releases/tag/v1.2.50) — Clearer profiles and 90% set rolls

- Set a uniform **90%** minimum for supported identified set rolls in the last three profiles.
- A known lower roll cannot bypass the threshold through skill bonuses. Eligible fixed templates have no variable roll to grade.
- Unidentified, ambiguous or modified candidates retain conservative handling.
- Replaced terse profile abbreviations with full category names and clearer descriptions.

### [v1.2.49](https://github.com/Melly87s/Kiela/releases/tag/v1.2.49) — Visibility fixes and runeword bases

- Corrected rule-expansion order to match the actual PD2 filter engine. The previous error could leave hidden potions, scrolls, small gold piles and weak bases visible.
- Added regressions for observed Oil, HP, MP, Thawing, scroll and weak-equipment cases.
- Runeword base requirements become stricter from Farming: enhanced damage/defense thresholds at levels 5–11 are **5 / 8 / 10 / 12 / 15 / 18 / 20%**, with increasing relevant class and Paladin-shield requirements.
- The final profile requires maximum relevant base bonuses and actual recipe-compatible sockets. These base requirements do not apply to completed runewords.
- From Farming, `Possible RW` recommendations require a base that passes the selected profile's requirements.
- Narrowed ordinary magic and identified jewelry selection. Introduced late-profile set selection, refined by later releases.

### [v1.2.48](https://github.com/Melly87s/Kiela/releases/tag/v1.2.48) — Progression and reduced clutter

- Normal and Nightmare show all items.
- Hell and Baal Runs use cautious item-level guidance with useful-property and affix-potential exceptions. There is no hard ilvl-85 cutoff.
- Hell and Baal Runs retain Flawless and Perfect gems; Farming and higher retain Perfect gems. Runes, uniques and Perfect gems remain visible at every level.
- From Hell, hide Stamina, Thawing and Oil potions and loose Identify/Town Portal scrolls. Keep tomes.
- From Farming, hide Freezing/cold throwing potions.
- Restored purple rejuvenation labels: **35%** and **☺FULL☺**.

### [v1.2.47](https://github.com/Melly87s/Kiela/releases/tag/v1.2.47) — Initial skill-item protection

- Added protection for +2-or-higher all/class/tree/single-skill and oskill bonuses, and conservative unidentified-equipment handling.
- Protection continued through price, ROLL and help processing.
- Later releases replaced this blanket protection with specific magic, rare, set and runeword-base selection policies.

### [v1.2.46](https://github.com/Melly87s/Kiela/releases/tag/v1.2.46) — Original Kiela selection engine

- Built a new Kiela selection generator without using other filters as build inputs or rule templates.
- Runeword, crafting and item facts are derived from PD2 game tables.
- Preserved Kiela HR/WSS displays, ROLL ratings, crafting help, class recommendations and visual features.
- Added generation-time duplicate-rule removal while preserving processing order.
- Current generator checks report zero duplicate complete ItemDisplay rules and zero external-filter runtime inputs. Those checks alone do not establish authorship of the entire project.

### Public licensing and distribution cleanup

- Removed Kiela-specific usage restrictions and the separate restrictive Kiela license from the public filter.
- Preserved required MIT rights, license notices and [third-party notices](./THIRD-PARTY-NOTICES.md).
- The public repository distributes the prepared filter and documentation; authoring sources are maintained separately.
- Releases are available as ZIP and RAR archives. Filter updates are also installed locally and checked for matching contents.

Price dates change only when the price data itself is updated. Documentation-only changes do not increment the filter version.

---

## Lietuviškai

Tobuliname Kiela filtrą, kad jis būtų kuo originalesnis, o jo kūrimas nesiremtų kitais filtrais. Išsaugome Kiela kainų rodymą, ROLL vertinimą, receptų pagalbą ir žaidėjui naudingas funkcijas.

Įrašai pateikti nuo naujausio. Ankstesnių versijų taisykles gali pakeisti vėlesni atnaujinimai.

### [v1.2.56](https://github.com/Melly87s/Kiela/releases/tag/v1.2.56) — Angliški profiliai ir trumpesnis kiekių rodymas

- Strict lygių pavadinimai ir aprašymai pakeisti į anglų kalbą. Iš profilių eilučių pašalintas Kiela pavadinimas ir versija, kad tekstas užimtų mažiau vietos.
- Kiekis ant žemės rodomas tik tikroms krūvelėms nuo 2 vienetų: `2x Key`, `5x Worldstone Shard`.
- Nuo pavienių ir nesikaupiančių daiktų bei pavienių potionų pašalintas `x1`.
- Goldo pavadinimas išlaiko įprastą sumos rodymą. Atrankos taisyklės ir PD2 specialių daiktų apsauga išsaugotos.

- Klasei rekomenduojami runeword ant žemės rodomi žaliai. Kai klasei tinkamos rekomendacijos nėra, `Possible RW` rodo kitus suderinamus runeword pavadinimus pilkai.

### [v1.2.55](https://github.com/Melly87s/Kiela/releases/tag/v1.2.55) — PD2 specialių daiktų apsauga

- Visuose strict lygiuose atskirai apsaugoti mapai, jų gerinimo medžiagos ir orbai, WSS, Puzzlebox, Puzzlepiece, Malus, crafting medžiagos, fragmentai, essences, boss raktai bei kiti kataloge esantys specialūs daiktai.
- Šiems daiktams netaikomi įrangos modų skaičiaus ar set roll atrankos reikalavimai.
- Patikrinta 180 žaidimo lentelių įrašų, įskaitant 42 mapus. Apsauga tikrinta visuose 0–11 lygiuose ir penkiose kokybės kategorijose.
- Mapai papildomai apsaugoti pagal žaidimo map tier požymį, net jei jų kodo dar nėra kataloge.
- Išsaugotas tolesnis kiekių, kainų ir pagalbos rodymas. Praėjo 131 automatinis testas.

### [v1.2.54](https://github.com/Melly87s/Kiela/releases/tag/v1.2.54) — Item level aprašymuose

- Galutinio daikto aprašymo apačioje pridėta paprasta eilutė `Item level: 85` su tikru daikto lygiu.
- Item level žyma nededama prie daikto pavadinimo.
- Išsaugotas kiekio, kainų, receptų ir ROLL rodymas.

### [v1.2.53](https://github.com/Melly87s/Kiela/releases/tag/v1.2.53) — Griežtesnė set atranka

- Nuo **Endgame – Strict**, 9 lygio, atpažinti žemesnės kategorijos set daiktai nebepraeina atrankos vien dėl +skill bonusų.
- Tai taikoma ir corrupted daiktams, kai jų žemesnės kategorijos set tapatybę galima nustatyti.
- Atrinktiems geresniems set daiktams paliktas 90% minimumas, kai jų roll palaikomas ir patikimai įvertinamas.
- Neaiškūs bendros bazės kandidatai ir nepalaikomi roll atvejai saugomi atsargiai. Inventoriaus daiktai neslepiami; unique rodymas išsaugotas.

### [v1.2.52](https://github.com/Melly87s/Kiela/releases/tag/v1.2.52) — Daiktų kiekiai ir goldo ribos

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

### [v1.2.51](https://github.com/Melly87s/Kiela/releases/tag/v1.2.51) — Naudingų savybių atranka

- Nuo Farming Strict identifikuotiems magic įrangos daiktams ir žiedams/amuletams reikia bent 2 naudingų savybių derinio.
- Identifikuotai rare įrangai ir žiedams/amuletams 5–11 lygiuose reikia atitinkamai **3 / 4 / 4 / 5 / 6 / 6 / 6** naudingų savybių.
- Skaičiuojamos naudingos savybės, o ne tikslus affixų skaičius. Keli skill laukai skaičiuojami kaip viena savybė; silpni atsitiktiniai bonusai nepadeda pasiekti ribos.
- Nuo Endgame, 7 lygio, slepiama įprasta magic įranga, įskaitant +skill daiktus. Charms, jewels, žiedams ir amuletams taikoma atskira atranka.
- Neidentifikuoti rare kandidatai paliekami pagal atskiras bazės taisykles, nes jų tikrų bonusų dar negalima įvertinti.
- Ant žemės prie identifikuotų magic/rare daiktų pridėti tikri skill ir stat bonusai, pvz., `+3 Bow skills` ir `+20% IAS`.
- Runeword rekomendacijoms naudojami pilni pavadinimai; klasei rekomenduojami receptai ir runų eilė aprašyme pažymėti žaliai.

### [v1.2.50](https://github.com/Melly87s/Kiela/releases/tag/v1.2.50) — Aiškesni profiliai ir 90% set roll

- Paskutiniuose trijuose lygiuose palaikomiems identifikuotiems set roll nustatytas vienodas **90%** minimumas.
- Žinomas mažesnis roll nepraeina vien dėl +skill bonuso. Fiksuotiems tinkamiems šablonams, neturintiems kintamo roll, procentas nepriskiriamas.
- Neaiškūs, neidentifikuoti ar modifikuoti kandidatai vertinami atsargiai.
- Profilių aprašymuose trumpiniai pakeisti pilnais kategorijų pavadinimais ir aiškesniais paaiškinimais.

### [v1.2.49](https://github.com/Melly87s/Kiela/releases/tag/v1.2.49) — Slėpimo pataisos ir runeword bazės

- Pataisyta taisyklių išplėtimo tvarka pagal tikrą PD2 filtro veikimą. Ankstesnė klaida galėjo palikti matomus slepiamus potionus, scrolls, mažas goldo krūveles ir silpnas bazes.
- Pridėtos patikros pagal žaidime pastebėtus Oil, HP, MP, Thawing, scrolls ir silpnų įrangos daiktų atvejus.
- Runeword bazių atranka nuo Farming palaipsniui griežtinama: ED/defense ribos 5–11 lygiuose yra **5 / 8 / 10 / 12 / 15 / 18 / 20%**, kartu griežtinami aktualūs klasės ir Paladin shield bonusai.
- Paskutiniame lygyje reikia maksimalių aktualių bazės bonusų ir tikrų receptui tinkamų socketų. Jau pagamintiems runewords šios bazių taisyklės netaikomos.
- Nuo Farming `Possible RW` rekomendacijos rodomos tik bazėms, praeinančioms pasirinkto profilio atranką.
- Susiaurinta paprastų magic daiktų ir identifikuotos juvelyrikos atranka. Pradėta set atranka paskutiniuose trijuose lygiuose; vėlesnės versijos ją patikslino.

### [v1.2.48](https://github.com/Melly87s/Kiela/releases/tag/v1.2.48) — Progresija ir mažiau nereikalingų daiktų

- Normal ir Nightmare rodo visus daiktus.
- Hell ir Baal Runs naudoja atsargias item level gaires bei naudingų savybių ir affix potencialo išimtis. Griežto ilvl 85 slenksčio nėra.
- Hell ir Baal Runs rodo Flawless bei Perfect gemus; nuo Farming — tik Perfect. Runos, unique ir Perfect gemai rodomi visuose lygiuose.
- Nuo Hell slepiami Stamina, Thawing, Oil potionai ir palaidi Identify/Town Portal scrolls. Tomes paliekami.
- Nuo Farming slepiami Freezing/cold throwing potionai.
- Grąžintas violetinis rejuvenation rodymas: **35%** ir **☺FULL☺**.

### [v1.2.47](https://github.com/Melly87s/Kiela/releases/tag/v1.2.47) — Pradinė skill daiktų apsauga

- Pridėta +2 ar didesnių all/class/tree/single skill ir oskill bonusų apsauga bei neidentifikuotos įrangos saugojimas.
- Apsauga leido tęsti kainų, ROLL ir pagalbos apdorojimą.
- Vėlesnės versijos šią bendrą apsaugą pakeitė konkrečiomis magic, rare, set ir runeword bazių atrankos taisyklėmis.

### [v1.2.46](https://github.com/Melly87s/Kiela/releases/tag/v1.2.46) — Originalus Kiela atrankos pagrindas

- Sukurtas naujas Kiela atrankos generatorius, nenaudojantis kitų filtrų kaip kūrimo įvesties ar taisyklių šablono.
- Runeword, crafting ir daiktų faktai imami iš PD2 žaidimo lentelių.
- Išsaugotas Kiela HR/WSS kainų rodymas, ROLL vertinimas, crafting pagalba, klasės rekomendacijos ir vaizdinės funkcijos.
- Pridėtas pasikartojančių taisyklių šalinimas generavimo metu, išsaugant jų apdorojimo tvarką.
- Dabartinio generatoriaus patikros fiksuoja 0 vienodų pasikartojančių ItemDisplay taisyklių ir 0 kitų filtrų kaip vykdymo įvesčių. Šios patikros savaime nėra viso projekto autorystės įrodymas.

### Viešo filtro licencijos ir platinimo sutvarkymas

- Iš viešo filtro pašalinti Kiela specifiniai naudojimo apribojimai ir atskira ribojanti Kiela licencija.
- Išsaugoti privalomi MIT teisių ir licencijos įrašai bei [trečiųjų šalių pranešimai](./THIRD-PARTY-NOTICES.md).
- Viešame repozitoriume platinamas paruoštas filtras ir dokumentacija; generatoriaus šaltiniai palaikomi atskirai.
- Leidimai platinami ZIP ir RAR archyvais. Pakeitimai taip pat diegiami į vietines žaidimo filtro kopijas ir tikrinamas jų sutapimas.

Kainų datos atnaujinamos tik atnaujinus pačius kainų duomenis. Dokumentacijos pataisa filtro versijos nekeičia.
