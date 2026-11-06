# Kiela filter specification / Filtro specifikacija

## English

Current policy: **v1.2.71**, seven profiles: Normal, Nightmare, Hell, Baal Runs, Farming with Blue, Farming without Blue and Endgame. See the [profile table and installation guide](./README.md).

### Permanent visibility

All profiles show all uniques, including Endgame, so players can collect their unique-item grail. All runes, charms, jewels, jewel fragments and protected PD2 special drops remain visible regardless of equipment roll thresholds. These include maps, map-upgrade materials and orbs, corruption/socket tools, crafting materials, fragments, boss keys, organs and essences. Inventory items remain inspectable.

### Rare equipment and identification

Farming and Endgame preserve **all unidentified rare equipment**, including lower-level bases. Their actual hidden properties cannot be evaluated before identification. Kiela intentionally accepts more ground clutter to reduce the risk of missing an item that becomes valuable when identified. Some stricter approaches hide more unidentified rare bases and accept that risk; this is not a claim about every filter or a guarantee of value.

After identification, Farming requires relevant combinations for the equipment slot, rather than a universal count of property lines. Endgame requires stronger combinations and **at least 90% when the owned rare ROLL model supports reliable grading**. A property line is not an affix slot. Unsupported or modified rolls do not receive an invented percentage; conservative exceptions remain. Charms and jewels are exempt.

### Set items

- **Both Farming profiles: all sets remain visible.**
- **Endgame: selected higher-tier/useful set candidates.** Known lower-tier sets are hidden. Reliably supported variable rolls must reach 90%; fixed selected sets have no variable roll to grade.
- Unidentified bases shared with eligible sets remain candidates. A base known to contain only excluded sets can be hidden. Ambiguous identities and unsupported/modified roll cases retain safety exceptions; these exceptions do not make every low-tier set eligible.

### Magic equipment and completed crafts

Craft-only blue bases stop after Baal Runs. Farming with Blue uses Kiela's independent useful skill/speed, caster, physical and socket/life/block signatures plus unidentified affix-potential candidates. Farming without Blue and Endgame hide all ordinary Magic equipment/jewelry, identified or not. Charms, jewels and protected PD2 specials remain visible. All completed orange crafts stay visible at every level. The two Farming modes share Rare/Set/RW selection. Gold: 2000 / 3000 / 4000 at levels 5 / 6 / 7.

### Runeword bases

From Farming, a base must suit Kiela's advanced-recipe selection and meet its relevant quality requirements. Advanced recipes here use a Pul-or-later rune; this is a selection boundary, not a market-value claim. Starter-only bases, including those only useful for Lore, no longer qualify. Selected low-requirement caster/buff bases remain useful exceptions, including CTA swords and HOTO flails.

Endgame additionally requires maximum relevant base bonuses and actual recipe-compatible sockets. Relevant maxima depend on the item: enhanced damage/defense, class-skill properties or Paladin automagic where applicable. This does not promise a perfect combination of every possible stat. A high item level alone does not qualify a base.

Class recommendations and required runes are green; generic compatible options are gray. The filter recognizes class, not the player's exact build. Unsocketed bases still need the stated socket count.

### Progression and consumables

Normal/Nightmare show all items. Hell/Baal use cautious equipment guidance without a universal item-level-85 cutoff and show Flawless/Perfect gems. Farming/Endgame show only Perfect gems. Gold minimums are 2,000 and 3,000 respectively. Hell hides loose ID/TP scrolls and Stamina/Thawing/Oil potions. Farming also hides ordinary HP/MP, Antidote and cold/gas/fire throwing potions; both rejuvenation sizes remain.

Stack labels appear only for quantities above one, e.g. `5x Worldstone Shard`. Item level appears as plain text at the bottom of descriptions. Charm/skiller, magic-jewel and supported RW-base quotes use a five-day (120-hour) listing/bump window and five-day snapshot validity at build/update time. Exact matches take priority over approximate pooled-roll mod groups. Supported RW-base quotes distinguish base, socket count, ETH, Normal/Superior and ED/durability bands, pooling base-defense rolls; they do not price filled/corrupted bases. Unknown quotes are stated explicitly, never inferred from NPC gold. Baseline unique/set data retains its original date.

### Initialization and validation

Repeated expressions are compiled through shared named formulas; RW eligibility is dispatched without repeating the full base-selection condition for every recipe. This reduces structural initialization work. First-game loading and connection behavior still require an actual game test. Automated checks cover native single-pass aliases, formula bindings, equipment transitions, protected special drops, recipes and duplicate directives. Other loot filters are not build inputs. Common game syntax is not by itself evidence of copied authorship, and comparison audits do not prove universal originality.

## Lietuviškai

Dabartinė politika: **v1.2.71**, septyni profiliai: Normal, Nightmare, Hell, Baal Runs, Farming with Blue, Farming without Blue ir Endgame. [Profilių lentelė ir diegimas](./README.md#lietuviškai).

### Kas visada matoma

Visuose profiliuose, įskaitant Endgame, rodomi visi unique, kad būtų galima rinkti unique grail kolekciją. Visada lieka runos, charmai, jewels, jewel fragmentai ir saugomi PD2 specialūs daiktai: mapai, jų upgrade medžiagos ir orbai, corruption/socket įrankiai, craft medžiagos, fragmentai, boss keys, organai ir essences. Įrangos roll ribos jų neslepia. Inventoriaus daiktus galima apžiūrėti.

### Rare ir identifikavimas

Farming ir Endgame palieka **visą neidentifikuotą rare įrangą**, taip pat žemesnio lygio bazes. Tikrų paslėptų savybių prieš identifikavimą įvertinti negalime. Sąmoningai rodome daugiau daiktų, kad sumažintume vertingo rare praradimo riziką. Kai kurie griežtesni atrankos būdai slepia daugiau neidentifikuotų rare bazių ir priima šią riziką; tai nėra teiginys apie kiekvieną filtrą ar garantuota daikto vertė.

Identifikavus Farming vertina kategorijai naudingus derinius, ne universalų savybių eilučių skaičių. Endgame reikalauja stipresnių derinių ir **bent 90%, kai mūsų rare ROLL modelis leidžia patikimai įvertinti rezultatą**. Savybės eilutė nėra tas pats kaip affix vieta. Nepalaikomiems ar pakeistiems roll procento neišgalvojame; paliekamos atsargios išimtys. Charmai ir jewels nuo šių ribų apsaugoti.

### Set daiktai

- **Farming Strict rodo visus set.**
- **Endgame atrenka aukštesnio lygio/naudingus set.** Žinomi žemos vertės šablonai slepiami. Palaikomiems ir patikimai vertinamiems kintamiems roll reikia 90%; atrinkti fiksuotų savybių set neturi kintamo procento.
- Neidentifikuotos bendros bazės paliekamos, jeigu jose gali būti tinkamas set. Bazę, kuri turi tik atmestus set, galima slėpti. Neaiški tapatybė ir nepalaikomi/pakeisti roll vertinami atsargiau; tai nėra bendras leidimas visiems prastiems set.

### Magic įranga ir pagaminti craft

Mėlynų bazių rodymas vien craftinimui baigiasi po Baal Runs. Farming slepia visus Magic ginklus, šalmus/circlet/klasių šalmus, diržus, batus, pirštines ir skydus, ID ir unID nepaisant bonusų. Atrinkti Magic žiedai, amuletai, kūno šarvai ir quiver lieka. Endgame slepia visus Magic žiedus, amuletus, skydus, ginklus, diržus, pirštines, batus ir šalmus, įskaitant circlet ir klasių šalmus, ID ir unID, nepaisant bonusų. Magic kūno šarvų ir quiver atranka išlieka atskira. Vien craft potencialas atrankos neapeina. Charmai, jewels ir saugomi magic PD2 mapai/medžiagos lieka. Visi jau pagaminti oranžiniai crafted daiktai matomi visuose lygiuose; jie gali būti naudingi ir Endgame, o mėlyna craft bazė yra kitas dalykas.

### Runeword bazės

Nuo Farming bazė turi tikti mūsų pažangių receptų atrankai ir atitikti aktualią kokybę. Šiai atrankai pažangus receptas naudoja Pul arba vėlesnę runą; tai atrankos riba, ne rinkos kainos teiginys. Tik starter receptams, pvz., Lore, tinkamos bazės neberodomos. Paliekamos naudingos žemų reikalavimų caster/buff išimtys, įskaitant CTA kardus ir HOTO flailus.

Endgame papildomai reikia maksimalių aktualių bazės bonusų ir tikrų receptui tinkamų socketų. Aktualūs maksimumai priklauso nuo bazės: enhanced damage/defense, klasės skill ar Paladin automagic. Tai nereiškia tobulo visų galimų savybių derinio. Vien aukštas item level bazės neišsaugo.

Klasei rekomenduojami RW ir runos žali, bendri tinkami variantai pilki. Atpažįstama klasė, ne tikslus build. Bazei be socketų vis dar reikia nurodyto jų skaičiaus.

### Progresas ir vartojami daiktai

Normal/Nightmare rodo viską. Hell/Baal naudoja atsargias įrangos gaires be bendros item level 85 ribos; rodo Flawless/Perfect gemus. Farming/Endgame rodo tik Perfect gemus. Gold minimumai atitinkamai 2 000 ir 3 000. Hell slepia palaidus ID/TP scrolls ir Stamina/Thawing/Oil potionus. Farming papildomai slepia įprastus HP/MP, Antidote ir cold/gas/fire throwing potionus; abu rejuvenation dydžiai lieka.

Kiekis rodomas tik krūvelėms nuo 2 vnt., pvz., `5x Worldstone Shard`. Item level rašomas paprastu tekstu aprašymo apačioje. Charmų/skillerių, magic jewels ir palaikomų RW bazių kainos naudoja 5 parų (120 val.) skelbimų/atnaujinimų langą bei 5 parų įverčio galiojimą kūrimo/atnaujinimo metu. Tikslūs deriniai turi pirmenybę prieš apytiksles modų grupes. RW bazėms atskiriama bazė, socketai, ETH, Normal/Superior ir ED/durability ribos, sujungiami defense roll; užpildytoms/corrupted bazėms šis įvertis netaikomas. Nežinomas įvertis pažymimas aiškiai, ne išvedamas iš NPC gold. Bazinės unique/set kainos išlaiko pradinę datą.

### Inicializavimas ir patikra

Pasikartojančios išraiškos naudoja bendras vardines formules; pilna RW bazės atranka nebekartojama prie kiekvieno recepto. Tai mažina inicializavimo darbą. Pirmo žaidimo krovimą ir ryšį dar reikia patikrinti žaidime. Automatinė patikra apima native vienos eigos alias, formulių nuorodas, įrangos būsenas, specialių daiktų apsaugą, receptus ir dublikatus. Kiti filtrai nėra kūrimo įvestis. Bendra žaidimo sintaksė savaime nereiškia kopijavimo, o palyginimas neįrodo absoliutaus originalumo.

## v1.2.62 details / Papildymai

**English:** Ground tags use compact actual stats, including `max dmg 1`, `min dmg 8` and `Ltng1-5`. All quotes say Estimated price. Baseline unique/set quotes are not individualized to roll/corruption/sockets. Fresh material/map quotes use unmodified plain-map samples and unambiguous per-item offers; rolled maps are not priced as plain. Rare/crafted comparable intervals preserve skill/element identities, base/quality/ETH/socket identity and core bands, with minimum three listings/two sellers. Broader core comparisons explicitly pool secondary properties. Missing comparable evidence retains an unsupported-quote explanation. Practical RW targets are an independently curated use-case shortlist, intersected with game recipe compatibility; this is not a measured global usage ranking. Exact sockets are mandatory; Superior random-Cube instructions are excluded by the installed CubeMain quality requirement. `[owned grail]` uses native ALLOWNED, never DISCOVERED; ambiguous unID variants are not claimed owned. No find counter is provided.

**Lietuviškai:** Ant žemės rodoma trumpai, pvz., `max dmg 1`, `min dmg 8`, `Ltng1-5`. Visos kainos vadinamos Estimated price. Baziniai unique/set įverčiai nepritaikyti konkrečiam roll/corruption/socket. Mapų ir medžiagų įverčiai naudoja paprastus nepakeistus mapus ir aiškias vieneto kainas; išridenti mapai nekainuojami kaip paprasti. Rare/crafted palyginimai saugo skill/elemento, bazės/kokybės/ETH/socket tapatybę ir pagrindinių modų ribas; reikia bent 3 skelbimų/2 pardavėjų. Platesni palyginimai aiškiai sujungia antrines savybes. Kai palyginamų duomenų nėra, paliekamas paaiškinimas be išgalvotos kainos. RW sąrašai savarankiškai atrinkti pagal paskirtį ir suderinti su žaidimo receptais; tai nėra išmatuotas visų žaidėjų naudojimo reitingas. Reikia tikslių socketų; Superior random Cube receptas atmetamas pagal CubeMain kokybės ribą. `[owned grail]` naudoja native ALLOWNED, ne DISCOVERED; neaiškūs neidentifikuoti variantai nežymimi kaip tikrai turimi. Radimų skaitiklio nėra.

White/gray bases at Farming/Endgame must pass the RW-base selection even with skill bonuses or only one socket.

Baltos/pilkos bazės Farming/Endgame lygiuose turi atitikti RW atranką net turėdamos skill bonusų ar tik vieną socketą.

## v1.2.71 ownership labels / Nuosavybės žymos

**English:** Unique/Set names show [owned grail] on the ground and in inventory when native ALLOWNED confirms ownership. Pricing and roll details are preserved. The native ownership flag does not provide the owned copy’s stats/roll, so no automatic better-than-owned percentage is claimed.

**Lietuviškai:** Unique/Set vardai žymimi [owned grail] ant žemės ir inventoriuje, kai native ALLOWNED patvirtina turėjimą. Kainos ir roll informacija išsaugomi. Turėjimo žyma negrąžina turimos kopijos statų/roll, todėl automatinis procentinis palyginimas su ja neteikiamas.

## v1.2.71 current update / Dabartinis atnaujinimas

**English:** Seven profiles; the two Farming modes differ in ordinary blue gear and gold pickup threshold. Both show all Set, all unidentified Rare and completed Craft. Endgame is level 7 with supported identified Rare/selected Set 90% and perfect RW bases (unsocketed or with matching sockets). Prior six-profile Endgame selections migrate once to 7. Gold-only Magic charms have no numeric quote; sparse seller offers are not reliable value evidence. Craft ingredients use Crafting material, gem recipe lines use their gem colors, socket counts use Sockets: N/M. Existing ownership and protections remain.

**Lietuviškai:** Septyni profiliai; abu Farming skiriasi įprastos mėlynos įrangos matomumu ir gold riba. Abu rodo visus Set, neidentifikuotus Rare ir pagamintus Craft. Endgame yra 7 lygis su palaikomų identifikuotų Rare/atrinktų Set 90% ir perf RW bazėmis (be socketų arba su tinkamais socketais). Ankstesnis šešių profilių Endgame vieną kartą perkeliamas į 7. Tik Gold turintiems Magic charmams skaitinė kaina nerodoma: keli pardavėjų pasiūlymai neįrodo vertės. Ingredientai žymimi Crafting material, gemų receptai jų spalvomis, socketai Sockets: N/M. Ankstesnės owned žymos ir apsaugos išlieka.

### Practical runeword bases / Praktiškos runeword bazės

**English:** From Farming, recommendations use an explicit practical base/RW shortlist instead of every legal recipe. Examples: CTA Crystal Sword/Flail or staff-mod War Scepter; HOTO Flail; Enigma Mage Plate/Dusk Shroud/Archon Plate; Faith Gorgon Crossbow/selected bows; merc Insight/Infinity/Pride/Obedience on selected elite polearms/spears where legal; Fortitude/Innocence on selected armor. Insight is not recommended on caster staves. Generic Wind on arbitrary melee bases is removed; Fury targets selected claws. Mercenary candidates show Merc RW on the ground and Possible merc RW in recipe help. Earlier profile recipes remain broader. Existing quality/socket thresholds still apply: popular does not mean any roll/socket layout qualifies. The shortlist uses game compatibility and a bounded current completed-RW trade sample, not a global popularity census. No other loot-filter rules are build inputs.

**Lietuviškai:** Nuo Farming rekomendacijos remiasi konkrečiu praktinių bazės/RW derinių sąrašu, ne visais techniškai galimais receptais. Pavyzdžiai: CTA Crystal Sword/Flail arba staffmod War Scepter; HOTO Flail; Enigma Mage Plate/Dusk Shroud/Archon Plate; Faith Gorgon Crossbow/atrinktuose lankuose; merc Insight/Infinity/Pride/Obedience atrinktose elite polearm/spear bazėse, kai leidžia receptas; Fortitude/Innocence atrinktuose šarvuose. Caster staff nebesiūlomas Insight. Bendras Wind bet kokiems melee ginklams pašalintas; Fury paliekamas atrinktoms claws. Merc kandidatams ant žemės rodoma Merc RW, receptuose Possible merc RW. Ankstesnių lygių receptai platesni. Kokybės/socket ribos galioja: populiari bazė nereiškia bet kokio roll/socket varianto. Sąrašas remiasi žaidimo suderinamumu ir ribota dabartinių pagamintų RW prekybos imtimi, ne visų žaidėjų populiarumo statistika. Kitų filtrų taisyklės generatoriui nenaudojamos.

Farming retains selected plain ETH elite merc weapons and low-requirement caster/buff bases even without enhanced damage; Endgame keeps the stricter perfect-bonus requirement; 0 sockets are allowed, existing sockets must match a selected recipe.

Farming palieka atrinktus paprastus ETH elite merc ginklus ir mažų reikalavimų caster/buff bazes net be enhanced damage; Endgame lieka perf bonusų reikalavimas; leidžiami 0 socketų, o esami socketai turi tikti atrinktam receptui.

Ground resistance labels use Fire res / Cold res / Light res / Poison res for clarity.

Atsparumai ant žemės rašomi Fire res / Cold res / Light res / Poison res, kad nereikėtų spėlioti trumpinių.

**v1.2.71:** Endgame now accepts selected perfect unsocketed RW bases when capacity supports a practical recipe. Existing sockets must match a selected recipe exactly; bonus quality, special-drop protection and all other profiles remain unchanged. Socket capacity is not a guaranteed socketing result.

**v1.2.71:** Endgame leidžia atrinktas perf RW bazes be socketų, kai jų talpa leidžia praktišką receptą. Esami socketai turi tiksliai atitikti atrinktą receptą; bonusų kokybė, PD2 apsaugos ir kiti profiliai nepakeisti. Talpa negarantuoja socketinimo rezultato.
