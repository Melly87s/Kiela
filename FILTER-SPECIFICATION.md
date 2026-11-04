# Kiela filter specification / Filtro specifikacija

## English

Current policy: **v1.2.58**, six profiles: Normal, Nightmare, Hell, Baal Runs, Farming Strict and Endgame. See the [profile table and installation guide](./README.md).

### Permanent visibility

All profiles show all uniques, including Endgame, so players can collect their unique-item grail. All runes, charms, jewels, jewel fragments and protected PD2 special drops remain visible regardless of equipment roll thresholds. These include maps, map-upgrade materials and orbs, corruption/socket tools, crafting materials, fragments, boss keys, organs and essences. Inventory items remain inspectable.

### Rare equipment and identification

Farming and Endgame preserve **all unidentified rare equipment**, including lower-level bases. Their actual hidden properties cannot be evaluated before identification. Kiela intentionally accepts more ground clutter to reduce the risk of missing an item that becomes valuable when identified. Some stricter approaches hide more unidentified rare bases and accept that risk; this is not a claim about every filter or a guarantee of value.

After identification, Farming requires relevant combinations for the equipment slot, rather than a universal count of property lines. Endgame requires stronger combinations and **at least 90% when the owned rare ROLL model supports reliable grading**. A property line is not an affix slot. Unsupported or modified rolls do not receive an invented percentage; conservative exceptions remain. Charms and jewels are exempt.

### Set items

- **Farming Strict: all sets remain visible.**
- **Endgame: selected higher-tier/useful set candidates.** Known lower-tier sets are hidden. Reliably supported variable rolls must reach 90%; fixed selected sets have no variable roll to grade.
- Unidentified bases shared with eligible sets remain candidates. A base known to contain only excluded sets can be hidden. Ambiguous identities and unsupported/modified roll cases retain safety exceptions; these exceptions do not make every low-tier set eligible.

### Magic equipment

Farming retains selected exceptional/elite ETH crafting bases; Endgame narrows these to elite ETH bases. Native crafting affix availability must be sufficient. Explicit strong skill/speed, socket/block, socket/life and other useful combinations remain exceptions. Unidentified magic equipment uses base/affix potential, never guessed hidden modifiers. Ordinary blue equipment is not universally preserved. All charms and jewels remain visible as collectibles and crafting material, regardless of these equipment checks.

### Runeword bases

From Farming, a base must suit Kiela's advanced-recipe selection and meet its relevant quality requirements. Advanced recipes here use a Pul-or-later rune; this is a selection boundary, not a market-value claim. Starter-only bases, including those only useful for Lore, no longer qualify. Selected low-requirement caster/buff bases remain useful exceptions, including CTA swords and HOTO flails.

Endgame additionally requires maximum relevant base bonuses and actual recipe-compatible sockets. Relevant maxima depend on the item: enhanced damage/defense, class-skill properties or Paladin automagic where applicable. This does not promise a perfect combination of every possible stat. A high item level alone does not qualify a base.

Class recommendations and required runes are green; generic compatible options are gray. The filter recognizes class, not the player's exact build. Unsocketed bases still need the stated socket count.

### Progression and consumables

Normal/Nightmare show all items. Hell/Baal use cautious equipment guidance without a universal item-level-85 cutoff and show Flawless/Perfect gems. Farming/Endgame show only Perfect gems. Gold minimums are 2,000 and 3,000 respectively. Hell hides loose ID/TP scrolls and Stamina/Thawing/Oil potions. Farming also hides ordinary HP/MP, Antidote and cold/gas/fire throwing potions; both rejuvenation sizes remain.

Stack labels appear only for quantities above one, e.g. `5x Worldstone Shard`. Item level appears as plain text at the bottom of descriptions. HR/WSS quotes retain their snapshot dates and remain per-item asking-price estimates.

### Initialization and validation

Repeated expressions are compiled through shared named formulas; RW eligibility is dispatched without repeating the full base-selection condition for every recipe. This reduces structural initialization work. First-game loading and connection behavior still require an actual game test. Automated checks cover native single-pass aliases, formula bindings, equipment transitions, protected special drops, recipes and duplicate directives. Other loot filters are not build inputs. Common game syntax is not by itself evidence of copied authorship, and comparison audits do not prove universal originality.

## Lietuviškai

Dabartinė politika: **v1.2.58**, šeši profiliai: Normal, Nightmare, Hell, Baal Runs, Farming Strict ir Endgame. [Profilių lentelė ir diegimas](./README.md#lietuviškai).

### Kas visada matoma

Visuose profiliuose, įskaitant Endgame, rodomi visi unique, kad būtų galima rinkti unique grail kolekciją. Visada lieka runos, charmai, jewels, jewel fragmentai ir saugomi PD2 specialūs daiktai: mapai, jų upgrade medžiagos ir orbai, corruption/socket įrankiai, craft medžiagos, fragmentai, boss keys, organai ir essences. Įrangos roll ribos jų neslepia. Inventoriaus daiktus galima apžiūrėti.

### Rare ir identifikavimas

Farming ir Endgame palieka **visą neidentifikuotą rare įrangą**, taip pat žemesnio lygio bazes. Tikrų paslėptų savybių prieš identifikavimą įvertinti negalime. Sąmoningai rodome daugiau daiktų, kad sumažintume vertingo rare praradimo riziką. Kai kurie griežtesni atrankos būdai slepia daugiau neidentifikuotų rare bazių ir priima šią riziką; tai nėra teiginys apie kiekvieną filtrą ar garantuota daikto vertė.

Identifikavus Farming vertina kategorijai naudingus derinius, ne universalų savybių eilučių skaičių. Endgame reikalauja stipresnių derinių ir **bent 90%, kai mūsų rare ROLL modelis leidžia patikimai įvertinti rezultatą**. Savybės eilutė nėra tas pats kaip affix vieta. Nepalaikomiems ar pakeistiems roll procento neišgalvojame; paliekamos atsargios išimtys. Charmai ir jewels nuo šių ribų apsaugoti.

### Set daiktai

- **Farming Strict rodo visus set.**
- **Endgame atrenka aukštesnio lygio/naudingus set.** Žinomi žemos vertės šablonai slepiami. Palaikomiems ir patikimai vertinamiems kintamiems roll reikia 90%; atrinkti fiksuotų savybių set neturi kintamo procento.
- Neidentifikuotos bendros bazės paliekamos, jeigu jose gali būti tinkamas set. Bazę, kuri turi tik atmestus set, galima slėpti. Neaiški tapatybė ir nepalaikomi/pakeisti roll vertinami atsargiau; tai nėra bendras leidimas visiems prastiems set.

### Magic įranga

Farming palieka atrinktas exceptional/elite ETH craft bazes, Endgame – tik elite ETH. Reikia pakankamos native crafting affix galimybės. Taip pat paliekamos aiškios stiprių skill/speed, socket/block, socket/life ir kitų naudingų derinių išimtys. Neidentifikuoti magic vertinami pagal bazės ir affix potencialą, ne išgalvotas paslėptas savybes. Įprasti blue nėra saugomi visi. Charmai ir jewels lieka visada, taip pat craft naudojimui.

### Runeword bazės

Nuo Farming bazė turi tikti mūsų pažangių receptų atrankai ir atitikti aktualią kokybę. Šiai atrankai pažangus receptas naudoja Pul arba vėlesnę runą; tai atrankos riba, ne rinkos kainos teiginys. Tik starter receptams, pvz., Lore, tinkamos bazės neberodomos. Paliekamos naudingos žemų reikalavimų caster/buff išimtys, įskaitant CTA kardus ir HOTO flailus.

Endgame papildomai reikia maksimalių aktualių bazės bonusų ir tikrų receptui tinkamų socketų. Aktualūs maksimumai priklauso nuo bazės: enhanced damage/defense, klasės skill ar Paladin automagic. Tai nereiškia tobulo visų galimų savybių derinio. Vien aukštas item level bazės neišsaugo.

Klasei rekomenduojami RW ir runos žali, bendri tinkami variantai pilki. Atpažįstama klasė, ne tikslus build. Bazei be socketų vis dar reikia nurodyto jų skaičiaus.

### Progresas ir vartojami daiktai

Normal/Nightmare rodo viską. Hell/Baal naudoja atsargias įrangos gaires be bendros item level 85 ribos; rodo Flawless/Perfect gemus. Farming/Endgame rodo tik Perfect gemus. Gold minimumai atitinkamai 2 000 ir 3 000. Hell slepia palaidus ID/TP scrolls ir Stamina/Thawing/Oil potionus. Farming papildomai slepia įprastus HP/MP, Antidote ir cold/gas/fire throwing potionus; abu rejuvenation dydžiai lieka.

Kiekis rodomas tik krūvelėms nuo 2 vnt., pvz., `5x Worldstone Shard`. Item level rašomas paprastu tekstu aprašymo apačioje. HR/WSS kainos lieka datuoti vieneto prašomos kainos įverčiai.

### Inicializavimas ir patikra

Pasikartojančios išraiškos naudoja bendras vardines formules; pilna RW bazės atranka nebekartojama prie kiekvieno recepto. Tai mažina inicializavimo darbą. Pirmo žaidimo krovimą ir ryšį dar reikia patikrinti žaidime. Automatinė patikra apima native vienos eigos alias, formulių nuorodas, įrangos būsenas, specialių daiktų apsaugą, receptus ir dublikatus. Kiti filtrai nėra kūrimo įvestis. Bendra žaidimo sintaksė savaime nereiškia kopijavimo, o palyginimas neįrodo absoliutaus originalumo.
