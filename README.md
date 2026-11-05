# Kiela v1.2.62

## English

Project Diablo 2 loot filter with HR/WSS market estimates, supported ROLL percentages, crafting help and class-aware runeword recommendations. Kiela uses its own selection generator; other loot filters are not build inputs.

**[Download ZIP](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)** · **[Download RAR](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** · **[Filter specification](./FILTER-SPECIFICATION.md)** · **[Changelog](./CHANGELOG.md)**

### Six strictness profiles

| Level | Profile | Ground selection |
| --- | --- | --- |
| 1 | Normal | All items. |
| 2 | Nightmare | All items. |
| 3 | Hell | Broad equipment candidates; Flawless and Perfect gems. |
| 4 | Baal Runs | Tighter equipment candidates; Flawless and Perfect gems. |
| 5 | Farming Strict | Useful equipment and strong magic exceptions, not craft-only blue bases; **all sets and completed crafts**; advanced RW bases; **Perfect gems only**; gold 2,000+. |
| 6 | Endgame | **Narrow top magic exceptions; all uniques for grail collecting and all completed crafts**; useful identified rares and selected sets with **90%+ supported rolls**; perfect relevant RW base bonuses and matching sockets; Perfect gems; gold 3,000+. |

**Every profile preserves all uniques, completed crafted items, runes, charms, jewels and protected PD2 special drops**: maps, map-upgrade materials/orbs, crafting materials, fragments, essences, boss keys and socket/corruption tools.

**Farming and Endgame retain all unidentified rare equipment.** Hidden affixes cannot be graded before identification. This deliberately broader visibility reduces the risk of missing a valuable rare. Some stricter selection approaches hide more unidentified rare bases, which can also exclude items that would prove useful after identification. No filter can guarantee every item's value.

Farming retains all set items. Endgame selects higher-tier/useful set candidates and applies 90% where a supported variable roll can be evaluated reliably. Ambiguous unidentified shared bases and unsupported/modified roll cases remain conservative; fixed selected sets have no variable percentage to grade.

The same short English summaries appear when changing strictness in game. Profile names omit Kiela/version. The Horadric Cube description shows the version, selected profile and visibility reminder.

### Magic equipment and runeword bases

Normal/Nightmare show all magic equipment. Hell/Baal retain cautious useful candidates, including crafting bases. From Farming, crafting potential alone no longer keeps a blue base: only useful equipment combinations/potential remain. Endgame keeps a narrower set of strong skill/speed, socket/block/life, stacked-skill and elite ETH combat candidates. Weaker ordinary magic gear is hidden; magic rings and most non-candidate bases are excluded. Unidentified candidates use focused base/affix potential, not guessed hidden stats. All charms, jewels and protected PD2 maps/materials remain. Completed orange crafted items stay visible at every profile.

Farming RW selection requires advanced-recipe suitability and good relevant base properties. Starter-only candidates, including Lore-only bases, are hidden. Useful low-requirement CTA swords/HOTO flails remain exceptions. Endgame requires maximum relevant bonuses plus actual matching sockets. High item level alone does not qualify a base. Green recommendations are class-appropriate; gray choices are generic compatible options, not detection of the player's exact build.

### Five-day prices

Charm/skiller, magic-jewel, supported RW-base, plain-map/material and rare/crafted comparable estimates now use a **five-day (120-hour) listing/bump window** and are excluded if over five days old when the filter is rebuilt. Exact-stat prices take priority over explicitly approximate same-mod groups. The sample is bounded; missing quotes do not mean no listings exist. NPC gold is separate. Older baseline unique/set estimates retain their original date, rather than pretending they were refreshed.

### Ownership and practical RW targets

`[owned]` follows PD2's native collection ownership state for uniques/sets, not merely discovery history. Unidentified items are marked only when all possible candidate groups are owned. It is not a find counter or an independent scan of every stash; if the last copy is sold, the marker clears when PD2 reports it no longer owned; another retained copy keeps it. Immediate versus rejoin timing still needs in-game verification.

RW ground labels show short practical targets, up to three names plus a remaining count. Great Poleaxe uses mercenary targets such as 4-socket Insight/Infinity/Pride and 5-socket Obedience/Doomsayer, rather than CTA. CTA targets low-requirement Crystal Swords/Flails; HOTO targets Flails/staves. The exact socket count is mandatory. Maximum capacity is not the result of a socket method. Superior bases no longer advertise the normal-only random socket Cube recipe.

All market labels say **Estimated price**. Known baseline items from 1 HR receive priority variant comparisons; if the exact clean/skill/primary-roll/socket case lacks enough evidence, an unverified-variant message replaces the headline price and the dated broad reference is labeled separately. Generic unique/set snapshots are item-wide: they are not exact-roll/socket/corruption valuations. Rare/crafted comparable intervals match core modifiers and roll bands where enough independent listings exist; broad matches explicitly say other stats can change value greatly. No quote is invented to fill a gap.

### Features and limits

- HR/WSS prices are dated asking-price snapshots, not live game queries or guaranteed sale values. NPC gold prices are separate. The baseline price date remains 2026-10-29.
- Supported ROLL percentages describe tracked variable stats, not universal build value. Unsupported/modified cases may show CHECK.
- Identified equipment/charm/jewel labels expose compact actual bonuses such as `BarbSk1`, `DruSumm1` and `PoisDmg4%`. Plain `Item class: Hammer (Mace family)` and other exact item types clarify recipe categories; `Item level: N` appears at the bottom of descriptions.
- Only stacks of two or more receive a count: `2x Key`, `5x Worldstone Shard`. Single items have no 1x marker.
- Class-appropriate Possible RW names and recipe help are green; compatible generic choices are gray. Recommendations recognize class, not the exact build. Unsocketed bases still need the required sockets.
- From Farming, RW bases must suit advanced recipes. Starter-only bases are hidden. Useful low-requirement CTA/HOTO caster/buff bases retain explicit exceptions. Endgame requires perfect relevant bonuses and actual compatible sockets.
- From Hell, hide Stamina/Thawing/Oil potions and loose Identify/Town Portal scrolls. Farming also hides ordinary healing/mana, Antidote, cold/gas/fire throwing potions. Rejuvenation keeps purple 35% and FULL labels.
- Perfect gems retain Caster/Blood and other crafting recipes; charms retain reroll guidance. Socket methods and clear-sockets help remain.

### Installation (English)

1. Extract the archive. Only **Kiela.filter** is needed by the game.
2. Copy it to your actual `ProjectD2\filters\local` folder, for example `C:\Diablo II\ProjectD2\filters\local\Kiela.filter`.
3. In the PD2 launcher choose **Item Filter Profiles → Local Filter → Kiela.filter → Save**, then launch the game with the loot filter enabled.
4. Check **v1.2.62** in the Horadric Cube description. Configure **Increase Filter Level**, **Decrease Filter Level** and optionally **Reload Loot Filter** under **Esc → Options → Configure Controls**. Suggested keys: Num Pad + and Num Pad -. The filter does not bind keys automatically.

For v1.2.58, fully close and restart PD2 to test the first-game initialization change. Shared expressions and compact RW dispatch reduce initialization work; this is not a measured loading-time guarantee or confirmation that connection interruptions are fixed.

## Lietuviškai

Project Diablo 2 filtras su HR/WSS kainų įverčiais, palaikomais ROLL procentais, craft pagalba ir klasei pritaikytomis runeword rekomendacijomis. Atranką generuojame savo generatoriumi, nenaudodami kitų filtrų kaip kūrimo įvesties.

**[Atsisiųsti ZIP](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)** · **[Atsisiųsti RAR](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** · **[Filtro specifikacija](./FILTER-SPECIFICATION.md#lietuviškai)** · **[Pakeitimai](./CHANGELOG.md#lietuviškai)**

### Šeši strictness lygiai

| Lygis | Profilis | Kas rodoma ant žemės |
| --- | --- | --- |
| 1 | Normal | Visi daiktai. |
| 2 | Nightmare | Visi daiktai. |
| 3 | Hell | Platesnė įrangos atranka; Flawless ir Perfect gemai. |
| 4 | Baal Runs | Griežtesnė įrangos atranka; Flawless ir Perfect gemai. |
| 5 | Farming Strict | Naudinga įranga ir stiprių magic derinių išimtys, ne mėlynos bazės vien craftinimui; **visi set ir pagaminti craft**; pažangių RW bazės; **tik Perfect gemai**; gold nuo 2 000. |
| 6 | Endgame | **Siauros stipriausių magic išimtys; visi unique grail kolekcijai ir pagaminti craft**; naudingi identifikuoti rare ir atrinkti set su **90%+ palaikomu roll**; maksimalūs aktualūs RW bazės bonusai ir tinkami socketai; Perfect gemai; gold nuo 3 000. |

**Visuose lygiuose lieka visi unique, runos, charmai, jewels ir saugomi PD2 specialūs daiktai**: mapai, jų upgrade medžiagos/orbai, craft medžiagos, fragmentai, essences, boss keys bei socket/corruption įrankiai.

**Farming ir Endgame palieka visą neidentifikuotą rare įrangą.** Paslėptų savybių prieš identifikavimą įvertinti negalime. Sąmoningai didesnis matomumas mažina gero rare praradimo riziką. Kai kurie griežtesni atrankos būdai slepia daugiau neidentifikuotų rare bazių, todėl gali paslėpti ir po identifikavimo naudingą daiktą. Joks filtras negali garantuoti kiekvieno daikto vertės.

Farming rodo visus set. Endgame atrenka aukštesnio lygio/naudingus set ir taiko 90% ribą, kai jų kintamas roll palaikomas ir patikimai įvertinamas. Neaiškios bendros neidentifikuotų set bazės bei nepalaikomi/pakeisti roll vertinami atsargiau. Atrinkti fiksuotų savybių set neturi kintamo procento.

Keičiant strictness žaidime rodoma trumpa angliška santrauka be Kiela ir versijos pavadinime. Versija, profilis ir matomumo priminimas pateikiami Horadric Cube aprašyme.

Kainos yra datuoti pardavėjų prašomų kainų įverčiai, ne gyvos užklausos ar garantuota pardavimo vertė. Bazinių kainų data lieka 2026-10-29. ROLL vertina palaikomas kintamas savybes, ne universalų tinkamumą veikėjui. Daikto lygis rašomas aprašymo apačioje; kiekis žymimas tik krūvelėms nuo 2 vnt., pvz., `5x Worldstone Shard`.

Baltos/pilkos ETH RW bazės atrenkamos atskirai: nuo Farming paliekamos pažangių RW bazės su CTA/HOTO caster/buff išimtimis; Endgame reikalauja maksimalių aktualių bonusų ir tikrų tinkamų socketų. Starter-only bazės slepiamos. Klasei tinkami RW ir receptai žali; bendros galimybės pilkos. Išsaugota craft, gemų, charmų ir socketų pagalba.

Nuo Hell slepiami Stamina/Thawing/Oil potionai ir palaidi ID/TP scrolls. Farming papildomai slepia įprastus HP/MP, Antidote ir cold/gas/fire throwing potionus. Rejuvenation lieka violetiniai 35% ir FULL.

### Turimi daiktai ir praktiškos RW rekomendacijos

`[owned]` remiasi PD2 unique/set kolekcijos turimo daikto būsena, ne vien atradimo istorija. Neidentifikuotam daiktui žyma rodoma tik kai turimos visos galimos kandidatų grupės. Tai nėra radimų skaitiklis ar savarankiškas visų stash tikrinimas; pardavus paskutinę kopiją žyma dingsta, kai PD2 praneša, kad daikto nebeturi; likus kitai kopijai žyma lieka. Ar būsena atsinaujina iškart, ar po prisijungimo iš naujo, dar reikia patikrinti žaidime.

Trumpas RW sąrašas ant žemės rodo iki trijų praktiškų variantų ir likusių kiekį. Great Poleaxe siejama su merc taikiniais, pvz., 4 socketų Insight/Infinity/Pride ir 5 socketų Obedience/Doomsayer, ne CTA. CTA rekomenduojama žemų reikalavimų Crystal Sword/Flail; HOTO – Flail/staff. Socketų skaičius turi tiksliai sutapti. Maksimali talpa nėra socketinimo rezultatas. Superior bazėms neberodomas tik normal kokybei tinkamas random socket Cube receptas.

Visos rinkos kainų žymos vadinamos **Estimated price**. Žinomiems baziniams daiktams nuo 1 HR prioritetas teikiamas variantų palyginimams; jei konkretaus clean/skill/pagrindinio roll/socket atvejui duomenų trūksta, pagrindinę kainą pakeičia nepatvirtinto varianto žinutė, o datuotas bendras įvertis pažymimas atskirai. Bendri unique/set įverčiai nevertina konkrečių roll/socket/corruption. Rare/crafted intervalai remiasi pagrindiniais modais ir jų ribomis, kai pakanka nepriklausomų skelbimų; platesni palyginimai pažymėti kaip labai priklausomi nuo kitų savybių. Trūkstamos kainos neišgalvojamos.

### Penkių parų kainos

Charmų/skillerių, magic jewels, palaikomų RW bazių, paprastų mapų/medžiagų ir panašių rare/crafted daiktų įverčiai naudoja **5 parų (120 val.) paskelbimo/atnaujinimo langą** ir kuriant/atnaujinant filtrą atmetami, jei senesni nei 5 paros. Tikslūs stat įverčiai turi pirmenybę prieš aiškiai apytiksles tų pačių modų grupes. Imtis ribota; kainos nebuvimas nereiškia, kad nėra skelbimų. NPC gold yra atskira kaina. Senesnių bazinių unique/set įverčių datos išlaikomos.

### Magic įranga ir runeword bazės

Normal/Nightmare rodo visą magic įrangą. Hell/Baal palieka atsargiai atrinktus kandidatus, taip pat craft bazes. Nuo Farming vien craft potencialo mėlynai bazei nepakanka: lieka tik naudingos įrangos deriniai/potencialas. Endgame palieka siauresnes stiprių skill/speed, socket/block/life, sudėtų skill bonusų bei elite ETH kovinių kandidatų išimtis. Silpnesni magic slepiami; magic žiedai ir dauguma netinkamų bazių atmetami. Neidentifikuotų daiktų atranka remiasi siauresniu bazės/affix potencialu, ne atspėtais paslėptais modais. Charmai, jewels bei saugomi PD2 mapai/medžiagos lieka. Jau pagaminti oranžiniai crafted daiktai matomi visuose profiliuose.

Farming RW atranka reikalauja tinkamumo pažangiems receptams ir gerų aktualių bazės savybių. Tik starter receptams, pvz., Lore, tinkamos bazės slepiamos. Naudingos žemų reikalavimų CTA kardų/HOTO flailų išimtys lieka. Endgame reikia maksimalių aktualių bonusų ir tikrų tinkamų socketų. Vien aukšto item level nepakanka. Žalios rekomendacijos skirtos klasei, pilki variantai – bendros tinkamos galimybės; tikslus build neatpažįstamas.

### Diegimas (lietuviškai)

1. Išarchyvuok paketą. Žaidimui reikia tik **Kiela.filter**.
2. Įkelk į savo `ProjectD2\filters\local`, pvz., `C:\Diablo II\ProjectD2\filters\local\Kiela.filter`.
3. PD2 launcheryje pasirink **Item Filter Profiles → Local Filter → Kiela.filter → Save**. Paleisk žaidimą ir įjunk loot filtrą.
4. Horadric Cube aprašyme patikrink **v1.2.62**. Mygtukus **Increase Filter Level**, **Decrease Filter Level** ir **Reload Loot Filter** priskirk per **Esc → Options → Configure Controls**. Siūlome Num Pad + ir Num Pad -; filtras mygtukų pats nepriskiria.

Bandydamas v1.2.58 pirmo žaidimo užkrovimą, visiškai uždaryk ir iš naujo paleisk PD2. Sumažintas inicializavimo darbas dar nėra išmatuotas žaidimo krovimo laikas ar patvirtintas ryšio nutrūkimo pataisymas.

## Authorship and use

Copyright (c) 2026 Melinda Kiela, original Kiela contributions only.
Kiela builds on the third-party work acknowledged in
**[THIRD-PARTY-NOTICES.md](./THIRD-PARTY-NOTICES.md)**.

The current selection rules are generated by Kiela. Earlier versions used a
third-party base; that history is recorded in the notices.

The public filter repository does not include a Kiela-specific license or
additional Kiela usage restrictions. Upstream MIT rights remain unchanged;
the standalone filter embeds the MIT notice.

This repository contains the prepared filter and release documents. The generator
and readable authoring sources are maintained separately.


White/gray bases at Farming/Endgame must pass the RW-base selection even with skill bonuses or only one socket.

Baltos/pilkos bazės Farming/Endgame lygiuose turi atitikti RW atranką net turėdamos skill bonusų ar tik vieną socketą.
