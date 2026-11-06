# Kiela v1.2.70

## English

Project Diablo 2 loot filter with our own equipment selection, dated HR/WSS estimates, supported ROLL ratings, actual ground bonuses, crafting help and class-aware runeword recommendations.

**[Download ZIP](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)** · **[Download RAR](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** · **[Changelog](./CHANGELOG.md)** · **[Full filter specification](./FILTER-SPECIFICATION.md)**

### Choose your strictness

| Level | Profile | What it shows and hides |
| --- | --- | --- |
| 1 | Normal | Shows all items. |
| 2 | Nightmare | Shows all items. |
| 3 | Hell | Broad useful Magic/Rare candidates and cautious unidentified potential. Flawless and Perfect gems. Hides Stamina, Thawing, Oil and loose ID/TP scrolls. |
| 4 | Baal Runs | Tighter equipment and plain-base selection than Hell. Flawless and Perfect gems. Useful crafting candidates can still appear. |
| 5 | Farming with Blue | Selected useful Magic combinations and unidentified candidates: skill + speed/cast, socket/block/life and strong weapon candidates. Useful Rare; all Unique/Set/Craft. Good advanced RW bases and CTA/HOTO exceptions. Perfect gems; gold 2,000+. |
| 6 | Farming without Blue | Hides all ordinary Magic equipment and jewelry, identified or not. Charms, jewels and PD2 specials remain. Same Rare/Set/RW selection as Farming with Blue. Perfect gems; gold 3,000+. |
| 7 | Endgame | Hides ordinary Magic gear/jewelry. Stronger identified Rare; selected useful Set; supported Rare/Set roll 90%+. All Unique/Craft and unidentified Rare kept. Perfect relevant RW bonuses + matching sockets. Perfect gems; gold 4,000+. |

**Always visible at every level:** all Unique items for grail collecting, completed orange Crafted items, runes, charms, jewels, protected PD2 maps/materials/fragments/boss ingredients/socket tools, both Rejuvenation potions and **Antidote potions**. Inventory items remain inspectable.

**Farming and Endgame keep all unidentified Rare equipment.** Hidden affixes are not graded. After identification, selection depends on relevant combinations for the equipment category. Unsupported or modified rolls are not assigned an invented percentage. Endgame's 90% requirement applies only where reliable grading is supported.

Farming/Endgame hide ordinary HP/MP potions, cold/gas/fire throwing potions and player ears. Endgame also hides ordinary chest keys. Both retain protected boss keys and special materials. Farming keeps all Set items; Endgame selects useful higher-tier candidates and handles ambiguous unidentified variants conservatively.

### Latest changes, v1.2.63–v1.2.70

- Added Farming with Blue / Farming without Blue; Endgame is now level 7. Gold thresholds from Farming are 2,000 / 3,000 / 4,000. Existing Endgame selections migrate safely.
- Pure Gold Find-only charms show no reliable price instead of a misleading numeric quote.
- Ingredients use Crafting material; gem recipes use their gem colors; socketed items show Sockets: N/M.
- [owned] appears beside Unique/Set names on the ground and in inventory.
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

The **[owned]** marker appears beside Unique/Set item names both on the ground and in inventory. It uses PD2's current Unique/Set collection state, not discovery history or an independent stash scan. Update timing after selling the last copy still needs in-game verification. Item level appears at the bottom of descriptions.

### Install or update

1. Extract the latest ZIP/RAR and copy **Kiela.filter** into **C:\Diablo II\ProjectD2\filters\local** (adjust for your installation).
2. Choose **Item Filter Profiles → Local Filter → Kiela.filter → Save** in the PD2 launcher.
3. Start/restart PD2, or use your configured **Reload Loot Filter** control. Check **v1.2.70** in the Horadric Cube description.
4. Change strictness with **Increase Filter Level / Decrease Filter Level** under **Esc → Options → Configure Controls**. The filter does not bind keys automatically.

[Required attribution and rights](./THIRD-PARTY-NOTICES.md) · [MIT license notice](./LICENSE-UPSTREAM-MIT.txt)

## Lietuviškai

Project Diablo 2 filtras su mūsų sukurta įrangos atranka, datuotais HR/WSS kainų įverčiais, palaikomais ROLL vertinimais, tikrais bonusais ant žemės, craft pagalba ir klasei pritaikytomis runeword rekomendacijomis.

**[Atsisiųsti ZIP](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)** · **[Atsisiųsti RAR](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** · **[Pakeitimai](./CHANGELOG.md)** · **[Visa filtro specifikacija](./FILTER-SPECIFICATION.md)**

### Pasirink strictness lygį

| Lygis | Profilis | Ką rodo ir slepia |
| --- | --- | --- |
| 1 | Normal | Rodo visus daiktus. |
| 2 | Nightmare | Rodo visus daiktus. |
| 3 | Hell | Platesnė naudingų Magic/Rare ir neidentifikuotų kandidatų atranka. Flawless ir Perfect gemai. Slepia Stamina, Thawing, Oil ir palaidus ID/TP scrolls. |
| 4 | Baal Runs | Griežtesnė įrangos ir paprastų bazių atranka negu Hell. Flawless ir Perfect gemai. Naudingi craft kandidatai dar gali būti rodomi. |
| 5 | Farming with Blue | Atrinkti naudingi Magic deriniai ir neidentifikuoti kandidatai: skill + speed/cast, socket/block/life bei stiprių ginklų kandidatai. Naudingi Rare; visi Unique/Set/Craft. Geros pažangių RW bazės ir CTA/HOTO išimtys. Tik Perfect gemai; gold nuo 2 000. |
| 6 | Farming without Blue | Slepia visą įprastą Magic įrangą ir jewelry, ID ir unID. Charmai, jewels ir PD2 specialūs daiktai lieka. Rare/Set/RW atranka tokia pati kaip Farming with Blue. Tik Perfect gemai; gold nuo 3 000. |
| 7 | Endgame | Slepia įprastą Magic įrangą/jewelry. Stipresni identifikuoti Rare ir atrinkti naudingi Set; palaikomas Rare/Set roll 90%+. Visi Unique/Craft ir neidentifikuoti Rare lieka. RW: maksimalūs aktualūs bonusai + tinkami socketai. Tik Perfect gemai; gold nuo 4 000. |

**Visuose lygiuose rodomi:** visi Unique grail kolekcijai, jau pagaminti oranžiniai Crafted, runos, charmai, jewels, saugomi PD2 mapai/medžiagos/fragmentai/boss ingredientai/socket įrankiai, abu Rejuvenation ir **Antidote potionai**. Inventoriuje daiktai neslepiami.

**Farming ir Endgame palieka visą neidentifikuotą Rare įrangą.** Paslėpti modai nevertinami. Identifikavus tikrinami įrangos kategorijai naudingi deriniai. Nepalaikomiems ar pakeistiems roll neišgalvojamas procentas. Endgame 90% riba taikoma tik patikimai palaikomam vertinimui.

Farming/Endgame slepia įprastus HP/MP, cold/gas/fire throwing potionus ir player ears. Endgame papildomai slepia įprastus chest keys. Boss raktai ir saugomos medžiagos išlieka. Farming rodo visus Set; Endgame atrenka naudingus aukštesnio lygio kandidatus, o neaiškius neidentifikuotus variantus vertina atsargiai.

### Naujausi pakeitimai, v1.2.63–v1.2.70

- Pridėti Farming with Blue / Farming without Blue; Endgame dabar 7 lygis. Gold nuo Farming: 2 000 / 3 000 / 4 000. Ankstesnis Endgame pasirinkimas saugiai perkeliamas.
- Tik Gold Find turintys charmai rodo, kad patikimos kainos nėra, vietoj klaidinančio skaičiaus.
- Ingredientai žymimi Crafting material; gemų receptams naudojamos jų spalvos; socketinti daiktai rodo Sockets: N/M.
- [owned] rodoma prie Unique/Set vardų ant žemės ir inventoriuje.
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

**[owned]** rodoma prie Unique/Set daikto vardo ir ant žemės, ir inventoriuje. Ji naudoja dabartinę PD2 Unique/Set kolekcijos turėjimo būseną, ne atradimų istoriją ar savarankišką stash skenavimą. Atnaujinimo laikas pardavus paskutinę kopiją dar tikrinamas žaidime. Item level rašomas aprašymo apačioje.

### Diegimas ir atnaujinimas

1. Išarchyvuok naujausią ZIP/RAR ir nukopijuok **Kiela.filter** į **C:\Diablo II\ProjectD2\filters\local** (arba savo žaidimo vietą).
2. PD2 launcheryje pasirink **Item Filter Profiles → Local Filter → Kiela.filter → Save**.
3. Paleisk žaidimą iš naujo arba naudok savo nustatytą **Reload Loot Filter** valdymą. Kubo aprašyme patikrink **v1.2.70**.
4. Strictness keičiamas **Increase Filter Level / Decrease Filter Level**, esančiais **Esc → Options → Configure Controls**. Filtras pats klavišų nepriskiria.

[Privalomi autorių ir teisių įrašai](./THIRD-PARTY-NOTICES.md) · [MIT licencijos įrašas](./LICENSE-UPSTREAM-MIT.txt)

### Practical runeword bases / Praktiškos runeword bazės

**English:** From Farming, recommendations use an explicit practical base/RW shortlist instead of every legal recipe. Examples: CTA Crystal Sword/Flail or staff-mod War Scepter; HOTO Flail; Enigma Mage Plate/Dusk Shroud/Archon Plate; Faith Gorgon Crossbow/selected bows; merc Insight/Infinity/Pride/Obedience on selected elite polearms/spears where legal; Fortitude/Innocence on selected armor. Insight is not recommended on caster staves. Generic Wind on arbitrary melee bases is removed; Fury targets selected claws. Mercenary candidates show Merc RW on the ground and Possible merc RW in recipe help. Earlier profile recipes remain broader. Existing quality/socket thresholds still apply: popular does not mean any roll/socket layout qualifies. The shortlist uses game compatibility and a bounded current completed-RW trade sample, not a global popularity census. No other loot-filter rules are build inputs.

**Lietuviškai:** Nuo Farming rekomendacijos remiasi konkrečiu praktinių bazės/RW derinių sąrašu, ne visais techniškai galimais receptais. Pavyzdžiai: CTA Crystal Sword/Flail arba staffmod War Scepter; HOTO Flail; Enigma Mage Plate/Dusk Shroud/Archon Plate; Faith Gorgon Crossbow/atrinktuose lankuose; merc Insight/Infinity/Pride/Obedience atrinktose elite polearm/spear bazėse, kai leidžia receptas; Fortitude/Innocence atrinktuose šarvuose. Caster staff nebesiūlomas Insight. Bendras Wind bet kokiems melee ginklams pašalintas; Fury paliekamas atrinktoms claws. Merc kandidatams ant žemės rodoma Merc RW, receptuose Possible merc RW. Ankstesnių lygių receptai platesni. Kokybės/socket ribos galioja: populiari bazė nereiškia bet kokio roll/socket varianto. Sąrašas remiasi žaidimo suderinamumu ir ribota dabartinių pagamintų RW prekybos imtimi, ne visų žaidėjų populiarumo statistika. Kitų filtrų taisyklės generatoriui nenaudojamos.

Farming retains selected plain ETH elite merc weapons and low-requirement caster/buff bases even without enhanced damage; Endgame keeps the stricter perfect-bonus/socket requirement.

Farming palieka atrinktus paprastus ETH elite merc ginklus ir mažų reikalavimų caster/buff bazes net be enhanced damage; Endgame lieka perf bonusų ir tinkamų socketų reikalavimas.

Ground resistance labels use Fire res / Cold res / Light res / Poison res for clarity.

Atsparumai ant žemės rašomi Fire res / Cold res / Light res / Poison res, kad nereikėtų spėlioti trumpinių.
