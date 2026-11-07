# Melindaa v1.2.74

## PD2 Launcher registration

Copy this entry into the official PD2 `filters.json` when submitting a pull request. Pateikdami „pull request“, nukopijuokite šį įrašą į oficialų PD2 `filters.json`.

```json
{"name": "Melindaa", "url": "https://api.github.com/repos/Melly87s/Melindaa/contents", "author": "Melindaa"}
```

## English

Project Diablo 2 loot filter with our own equipment selection, dated HR/WSS estimates, supported ROLL ratings, actual ground bonuses, crafting help and class-aware runeword recommendations.

**[Download ZIP](https://github.com/Melly87s/Melindaa/releases/latest/download/Melindaa.zip)** · **[Download RAR](https://github.com/Melly87s/Melindaa/releases/latest/download/Melindaa.rar)** · **[Changelog](./CHANGELOG.md)** · **[Full filter specification](./FILTER-SPECIFICATION.md)**

### Choose your strictness

| Level | Profile | What it shows and hides |
| --- | --- | --- |
| 1 | Normal | Shows all items. |
| 2 | Nightmare | Shows all items. |
| 3 | Hell | Broad useful Magic/Rare candidates and cautious unidentified potential. Flawless and Perfect gems. Hides Stamina, Thawing, Oil and loose ID/TP scrolls. |
| 4 | Baal Runs | Tighter equipment and plain-base selection than Hell. Flawless and Perfect gems. Useful crafting candidates can still appear. |
| 5 | Farming with Blue | Selected useful Magic combinations and unidentified candidates: skill + speed/cast, socket/block/life and strong weapons. Unidentified throwing knives/axes/javelins require ETH elite bases; non-ETH or normal/exceptional blue throwing drops are hidden. Useful Rare; all Unique/Set/Craft. Good advanced RW bases and CTA/HOTO exceptions. Perfect gems; gold 2,000+. |
| 6 | Farming without Blue | Hides all ordinary Magic equipment and jewelry, identified or not. Charms, jewels and PD2 specials remain. Same Rare/Set/RW selection as Farming with Blue. Perfect gems; gold 3,000+. |
| 7 | Endgame | Hides ordinary Magic gear/jewelry. Stronger identified Rare; selected useful Set; supported Rare/Set roll 90%+. All Unique/Craft and unidentified Rare kept. Perfect relevant RW bonuses; unsocketed or matching existing sockets. Perfect gems; gold 4,000+. |

**Always visible at every level:** all Unique items for grail collecting, completed orange Crafted items, runes, charms, jewels, protected PD2 maps/materials/fragments/boss ingredients/socket tools, both Rejuvenation potions and **Antidote potions**. Inventory items remain inspectable.

**Farming and Endgame keep all unidentified Rare equipment.** Hidden affixes are not graded. After identification, selection depends on relevant combinations for the equipment category. Unsupported or modified rolls are not assigned an invented percentage. Endgame's 90% requirement applies only where reliable grading is supported.

Farming/Endgame hide ordinary HP/MP potions, cold/gas/fire throwing potions and player ears. Endgame also hides ordinary chest keys. Both retain protected boss keys and special materials. Farming keeps all Set items; Endgame selects useful higher-tier candidates and handles ambiguous unidentified variants conservatively.

### Latest changes, v1.2.63–v1.2.70

- Added Farming with Blue / Farming without Blue; Endgame is now level 7. Gold thresholds from Farming are 2,000 / 3,000 / 4,000. Existing Endgame selections migrate safely.
- Pure Gold Find-only charms show no reliable price instead of a misleading numeric quote.
- Ingredients use Crafting material; gem recipes use their gem colors; socketed items show Sockets: N/M.
- [owned grail] appears beside Unique/Set names on the ground and in inventory.
- Antidote potions are visible at every level again.
- Supported charm ROLL information now survives crafting help and price descriptions.
- Added poison damage and duration to identified Magic/Rare/Crafted ground labels. A poison-only charm can show **[GC] [Psn 11/2s]**.
- Arrows, bolts and throwing weapons (including javelins) no longer show legacy quantity numbers. Real consumable/material stacks still show counts from 2 items upward.
- Removed the FIXED label for items without variable rolls. Socket-method help uses the same light-blue TEAL as ground socket markers.
- Charm and Magic-jewel prices prioritize the complete matching modifier set, pooling numeric rolls while keeping skill identities separate. One-mod Gold charms and skiller + Gold charms are separate comparisons. Rare/Crafted comparisons retain core mods and strongest support roll bands.
- Cube/tome help now preserves all accumulated information across short continuing actions: version, update time, price date, profile and visibility summary. The Cube warns that asking prices may be unrealistic.

### Prices, rolls and help

Prices are dated **asking-price estimates**, not guaranteed sale prices. **Sellers may ask unrealistic amounts, which can distort estimates.** Supported charm/skiller/jewel/base/material/Rare/Crafted samples use a 120-hour listing/bump window. Missing supported samples mean no quote, not proof that no listings exist. Older baseline Unique/Set prices retain their original dates. NPC gold is separate.

ROLL describes supported variable properties, not universal build value. Unknown/modified cases may show CHECK. Ground labels show actual identified bonuses. Socket counts, limits and Larzuk/Puzzle/WSS/Cube help are light blue; class RW recommendations and recipes are green. Maximum socket capacity does not guarantee a socketing result. Superior bases do not use the normal-only random socket Cube recipe.

The **[owned grail]** marker appears beside Unique/Set item names both on the ground and in inventory. It uses PD2's current Unique/Set collection state, not discovery history or an independent stash scan. Update timing after selling the last copy still needs in-game verification. Item level appears at the bottom of descriptions.



### Socketing methods

Eligible unsocketed items show the method's full name and socket result, capped by that base's capacity. For example, a Stealskull with maximum two sockets can show:

| Method | Result for this example | How to use |
| --- | --- | --- |
| Larzuk quest (Act 5) | 1 socket | Use the Act 5 socket quest reward at Larzuk. |
| Larzuk's Puzzlebox | 1–2 sockets | Combine the item and the named tool in the Horadric Cube. |
| Larzuk's Malus | 1 socket | Combine the item and Larzuk's Malus in the Cube; this is an item, not a quest. |

Non-Unique/Set candidates use the eligible **Larzuk's Puzzlepiece** recommendation. Results depend on quality, weapon type and capacity; do not treat the Stealskull example as the result for every item. Already-socketed items keep the compact Sockets: N/M label. Worldstone Shard corruption is a separate risky option.

### Owned Grail

**[owned grail]** is a duplicate-collection hint for Unique and Set items. It appears beside the item name **on the ground and in inventory**, with **Owned Grail: owned** in its description. The name, supported ROLL and price details remain available.

| Situation | What the marker means |
| --- | --- |
| Identified Unique/Set | PD2's native collection state reports that exact item variant as currently owned. |
| Unidentified Unique/Set | Marked only when PD2 confirms ownership for all variants the unknown drop could be. Ambiguous candidates remain unmarked. |
| Marker absent | Ownership was not confirmed. It is not proof you never found the item or that it is missing from every stash. |
| Sold or removed last copy | Marker clears when PD2 updates its ownership state. Immediate versus rejoin timing has not been verified in game. |
| Another owned copy remains | Marker follows PD2's remaining ownership state. Melindaa does not independently scan every stash tab. |
| Previously found, then sold | This is current ownership, not discovery history, a permanent grail achievement or a found-item counter. |
| Better duplicate rolls | Check the displayed stats/ROLL yourself. The ownership flag does not provide the stored copy's roll, so Melindaa cannot calculate an automatic upgrade percentage from it. |

**Owned Grail never hides a Unique item.** Set visibility still follows the selected strictness; this marker itself does not hide items. Ownership information requires PD2's native support and an updated, reloaded filter.

### Install or update

1. Extract the latest ZIP/RAR and copy **Melindaa.filter** into **C:\Diablo II\ProjectD2\filters\local** (adjust for your installation).
2. Choose **Item Filter Profiles → Local Filter → Melindaa.filter → Save** in the PD2 launcher.
3. Start/restart PD2, or use your configured **Reload Loot Filter** control. Check **v1.2.74** in the Horadric Cube description.
4. Change strictness with **Increase Filter Level / Decrease Filter Level** under **Esc → Options → Configure Controls**. The filter does not bind keys automatically.

[MIT license notice](./MIT-NOTICE.txt)

## Lietuviškai

Project Diablo 2 filtras su mūsų sukurta įrangos atranka, datuotais HR/WSS kainų įverčiais, palaikomais ROLL vertinimais, tikrais bonusais ant žemės, craft pagalba ir klasei pritaikytomis runeword rekomendacijomis.

**[Atsisiųsti ZIP](https://github.com/Melly87s/Melindaa/releases/latest/download/Melindaa.zip)** · **[Atsisiųsti RAR](https://github.com/Melly87s/Melindaa/releases/latest/download/Melindaa.rar)** · **[Pakeitimai](./CHANGELOG.md)** · **[Visa filtro specifikacija](./FILTER-SPECIFICATION.md)**

### Pasirink strictness lygį

| Lygis | Profilis | Ką rodo ir slepia |
| --- | --- | --- |
| 1 | Normal | Rodo visus daiktus. |
| 2 | Nightmare | Rodo visus daiktus. |
| 3 | Hell | Platesnė naudingų Magic/Rare ir neidentifikuotų kandidatų atranka. Flawless ir Perfect gemai. Slepia Stamina, Thawing, Oil ir palaidus ID/TP scrolls. |
| 4 | Baal Runs | Griežtesnė įrangos ir paprastų bazių atranka negu Hell. Flawless ir Perfect gemai. Naudingi craft kandidatai dar gali būti rodomi. |
| 5 | Farming with Blue | Atrinkti naudingi Magic deriniai ir neidentifikuoti kandidatai: skill + speed/cast, socket/block/life bei stiprūs ginklai. Neidentifikuoti mėlyni throwing knives/axes/javelins paliekami tik ETH elite bazėse; ne-ETH bei normal/exceptional throwing slepiami. Naudingi Rare; visi Unique/Set/Craft. Geros pažangių RW bazės ir CTA/HOTO išimtys. Tik Perfect gemai; gold nuo 2 000. |
| 6 | Farming without Blue | Slepia visą įprastą Magic įrangą ir jewelry, ID ir unID. Charmai, jewels ir PD2 specialūs daiktai lieka. Rare/Set/RW atranka tokia pati kaip Farming with Blue. Tik Perfect gemai; gold nuo 3 000. |
| 7 | Endgame | Slepia įprastą Magic įrangą/jewelry. Stipresni identifikuoti Rare ir atrinkti naudingi Set; palaikomas Rare/Set roll 90%+. Visi Unique/Craft ir neidentifikuoti Rare lieka. RW: maksimalūs aktualūs bonusai; be socketų arba su tinkamais esamais socketais. Tik Perfect gemai; gold nuo 4 000. |

**Visuose lygiuose rodomi:** visi Unique grail kolekcijai, jau pagaminti oranžiniai Crafted, runos, charmai, jewels, saugomi PD2 mapai/medžiagos/fragmentai/boss ingredientai/socket įrankiai, abu Rejuvenation ir **Antidote potionai**. Inventoriuje daiktai neslepiami.

**Farming ir Endgame palieka visą neidentifikuotą Rare įrangą.** Paslėpti modai nevertinami. Identifikavus tikrinami įrangos kategorijai naudingi deriniai. Nepalaikomiems ar pakeistiems roll neišgalvojamas procentas. Endgame 90% riba taikoma tik patikimai palaikomam vertinimui.

Farming/Endgame slepia įprastus HP/MP, cold/gas/fire throwing potionus ir player ears. Endgame papildomai slepia įprastus chest keys. Boss raktai ir saugomos medžiagos išlieka. Farming rodo visus Set; Endgame atrenka naudingus aukštesnio lygio kandidatus, o neaiškius neidentifikuotus variantus vertina atsargiai.

### Naujausi pakeitimai, v1.2.63–v1.2.70

- Pridėti Farming with Blue / Farming without Blue; Endgame dabar 7 lygis. Gold nuo Farming: 2 000 / 3 000 / 4 000. Ankstesnis Endgame pasirinkimas saugiai perkeliamas.
- Tik Gold Find turintys charmai rodo, kad patikimos kainos nėra, vietoj klaidinančio skaičiaus.
- Ingredientai žymimi Crafting material; gemų receptams naudojamos jų spalvos; socketinti daiktai rodo Sockets: N/M.
- [owned grail] rodoma prie Unique/Set vardų ant žemės ir inventoriuje.
- Antidote vėl rodomi visuose lygiuose.
- Palaikoma charmų ROLL informacija išlieka pridėjus craft pagalbą ir kainas.
- Identifikuotų Magic/Rare/Crafted žymose ant žemės pridėta poison žala ir trukmė, pvz., **[GC] [Psn 11/2s]**.
- Arrows, bolts ir mėtomiems ginklams, įskaitant javelin, neberodomi seni kiekio skaičiai. Tikrų sunaudojamų daiktų/medžiagų krūvelių kiekiai rodomi nuo 2 vnt.
- Daiktams be kintamų roll neberodoma FIXED. Socketų metodų pagalba šviesiai mėlyna TEAL, kaip socketų žymos ant žemės.
- Charmų ir Magic jewel kainai pirmiausia lyginamas visas modų derinys, sujungiant skaitinius roll ir atskiriant skill tapatybes. Vien Gold turintys charmai ir skiller + Gold vertinami atskirai. Rare/Crafted palyginimuose išlaikomi pagrindiniai modai ir stipriausių papildomų modų roll intervalai.
- Kubo/tome pagalba išlaiko visą informaciją tarp trumpų tęstinių taisyklių: versiją, atnaujinimo laiką, kainų datą, profilį ir matomumo santrauką. Kube įspėjama, kad pardavėjų prašomos kainos gali būti nerealios.

### Kainos, roll ir pagalba

Kainos yra datuoti **pardavėjų prašomų kainų įverčiai**, ne garantuota pardavimo vertė. **Pardavėjai gali prašyti nerealių sumų, todėl įverčiai gali būti iškreipti.** Palaikomų charm/skiller/jewel/bazių/medžiagų/Rare/Crafted imtis naudoja 120 val. paskelbimo/atnaujinimo langą. Nepakankama imtis paliekama be kainos; tai nereiškia, kad nėra skelbimų. Senesni baziniai Unique/Set įverčiai išlaiko originalias datas. NPC gold atskiriamas.

ROLL vertina palaikomas kintamas savybes, ne universalų tinkamumą build. Nežinomi/pakeisti atvejai gali rodyti CHECK. Ant žemės rašomi tikri identifikuoti bonusai. Socketų kiekiai, ribos ir Larzuk/Puzzle/WSS/Cube pagalba šviesiai mėlyni; klasės RW rekomendacijos ir receptai žali. Maksimali socketų talpa negarantuoja socketinimo rezultato. Superior bazėms netaikomas tik normal kokybei skirtas random socket Cube receptas.

**[owned grail]** rodoma prie Unique/Set daikto vardo ir ant žemės, ir inventoriuje. Ji naudoja dabartinę PD2 Unique/Set kolekcijos turėjimo būseną, ne atradimų istoriją ar savarankišką stash skenavimą. Atnaujinimo laikas pardavus paskutinę kopiją dar tikrinamas žaidime. Item level rašomas aprašymo apačioje.


### Socketų suteikimo būdai

Tinkami daiktai be socketų rodo pilną metodo pavadinimą ir šiai bazei galimą rezultatą. Pavyzdžiui, Stealskull su dviejų socketų talpa gali rodyti:

| Metodas | Rezultatas šiam pavyzdžiui | Kaip naudoti |
| --- | --- | --- |
| Larzuk quest (Act 5) | 1 socketas | Pasinaudok Act 5 socketų užduoties atlygiu pas Larzuk. |
| Larzuk's Puzzlebox | 1–2 socketai | Daiktą ir šį įrankį sudėk į Horadric Cube. |
| Larzuk's Malus | 1 socketas | Daiktą ir Larzuk's Malus sudėk į Cube; tai daiktas, ne užduotis. |

Ne Unique/Set kandidatams rekomenduojamas tinkamas **Larzuk's Puzzlepiece**. Rezultatas priklauso nuo kokybės, ginklo tipo ir talpos — Stealskull pavyzdys netinka visiems daiktams. Jau socketinti daiktai rodo trumpai Sockets: N/M. Worldstone Shard corruption yra atskiras rizikingas būdas.

### Owned Grail

**[owned grail]** padeda atpažinti turimų Unique ir Set kolekcijos kopijas. Žyma rodoma prie vardo **ant žemės ir inventoriuje**, o aprašyme — **Owned Grail: owned**. Išlieka vardas, palaikomas ROLL ir kainų informacija.

| Situacija | Ką reiškia žyma |
| --- | --- |
| Identifikuotas Unique/Set | PD2 native kolekcijos būsena patvirtina, kad šį konkretų variantą šiuo metu turi. |
| Neidentifikuotas Unique/Set | Žymima tik jei PD2 patvirtina visų galimų nežinomo drop variantų turėjimą. Neaiškūs kandidatai nežymimi. |
| Žymos nėra | Turėjimas nepatvirtintas. Tai neįrodo, kad niekada neradai ar kad daikto nėra nė viename stash. |
| Parduota ar pašalinta paskutinė kopija | Žyma dingsta, kai PD2 atnaujina turėjimo būseną. Ar iškart, ar po naujo prisijungimo — žaidime dar nepatikrinta. |
| Kita kopija liko | Žyma remiasi PD2 likusio turėjimo būsena. Melindaa savarankiškai neskenuoja visų stash tabų. |
| Kadaise rastas, paskui parduotas | Tai dabartinis turėjimas, ne atradimų istorija, nuolatinis grail pasiekimas ar radimų skaitiklis. |
| Geresnis naujos kopijos roll | Palygink rodomus status/ROLL pats. Turėjimo žyma negrąžina laikomos kopijos roll, todėl iš jos automatinio pagerėjimo procento apskaičiuoti negalime. |

**Owned Grail neslepia Unique daiktų.** Set rodymas priklauso nuo strictness; pati žyma daiktų neslepia. Reikia PD2 native palaikymo ir atnaujinto, perkrauto filtro.


### Diegimas ir atnaujinimas

1. Išarchyvuok naujausią ZIP/RAR ir nukopijuok **Melindaa.filter** į **C:\Diablo II\ProjectD2\filters\local** (arba savo žaidimo vietą).
2. PD2 launcheryje pasirink **Item Filter Profiles → Local Filter → Melindaa.filter → Save**.
3. Paleisk žaidimą iš naujo arba naudok savo nustatytą **Reload Loot Filter** valdymą. Kubo aprašyme patikrink **v1.2.74**.
4. Strictness keičiamas **Increase Filter Level / Decrease Filter Level**, esančiais **Esc → Options → Configure Controls**. Filtras pats klavišų nepriskiria.

[MIT licencijos įrašas](./MIT-NOTICE.txt)

### Practical runeword bases / Praktiškos runeword bazės

**English:** From Farming, recommendations use an explicit practical base/RW shortlist instead of every legal recipe. Examples: CTA Crystal Sword/Flail or staff-mod War Scepter; HOTO Flail; Enigma Mage Plate/Dusk Shroud/Archon Plate; Faith Gorgon Crossbow/selected bows; merc Insight/Infinity/Pride/Obedience on selected elite polearms/spears where legal; Fortitude/Innocence on selected armor. Insight is not recommended on caster staves. Generic Wind on arbitrary melee bases is removed; Fury targets selected claws. Mercenary candidates show Merc RW on the ground and Possible merc RW in recipe help. Earlier profiles include more starter recipes, but caster/merc base-purpose checks apply at every level; Insight is never recommended on caster staves, HOTO uses Flail, and Lore retains eligible starter helms. Existing quality/socket thresholds still apply: popular does not mean any roll/socket layout qualifies. The shortlist uses game compatibility and a bounded current completed-RW trade sample, not a global popularity census. No other loot-filter rules are build inputs.

**Lietuviškai:** Nuo Farming rekomendacijos remiasi konkrečiu praktinių bazės/RW derinių sąrašu, ne visais techniškai galimais receptais. Pavyzdžiai: CTA Crystal Sword/Flail arba staffmod War Scepter; HOTO Flail; Enigma Mage Plate/Dusk Shroud/Archon Plate; Faith Gorgon Crossbow/atrinktuose lankuose; merc Insight/Infinity/Pride/Obedience atrinktose elite polearm/spear bazėse, kai leidžia receptas; Fortitude/Innocence atrinktuose šarvuose. Caster staff nebesiūlomas Insight. Bendras Wind bet kokiems melee ginklams pašalintas; Fury paliekamas atrinktoms claws. Merc kandidatams ant žemės rodoma Merc RW, receptuose Possible merc RW. Ankstesni lygiai rodo daugiau starter receptų, bet caster/merc bazių paskirtis tikrinama visur: staff nebesiūlomas Insight, HOTO siejamas su Flail, o Lore paliekamas tinkamiems starter šalmams. Kokybės/socket ribos galioja: populiari bazė nereiškia bet kokio roll/socket varianto. Sąrašas remiasi žaidimo suderinamumu ir ribota dabartinių pagamintų RW prekybos imtimi, ne visų žaidėjų populiarumo statistika. Kitų filtrų taisyklės generatoriui nenaudojamos.

Farming retains selected plain ETH elite merc weapons and low-requirement caster/buff bases even without enhanced damage; Endgame keeps the stricter perfect-bonus requirement; 0 sockets are allowed, existing sockets must match a selected recipe.

Farming palieka atrinktus paprastus ETH elite merc ginklus ir mažų reikalavimų caster/buff bazes net be enhanced damage; Endgame lieka perf bonusų reikalavimas; leidžiami 0 socketų, o esami socketai turi tikti atrinktam receptui.

Ground resistance labels use Fire res / Cold res / Light res / Poison res for clarity.

Atsparumai ant žemės rašomi Fire res / Cold res / Light res / Poison res, kad nereikėtų spėlioti trumpinių.

**v1.2.71:** Endgame now accepts selected perfect unsocketed RW bases when capacity supports a practical recipe. Existing sockets must match a selected recipe exactly; bonus quality, special-drop protection and all other profiles remain unchanged. Socket capacity is not a guaranteed socketing result.

**v1.2.71:** Endgame leidžia atrinktas perf RW bazes be socketų, kai jų talpa leidžia praktišką receptą. Esami socketai turi tiksliai atitikti atrinktą receptą; bonusų kokybė, PD2 apsaugos ir kiti profiliai nepakeisti. Talpa negarantuoja socketinimo rezultato.


### Launcher metadata / Launcher metaduomenys

[`filters.json`](./filters.json) contains our single registration entry for the official PD2 list. `filter_definitions.json` describes the single `Melindaa.filter` choice. The launcher registration uses the official `name`, `url`, `author` format with the repository contents API URL. Inclusion in the official launcher list still requires PD2 approval. Missing supported estimates display **Estimated price: in development**; existing numeric estimates keep their original data dates.

[`filters.json`](./filters.json) pateikia vienintelį mūsų registracijos įrašą oficialiam PD2 sąrašui. `filter_definitions.json` aprašo vienintelį `Melindaa.filter` pasirinkimą. Launcher registracijos įrašas naudoja oficialų `name`, `url`, `author` formatą ir repozitoriumo contents API adresą. Įtraukimui į oficialų launcher sąrašą dar reikalingas PD2 patvirtinimas. Kai palaikomo įverčio nėra, rodoma **Estimated price: in development**; esamų skaitinių įverčių duomenų datos išlieka.
