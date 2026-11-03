# Kiela v1.2.54

Project Diablo 2 loot filter built around **market-price estimates and item roll percentages**, with clear item labels, graded symbol accents and automatic player-class runeword recommendations.

**[Download Kiela.rar](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** · **[Download Kiela.zip](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)**

**[English installation instructions](#installation-english)** · **[Lietuviška instrukcija](#diegimas-lietuviškai)**

Official project: https://github.com/Melly87s/Kiela

**Only one game file is required: `Kiela.filter`.** Copy only that file into PD2. README files explain installation; license notices and release metadata are documentation, not additional filters.

## What Kiela does

From v1.2.46, Kiela uses its own selection engine without another filter as a build input. Our HR/WSS prices, roll ratings, labels and crafting help remain. Read [the rewrite and feature-preservation notes](./ORIGINALITY.md).

## Market prices and roll percentages — the heart of Kiela

Kiela is built around two core features: **in-game market-price estimates and item roll percentages**. Inspect supported items to see their estimated trade value in **HR / WSS** and how strong their tracked stat rolls are. This helps you decide what to keep, trade, upgrade or leave behind.

Market estimates come from collected listings on the live PD2 trade market and are included in filter updates. **The filter does not fetch live prices while you play.** Prices are dated snapshots of asking prices, not guaranteed sale values. For supported charms, skillers and class-specific Torches, approximate modifier-based prices can be shown even when the collected data has no exact-roll match.

## Set your own strictness hotkeys

Assign these keys yourself in **Esc → Options → Configure Controls**:

- **Increase Filter Level → Num Pad +**: increases strictness and hides more ordinary loot.
- **Decrease Filter Level → Num Pad -**: lowers strictness and shows more loot.
- Optionally assign **Reload Loot Filter** to a free key for reloading an updated local file.

Click each command's key field, press the desired key, then select **Accept**. We recommend the numeric keypad **+** and **-**. The filter file does not assign these keys automatically.

## Clear ground labels and a distinct visual style

Kiela uses compact symbols and colored labels to make different kinds of drops easier to recognize. It retains the underlying item-quality color system while adding accents for selected high-value categories.

- Small, Large and Grand Charms use the same familiar symbol with bright cyan size tags: **☯ [SC]**, **☯ [LC]** and **☯ [GC]**.
- Unique charms retain their recognizable item names alongside their size marker.
- Runes have numbered ground labels, making their position in the rune progression easier to recognize. Higher rune groups have stronger visual accents.
- Gem names follow their gem type's color. Different gem grades use compact symbols, with Perfect gems receiving their own distinctive marker.
- Healing potions use red recovery labels such as **+320**. Mana potions use blue labels such as **+250**. These are the recovery-point values in the installed PD2 data, not a promise of the exact amount every class will recover.
- Antidote potions use the short green label **anti**.
- Selected item groups use minimap markers and drop notifications. Selected valuable categories have drop sounds, applied to newly dropped items rather than ordinary inventory movement.

The result is a recognizable presentation with less ground-label clutter and useful information available when you inspect an item.

## Skill-item protection

Normal through Baal retain the cautious +2 skill safety rules. From Farming Strict, identified magic equipment and jewelry need at least two useful properties, and identified rare equipment/jewelry need 3 / 4 / 4 / 5 / 6 / 6 / 6 useful properties at levels 5–11. These are useful stat categories, not a claim to count hidden affix slots. Different skill fields count once; useful individual resistances count separately. Low dexterity and other weak incidental bonuses do not qualify.

From Endgame (level 7), ordinary magic weapons, armor and quivers are hidden even with skill bonuses, whether identified or not. Magic charms, jewels, rings and amulets follow their separate useful-property rules. Unidentified rare candidates retain existing safety checks because their true modifiers cannot yet be evaluated. Inventory items remain inspectable. White/gray runeword bases follow their separate progressive requirements.

## Current strictness and menu legend (v1.2.54)

Each in-game profile now spells out **Unique, Rare, Set and Runeword bazes** in full. The Lithuanian labels mean: **visi/visos = all**, **atrinkti = selected**, **naudingos = useful**, **geros/geresnes = good/better**, **perf su socketais = perfect with actual sockets**. Normal and Nightmare show all items. Unique items remain visible at every profile. Levels 1–8 retain sets; levels 9/10/11 use higher-level/endgame or market-supported set candidates with supported scalar rolls of at least 90% in all three profiles. Fixed eligible templates remain eligible. Unidentified shared-base candidates and modified/unsupported roll cases retain their safety exceptions. A known identified set roll below 90% is hidden even if the item has a skill bonus. Fixed eligible templates have no variable roll to grade.

From Farming, identified magic/rare jewelry needs useful skill, FCR, leech, resistance, life/mana or other supported strong properties. Unidentified jewelry remains a candidate, not a guaranteed valuable item. The final profiles retain selected charm/jewel/jewelry exceptions and rares meeting the useful-property count together with runes, uniques, selected sets, Perfect gems and PD2 maps/materials/orbs/essences/keys. Ordinary chest keys and gas/fire throwing potions are filtered at the documented later levels.

The v1.2.48 alias ordering bug has been corrected: the build now validates actual BH single-pass expansion before release. This fixes hide rules that could previously leave potions, scrolls, small gold piles and weak bases visible.

## Early progression

- **Normal and Nightmare:** show all items, including low-level equipment and small gold piles.
- **Hell:** a broad selection; ordinary magic/rare equipment uses ilvl 35/20 as initial guidance, with useful-stat and potential-affix exceptions. Show Flawless and Perfect gems.
- **Baal Runs:** somewhat tighter; ordinary magic/rare equipment uses ilvl 55/35 as guidance, with the same safety exceptions. There is no hard ilvl-85 requirement. Show Flawless and Perfect gems.
- **Farming and all higher profiles:** show Perfect gems; all runes and uniques remain visible at every profile.
- From **Hell onward**, hide Stamina, Thawing and Oil potions, plus loose Identify and Town Portal scrolls. Tomes and rejuvenation potions remain visible.
- Rejuvenation ground and inventory labels are purple **35%** and **☺FULL☺**.

Known +2 skill items, quest items and protected item categories override early hiding. Unidentified bases that can roll +2 skills or selected strong modifiers at their native affix level also override the early level guidance. Item level is not character level.

## Eleven strictness levels

Kiela provides a progression of filter levels:

1. Campaign — Normal
2. Campaign — Nightmare
3. Campaign — Hell
4. Baal Runs
5. Farming — Strict
6. Farming — Stricter
7. Endgame
8. Endgame — Stricter
9. Endgame — Strict
10. Endgame — Fast Mapping
11. Endgame — Minimal

Lower levels provide a broader selection for progression. Higher levels hide more ordinary drops and apply stricter requirements to protected runeword bases.

**From Farming, level 5 onward, only Perfect gems are shown on the ground.** Lower-grade gems are hidden at these levels. Gems already in your inventory can still be inspected normally.

For curated combat and armor bases, the middle levels use progressive quality requirements. Levels 5–6 use a 5% ED threshold; levels 7–8 use 10%. Paladin shield resistance thresholds also become stricter.

**RW base requirements now rise at every level from Farming:** ED/defense thresholds are 5/8/10/12/15/18/20 across levels 5–11, with increasing class-skill and Paladin-shield requirements. Level 11 additionally requires actual sockets matching a runeword recipe. The final relevant maxima are 20% enhanced damage/defense, 30 Paladin shield resistance (or the supported physical automagic maximum), and +3 staffmods; displayed lower staffmods and partial ED/defense bonuses do not qualify as perfect. Best-tier two-socket quivers have their own base exception.

These are rules for the stats that matter to that type of base. A maximum selected stat does not mean every possible skill combination, durability value and property on the item is perfect.

Useful low-requirement caster bases, such as compatible Crystal Swords, Broad Swords, Long Swords, Flails and Monarchs, have exceptions at lower and middle strictness levels. Those exceptions no longer bypass the progressive base requirements from Farming. The final profile requires perfect relevant bonuses and actual recipe-compatible sockets.

## Runeword bases selected for usefulness

Kiela distinguishes between an item that can technically accept a runeword and a base worth keeping at your selected strictness.

Higher strictness levels use a curated selection of weapon, armor, shield and class-specific bases instead of treating every socketable elite item as desirable. Niche bases can be hidden even when a runeword is technically possible in them.

Ground labels can identify a kept item as a **Runeword base**. Suitable bases can instead show a compact **Possible RW:** label with recommendations for your current character class.

The base-selection rules account for relevant properties such as enhanced damage, enhanced defense, Paladin shield resistance, useful skill bonuses, socket count and socket capacity. Ethereal status is used in selected base-selection rules; the filter does not treat every ethereal item as an automatic upgrade.

## Automatic class-aware runeword recommendations

Kiela uses PD2's native character-class checks to choose recommendations for Amazon, Assassin, Barbarian, Druid, Necromancer, Paladin and Sorceress characters.

When you change character class, the relevant recommendations change automatically. There is no need to install a separate filter for each class.

- Recommended runewords are highlighted in **green** in a base's tooltip.
- Other compatible options use **dark gray** text.
- Recommended entries on unsocketed bases include the required runes in insertion order.
- Required socket counts are shown with the runeword lists.
- Socketed bases show recipes appropriate to their exact socket count.
- Unsocketed bases show possible options within the base's socket capacity.

Class recognition is automatic; build recognition is not. Druid recommendations are tuned toward Summon, while the other classes use general shortlists. Weapon type and class restrictions still apply.

The tooltip has a fixed length limit in PD2. If an unsocketed base has too many possible options, Kiela preserves the recommended recipes and may summarize omitted ordinary entries as **+N other RW**.

## Socketing instructions on equipment

Kiela adds socket information to relevant equipment, including the base's capacity and the limits of available methods.

Depending on the item and its quality, the tooltip can show:

- Maximum socket capacity.
- Larzuk quest socket count or range.
- Larzuk's Puzzlepiece or Puzzlebox socket range.
- Larzuk's Malus socket information.
- The possible socket cap from a Worldstone Shard corruption.
- A Horadric Cube socket recipe where applicable.
- A warning that an already socketed item cannot receive additional sockets through those methods.
- The Hel rune + Town Portal Scroll recipe for clearing socket contents.

Cube instructions state both the ingredients and the result. For example, a suitable Flail can show **Cube: adds 1–5 random sockets**, followed by **Recipe: item + Ral + Amn + Perfect Amethyst**.

A random socket recipe does not guarantee the count needed for a particular runeword. Corruption is also a risk, not a guaranteed socket upgrade. Clearing sockets destroys their contents and does not change the number of sockets.

## Stat-roll ratings

Kiela provides roll information for supported magic and rare items, charms, unique and set items, and runewords.

- **Roll %** summarizes the tracked variable properties against their modeled maxima.
- **GOOD** and **TOP** labels distinguish stronger tracked rolls.
- **BAD ROLL** identifies a lower result in that model.
- **FIXED** means there are no variable rolls in the supported model.
- **Tracked roll** means some base-dependent properties have been excluded because they cannot be reliably separated from the runeword's own contribution.
- **Roll: CHECK** means the filter cannot confidently provide a supported percentage for that item in its current state.

The rating is not a universal build score. A lower overall percentage can still include a valuable stat, and a high percentage does not automatically make an unwanted item valuable.

Runeword models include the fixed effects of inserted runes. Relevant base contributions are handled separately, including base block on shields. Modified items and unsupported combinations may require manual checking.

## Charm combinations and skillers

Kiela recognizes useful charm combinations and can highlight combinations such as life + mana or life + resistance.

Charm tooltips also provide roll information and the magic-charm reroll recipe:

**Magic charm + any 3 Perfect gems in the Horadric Cube.**

This works for magic Small, Large and Grand Charms. It replaces the existing magic properties. It is not a recipe for rerolling unique charms.

The price data includes plain skillers across all 21 skill trees, selected exact-stat charm combinations, skillers with STR or DEX, broader modifier-set estimates, and class-specific Torch estimates where enough supported listings are available.

## NPC prices and market-price estimates

Kiela keeps vendor value and trade-market estimates separate:

- **Price: ... gold** is the NPC sell-price field on supported equipment.
- **Global price: ... HR / WSS** is a market estimate from collected trade listings.

For charms, an available exact-roll price match takes priority. If no exact-roll match is available but a supported modifier group has enough data, Kiela can show an approximate price for that group, pooling different rolls.

Examples include FHR + resistance Small Charms, life + mana Large Charms, STR/DEX skillers, and Torches grouped by character class and modifier set.

Approximate entries explicitly say **No exact-roll match in price data** and **Approx. / all rolls**. This refers to the filter's collected dataset; it does not claim that no matching item exists anywhere on the live market.

Grouped charm estimates require at least three supported listings from at least two sellers. Prices are asking-price medians, not confirmed sale prices. The current data is for **softcore ladder**. It is not a live in-game market connection or a hardcore price list.

When there is insufficient supported data, the filter reports limited market information rather than inventing a price. Roll quality, demand, season timing, corruption and unusual combinations can all change what an item actually sells for.

## Crafting and cube help

**Perfect gems** list their crafting family, supported equipment slots and required runes. The families include Caster, Blood, Hitpower, Safety, Bountiful, Brilliant and Vampiric.

The tooltip explains the general recipe and gives slot-specific rune information for amulets, rings, belts, gloves, boots, helms, armor, shields and weapons.

Lower-grade gems show their upgrade recipe instead of a list of crafts they cannot yet perform. Rune tooltips retain useful crafting and rune-upgrade information without displaying a long list of every runeword containing that rune.

Map tooltips can show baseline monster resistance ranges. These are reference
values, not live measurements of every monster after all map modifiers.

Additional tooltips provide relevant help for map-crafting materials, Worldstone Shards, socket clearing, item-base upgrades and other supported cube uses. These instructions apply to eligible items; an ingredient alone does not guarantee a recipe is valid for every target.

## Version and update information

The Horadric Cube tooltip displays the loaded Kiela version, selected profile, filter build time in Lithuania and the baseline price-data date.

**Filter updated** and **Prices** are separate dates. Editing the filter updates the release timestamp; it does not falsely refresh every market-price record. Individual charm estimates include their own snapshot date.


## Installation (English)

1. **[Download Kiela.rar](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** and extract it with WinRAR or 7-Zip.
   Alternatively, **[download Kiela.zip](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)** and use Windows **Extract All**.
   The archive contains `Kiela.filter`, instructions and licenses. Copy only **Kiela.filter** into the game folder.
2. Find your **Project Diablo 2** installation and put the file in
   **`ProjectD2\filters\local`**. For example:

   ```text
   C:\Diablo II\ProjectD2\filters\local\Kiela.filter
   ```

   Your drive and main installation folder may differ. Create `filters\local`
   inside your actual `ProjectD2` folder if necessary. Do not use the Downloads
   folder or a Diablo II Resurrected installation.
3. Open the PD2 launcher → **Item Filter Profiles** → **Local Filter** →
   **Kiela.filter** → **Save Filter / Save**, then start the game.
4. Make sure the in-game loot filter is enabled. Change its strictness level and
   look for **Kiela v1.2.54** in the displayed profile name. Start with a
   lower level; higher strictness intentionally hides more items and weaker bases.
5. Bind strictness in game: **Esc → Options → Configure Controls**. Scroll down
   to **Increase Filter Level** and **Decrease Filter Level**. Click the first
   key field beside each command, then press **Num Pad +** / **Num Pad -**,
   or unused **F8** / **F7**. Click **Accept** and test them in game.
   Increasing the level hides more items; decreasing shows more.
   Numpad keys are separate from the main keyboard + / - keys.
   Optional commands: **Reload Loot Filter** and **Restore Previous Level**.
   The filter does not bind keys automatically.

Only the `.filter` file is needed to play. No generator, Node.js, activation key,
custom loader or font installation is required. This is for **Project Diablo 2**,
not Diablo II Resurrected. Online launcher-catalog registration is a separate step.

To update, close the game, download the same file again, replace your local copy
and restart. A manually installed local filter does not update itself from GitHub.
If it is missing from the launcher, check the path, filename extension and Local
Filter selection, then reopen the launcher. If items are hidden, lower strictness.

## Diegimas lietuviškai

### 1. Atsisiųsk ir išarchyvuok

Spausk **[Atsisiųsti Kiela.rar](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)**.
Išarchyvuok su WinRAR arba 7-Zip. Arba atsisiųsk **[Kiela.zip](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)**
ir Windows meniu pasirink **Extract All / Išskleisti viską**.

Archyve yra `Kiela.filter`, ši instrukcija ir licencijos. Į žaidimo aplanką
kopijuok tik **Kiela.filter**. Paties `.rar` ar `.zip` į `local` dėti nereikia.

Failo pavadinimas turi būti tiksliai:

```text
Kiela.filter
```

Jis neturi baigtis `.txt` ar `.html`. Windows File Explorer meniu įjunk
**View / Rodymas → Show / Rodyti → File name extensions / Failų vardų plėtiniai**,
kad matytum tikrąjį pavadinimą. Jei gavosi `Kiela.filter.txt`, pašalink tik
galinį `.txt`.

Taip pat gali atsidaryti [filtro failą GitHub](https://github.com/Melly87s/Kiela/blob/main/Kiela.filter)
ir spausti **Download raw file**. Visos GitHub svetainės puslapio kaip HTML saugoti nereikia.

### 2. Įdėk failą į savo PD2 aplanką

Surask aplanką, kuriame įdiegtas **Project Diablo 2**. Jame atidaryk:

```text
ProjectD2\filters\local
```

Pavyzdžiui, jei Diablo II įdiegtas `C:\Diablo II`, galutinis failo kelias bus:

```text
C:\Diablo II\ProjectD2\filters\local\Kiela.filter
```

Tavo diskas ir pagrindinio aplanko pavadinimas gali skirtis. Svarbu naudoti savo
**ProjectD2** įdiegimo aplanką, o ne Downloads, Documents ar Diablo II Resurrected
aplanką. Jeigu `filters` arba `local` aplanko nėra, sukurk juos būtent po `ProjectD2`.

Jei nežinai, kur įdiegtas PD2, ant jo launcherio nuorodos spausk dešinį pelės
mygtuką → **Open file location / Atidaryti failo vietą**. Jei atsidaro dar vienas
nuorodų aplankas, atidaryk tikrojo launcherio failo vietą.

### 3. Pasirink filtrą PD2 launcheryje

1. Atidaryk įprastą **Project Diablo 2 launcherį**.
2. Spausk **Item Filter Profiles**.
3. Pasirink **Local Filter**.
4. Vietinių filtrų sąraše pasirink **Kiela.filter**.
5. Spausk **Save Filter / Save** ir paleisk žaidimą.

Tai vietinis filtras. Jo nereikia ieškoti tarp internetinių autorių profilių.
Vien GitHub repozitoriumas automatiškai neįtraukia jo į PD2 internetinių filtrų katalogą.

### 4. Patikrink žaidime

Įsitikink, kad PD2 nustatymuose įjungtas loot filtras. Pakeitus filtro griežtumo
lygį turi būti rodomas profilio pavadinimas su **Kiela v1.2.54**.

Pasirink norimą **Filter level / strictness**. Pradėk nuo žemesnio lygio ir kelk
jį pagal poreikį: aukštesnis strict slepia daugiau paprastų daiktų ir reikalauja
geresnių atrinktų runeword bazių statų. Nuo 5 lygio nišinės bazės slepiamos;
kovinėms bazėms taikomi 5 / 10 / 20 ED slenksčiai, paladino skydams –
20 / 25 / 30 res. Naudingi +3 skill bazių variantai išlaikomi. Iki 8 lygio tinkamų socketų
Crystal / Broad / Long Sword, Flail ir Monarch išimtys nereikalauja ED.
9–11 lygiuose saugomoms bazėms reikia maksimalaus svarbaus priedo.
Nuo Farming, 5 lygio, ant žemės rodomi tik Perfect gemai.
Aukščiausias lygis nėra skirtas parodyti viską.

### Griežtumo klavišai žaidime

1. Žaidime spausk **Esc → Options → Configure Controls**.
2. Nuslink iki loot filtro komandų, parodytų PD2 valdymo sąraše.
3. Prie **Increase Filter Level** spausk pirmą klavišo laukelį ir paspausk
   **Num Pad +** (arba laisvą **F8**) — didina strictness, slepia daugiau daiktų.
4. Prie **Decrease Filter Level** priskirk **Num Pad -** (arba laisvą **F7**)
   — mažina strictness, rodo daugiau daiktų.
5. Spausk **Accept**, grįžk į žaidimą ir išbandyk klavišus. Turi pasirodyti
   naujas **Filter level** su Kiela versija ir profilio pavadinimu.

**Num Pad + / -** yra skaičių klaviatūros klavišai, ne pagrindinės eilės + / -.
Jei šie klavišai jau priskirti įgūdžiams, pasirink kitus laisvus klavišus.
Pasirinktinai gali priskirti **Reload Loot Filter** filtro perkrovimui ir
**Restore Previous Level** ankstesniam griežtumui grąžinti.
Pats `.filter` failas klavišų automatiškai nepriskiria.

**Žaidimui užtenka vieno `.filter` failo. Node.js, generatoriaus, atskiro
paleidiklio, aktyvacijos rakto ar pakeistų šriftų įdiegti nereikia.**

### Atnaujinimas

Uždaryk žaidimą, iš naujo atsisiųsk filtrą iš tos pačios nuorodos ir pakeisk seną
`ProjectD2\filters\local\Kiela.filter`. Launcheryje patikrink pasirinkimą
ir vėl paleisk žaidimą. Vietinė kopija iš GitHub automatiškai neatsinaujina.

### Jei neveikia

| Kas nutiko? | Ką patikrinti? |
| --- | --- |
| Failo nėra sąraše | Jis turi būti tikrame `ProjectD2\filters\local` aplanke. Iš naujo atidaryk launcherį ir pasirink **Local Filter**. |
| Failas vadinasi `.filter.txt` | Įjunk Windows failų plėtinių rodymą ir pašalink galinį `.txt`. |
| Išsisaugojo HTML puslapis | Atsisiųsk per tiesioginę nuorodą arba GitHub **Download raw file**. |
| Vis dar rodo kitą filtrą | Dar kartą pasirink Kiela ir spausk **Save Filter**, tada iš naujo paleisk žaidimą. |
| Po atnaujinimo liko sena versija | Patikrink, ar pakeitei failą tame pačiame PD2 įdiegimo aplanke, kurio launcherį paleidi. |
| Nerodo dalies daiktų | Sumažink strict. Tai gali būti įprastas filtravimas, o ne diegimo klaida. |
| F7 / F8 nieko nedaro | Klavišus pirmiausia priskirk per **Configure Controls**. |
| Simboliai atrodo netaisyklingai | Naudok atnaujintą PD2 su jo HD atvaizdavimu. Šis paketas papildomų šriftų ar žaidimo archyvų nepakeičia. |

## What the labels mean / Ką reiškia žymos

- Original item-quality colors are retained. Better value categories receive
  stronger compact symbol accents.
- Ground charms use **☯ [SC] / ☯ [LC] / ☯ [GC]**, with bright cyan size tags.
- **Possible RW: ...** on a ground base recommends a compatible runeword for the
  current player class. Recommended runeword names are **green** in item tooltips.
  Class detection is automatic; build detection is not. Druid preferences are
  tuned for **Summon**. Add the required sockets before inserting runes.
- In the possible-runeword list, **2s / 3s / 4s / 5s / 6s** mean the required
  number of sockets. Ordinary entries are dark gray; class recommendations are green.
- Green recommendations include the runes in insertion order. On unsocketed bases,
  very long lists may end with **+N other RW** to fit PD2's tooltip limit.
  Socketed bases show matching recipes for their exact socket count.
- **Cube: adds 1-N random sockets** means cubing the unsocketed item with the
  listed runes and Perfect gem. It does not guarantee the socket count needed
  for a runeword. The recipe uses the item itself; **Perfect Amethyst** is written out.
- Socket tips show the base cap and method limits: **Larzuk** = quest,
  **Piece / Box** = Larzuk's Puzzlepiece / Puzzlebox, **Malus** = Larzuk's Malus.
  **WSS max** is a possible corruption result, not a guaranteed safe outcome.
- Only **Perfect** gem tooltips list crafting families, slots and runes.
  Lower gem grades show the upgrade recipe.
- Mod-based charm estimates pool the same modifier set across all rolls, including
  FHR + resist Small Charms, life + mana Large Charms, and class-specific Torches.
  Exact-roll matches take priority; pooled estimates say **No exact-roll match in
  price data** and **Approx. / all rolls**. This does not claim that no exact item
  exists anywhere on the live market.
- **Price** is the NPC vendor sell-price field. **Global price** is an available
  market estimate, not the amount an NPC pays and not a guaranteed sale.
- Skiller prices marked **STR / DEX, all rolls** pool the same skill tree and
  attribute mod across different attribute rolls. Exact-roll matches take priority.
- Runewords with variable stats have a **Roll %**. Fixed runewords say **FIXED**.
  **Tracked roll** excludes stats which cannot be separated from superior or
  innate base bonuses. Modified or unmatched items say **Roll: CHECK**.
- Magic Small, Large and Grand Charms can be rerolled with **the charm + any
  3 Perfect gems** in the Horadric Cube. The old stats are replaced; item level stays.
- **Roll %** rates tracked variable stats; it is not a universal build score or
  a guarantee that an item is valuable.
- Red and blue potion labels show recovery amounts, for example **+320** and **+250**.

The cube tooltip separates **Filter updated** (release build time in Lithuania)
from **Prices** (the baseline price-data date). Charm estimates show their own
market-snapshot date. A filter edit does not claim that every price was refreshed.

Market estimates in this release are a **softcore ladder snapshot**, not a live
in-game market connection or hardcore pricing. Prices can become stale, and
exact-stat charm price coverage is limited. Missing matching data is not a zero price.

## PD2 launcher catalog

The repository contains one playable filter: **Kiela.filter**. The remaining files are documentation, licenses and release metadata. Proposed launcher entry:

```json
{"name":"Kiela","url":"https://api.github.com/repos/Melly87s/Kiela/contents","author":"Melinda Kiela"}
```

The official PD2 team must approve and merge the `filters.json` pull request
before the filter appears in the launcher catalog. Until then, use **Local Filter**.
After approval: select **Melinda Kiela → Kiela.filter → Save Filter**. The online
selection lets the launcher download the latest filter when you press Play.
See the [official creator instructions](https://github.com/Project-Diablo-2/LootFilters#for-loot-filter-creators).

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

Freezing/cold throwing potions (all three sizes) remain visible through Baal Runs
and are hidden from Farming Strict (level 5) onward. Thawing potions remain
hidden from Hell as specified separately.


Identified magic/rare ground labels show their actual skill bonuses and relevant numeric stats, such as [+3 Bow skills] [+20% IAS]. Runeword ground recommendations use full names; the matching tooltip highlights class recommendations and their required rune order in green. A socketless base still needs the stated sockets before a runeword can be made. These class recommendations are broad profiles, not detection of the player’s exact skill build.


Every visible ground item now starts with a quantity: x1 for a single item and x5 for a five-item stack. The count is for that physical item/stack, not nearby drops. Ground HR/WSS quotes remain per-item estimates. Inventory labels retain their previous format.


From v1.2.54, Farming Strict gold minimum is 2000, rising by exactly 1000 at every subsequent level: profiles 5–11 use 2000/3000/4000/5000/6000/7000/8000. Earlier profiles retain their previous gold behavior. Every ground item shows an actual quantity or x1; gold shows its actual amount once.


## v1.2.54: enforce late set selection

From Endgame Strict (profile 9), lower-tier set templates no longer bypass set selection through +skill bonuses. This also applies to corrupted lower-tier items when their identity is known. Selected higher-tier/market-supported set candidates and the supported 90% roll requirement remain as before. Ambiguous shared-base or unsupported-roll candidates remain conservative; inventory and unique visibility are preserved. Levels 1–8 retain their existing set behavior.


## v1.2.54: item levels at the bottom of descriptions

Every final item description ends with plain text Item level: N. Item level is not included in ground or inventory names. This follows the user’s clarification; quantities, selection, prices, recipes and roll processing remain unchanged.
