# Melindaa Changelog / Pakeitimų istorija

[English](#english) · [Lietuviškai](#lietuviškai)

## English

Melindaa uses our own selection rules and features. This changelog records changes to strictness, prices, ROLL ratings, recipes and item labels.

Newest entries appear first. Later releases may supersede earlier selection rules. This documentation update does not change the filter version.

### v1.2.74 — Launcher metadata and clearer missing prices

- Added filter_definitions.json with a single Melindaa.filter entry; included it in future public packages and downloads.
- Items without a supported estimate now show "Estimated price: in development". Existing numeric HR/WSS estimates and their source dates are preserved.
- Prepared the launcher registration entry using the official name/url/author format and the current Melindaa repository address.

### v1.2.73 — Simplified public documentation

- Removed the separate ORIGINALITY and THIRD-PARTY-NOTICES documents from the current public package and removed their README links. Internal validation remains private.
- Required MIT copyright and permission text remains unchanged in **MIT-NOTICE.txt** and the standalone filter header. Gameplay, selection, prices and the Melindaa name remain unchanged from v1.2.72.

### v1.2.72 — Melindaa rename, focused blue drops and clear socketing methods

- Renamed the public project to **Melindaa**, including Melindaa.filter, in-game status, repository, descriptions and Melindaa ZIP/RAR archives. Local launcher settings migrate from the old filename; obsolete local copies are backed up and removed.
- Farming with Blue now hides unidentified Magic throwing knives, throwing axes and javelins unless ETH and elite. Existing potential and identified-stat checks remain; no general crafting bypass was added. Rare, Crafted, Unique, protected collectibles and earlier profiles are preserved.
- RW recommendations now respect caster/mercenary base purpose at every profile. Lower levels keep more suitable starter recipes, including Lore helms, but no caster-staff Insight or staff HOTO. Selected Fury/Wind/Obsession base roles are explicit instead of generic compatibility.
- Replaced ambiguous socket-method abbreviations with **Larzuk quest (Act 5)**, **Larzuk's Puzzlebox**, **Larzuk's Puzzlepiece** and **Cube + Larzuk's Malus**. Capacity-capped results and existing socket counts are unchanged. Added bilingual socket-method examples to the main description.

### v1.2.71 — Endgame unsocketed RW bases

- Endgame now accepts shortlisted perfect RW bases with **0 sockets**, provided capacity supports a selected practical recipe. Already-socketed bases must still match a selected recipe’s exact socket count.
- Renamed the marker to **[owned grail]** on ground and inventory names. Added a dedicated bilingual Owned Grail table explaining native ownership, unidentified ambiguity, selling-state timing and the lack of owned-roll comparison.
- Perfect relevant bonus checks, both Farming modes, gold thresholds, prices, inventory ownership labels and PD2 safeguards remain unchanged. Capacity does not guarantee the socketing result.

### v1.2.70 — Two Farming choices, cautious charm quotes and shorter crafting help

- Added level 5 **Farming with Blue** with independently authored useful Magic combinations/affix-potential candidates, and level 6 **Farming without Blue**, hiding all ordinary Magic gear/jewelry. Charms, jewels and protected PD2 items remain visible. Both Farming profiles share Rare/Set/RW selection; all completed crafts stay visible.
- Endgame is now level 7: ordinary blue gear hidden, supported identified Rare/selected Set 90%+, perfect relevant RW bonuses and matching sockets. Preserve all uniques, unidentified rares and protected collectibles. Migrate previous six-profile Endgame selections once to 7.
- From Farming, RW guidance uses concrete practical base/recipe pairs. Removed caster-staff Insight and arbitrary melee Wind/Fury recommendations; retained common caster/buff, mercenary and build-specific bases, intersected with installed game recipes. Merc candidates show **Merc RW** on the ground and **Possible merc RW** in help. Earlier profiles retain broader recipe guidance; quality/socket thresholds remain.
- Gold thresholds are 2,000 / 3,000 / 4,000 at the two Farming modes and Endgame; earlier profiles retain their thresholds.
- Pure Gold Find-only Magic charms now say **Estimated price: no reliable price for these mods**, without a numerical quote or a skiller price. Other complete-mod comparisons remain separate.
- Ground resistance tags now spell out **Fire res / Cold res / Light res / Poison res**, replacing FR/CR/LR/PR.
- Craft ingredients use **Crafting material**; Perfect-gem recipe lines use the corresponding gem color. Preserve recipes, ROLL and prices. Socket counts now say **Sockets: N/M**, without cannot add more.
- Retained the v1.2.69 inventory [owned] label, earlier poison/stat labels, pricing updates and safety protections. Native ownership does not expose owned-copy stats; automatic better-than-owned percentages are not claimed.

### v1.2.69 — Inventory ownership labels

- Unique/Set items now show **[owned]** beside their inventory name as well as on the ground, using the same conservative native ALLOWNED check. Names, ROLL and price descriptions remain intact.
- The flag reports current ownership, not an owned copy’s stats or roll. No automatic roll comparison with stored copies is implied. Existing v1.2.63–68 selection, pricing and presentation updates are retained.

### v1.2.68 — Restored Cube information and asking-price warning

- Farming Strict now hides every Magic weapon, helm, belt, boot, glove and shield, including circlets/class helms, ID or unID, regardless of bonuses. Rings, amulets, body armor and quivers retain their selected Farming candidates. Endgame also hides all Magic rings and amulets.
- Fixed charm/jewel crafting help overwriting accumulated ROLL information. Supported variable rolls remain visible alongside recipe help and prices, including the reported 4% fire-resist Small Charm (Roll 36%).

- Fixed Cube/tome descriptions replacing earlier lines. Short continuing actions now preserve accumulated information, including filter version, update time, baseline-price date and selected profile. Cube summaries are kept within the native description budget.
- Added a short Cube warning that asking prices can be unrealistic and are not guaranteed sales. The main README explains the effect of unrealistic seller prices on estimates.
- Rewrote the bilingual main description around all six strictness profiles, with exact Farming/Endgame differences and recent changes since v1.2.62.

### v1.2.67 — Poison damage ground labels

- Identified magic/rare/crafted ground labels now include added poison damage and duration. Poison rates are converted to total damage rather than displaying the raw internal stat. Fixes poison-only charms showing just their size tag.

### v1.2.66 — Silent fixed rolls and socket help colors

- Items without variable rolls no longer show FIXED. Fixed runewords remain silently recognized so they do not fall through to an unsupported-roll warning.
- Antidote potions are visible at every strictness level again.
- Socket counts, limits, Larzuk/Puzzle/WSS/Cube methods and socket-clearing help use the same light-blue TEAL as ground socket markers. RW socket-count headings and capacity reminders follow the same color; class recipe names remain green.

### v1.2.65 — Quantity labels and cube help

- Removed quantity badges from arrows, bolts and throwing weapons, including javelins, across quality and identification states. Other consumable/material stacks retain their counts.
- Split cube/tome status and profile help into short continuing actions to avoid the native BuildAction regex limit behind the reported cube-name error. In-game confirmation remains pending.

### v1.2.64 — Endgame magic equipment exclusions

- Endgame hides every magic ring, amulet, shield, weapon, belt, glove, boot and helm (including circlets and class helms), identified or unidentified, regardless of skills, sockets, ETH or other bonuses. Farming retains its previous selection. Magic chest armor/quivers retain their existing selection; charms, jewels and protected PD2 specials remain visible.

### v1.2.63 — Complete modifier-set price comparisons

- Charm and magic-jewel estimates prioritize the same complete modifier set with numeric rolls pooled. Skill tree identities remain separate; one-mod charms cannot inherit two-mod skiller prices. Added missing PD2 large-charm bonus exclusions to all charm quote paths.
- Rare/crafted comparisons retain core mods and strongest support roll bands; broad fallback quotes that omit support rolls are no longer used. Unsupported samples remain explicitly unquoted. Refreshed the bounded charm modifier-set sample.

### [v1.2.62](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.62) — Close weak RW-base skill bypass

- Farming and Endgame now apply the same curated RW-base requirements to one-socket and non-socketable white/gray equipment. A skill bonus alone cannot keep an unusable base, including the reported one-socket Burnt Wand. Earlier profiles, completed crafts, uniques and protected PD2 materials remain unaffected.
- Includes the ownership markers, practical RW guidance, compact stats, Item class descriptions and estimated-price improvements described below.

### [v1.2.61](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.61) — Owned markers, practical RW targets and clearer price estimates

- Added **[owned]** to unique/set ground names when PD2's native collection state reports every candidate variant group owned. This is current ownership, not discovery history or a find counter. Ambiguous unidentified variants are handled conservatively; ownership never hides a unique. After selling the last copy, the marker clears when PD2 reports it no longer owned; another retained copy keeps it. Immediate versus rejoin update timing still needs in-game verification.
- Reworked magic selection with independently authored signatures: Farming keeps broader useful equipment combinations/potential; Endgame keeps narrower strong skill/speed, socket/block/life, stacked-skill and elite ETH combat candidates. Craft-only blue bases stop after Baal. All completed orange crafts, charms, jewels and protected PD2 special drops remain visible.
- Replaced generic legal-recipe lists with practical base-role recommendations. Great Poleaxe targets include mercenary 4-socket Insight/Infinity/Pride and 5-socket Obedience/Doomsayer; CTA uses low-requirement Crystal Swords/Flails. Class recommendations stay green. Ground labels show up to three short RW names plus a remaining count, with fuller recipe help in descriptions.
- Clarified socket capacity versus required sockets. Removed the standard normal-only random socket Cube recipe from Superior bases. Exact recipe socket counts remain mandatory; maximum capacity is not a guaranteed socketing result.
- Added plain Item class labels for equipment and supported item families, distinguishing Hammer/Mace/Club/Scepter/Polearm/Staff.
- Shortened ground bonus text, including **max dmg 1**, **min dmg 8** and **Ltng1-5** and **GF8%**. Added compound elemental-damage decoding to charm/jewel price matching, preserving element and skill identities.
- Renamed every market display to **Estimated price**. Generic unique/set snapshots explicitly state that exact roll/socket/corruption is not matched. Dated asking-price estimates are not guaranteed sale prices.
- Added five-day rare/crafted comparable intervals, matched by base/quality/ETH/sockets and core modifiers/roll bands; broader core matches explicitly pool secondary stats. No number is invented without sufficient independent listings.
- Prioritized known baseline items at 1 HR or more for tighter five-day unique/set comparisons, matching class/tree skills, primary rolls, ETH and empty-socket count where enough evidence exists. Unsupported variants show an unverified-variant explanation and label the old broad reference separately. Corrupted/filled variants are not priced as clean items.
- Expanded RW-base samples by sockets, ETH, Normal/Superior and ED/durability bands. Added plain-map and map-material/tool samples with unambiguous per-item offers. Rolled/modified maps are not priced as plain maps.
- Preserved all unidentified rare equipment at Farming/Endgame, all uniques for grail, runes, Perfect gems, completed crafts and special-drop protection. Added native regressions for ownership, stricter magic, practical RW/socket rules, element matching and valuable-item variants. Final exact/normalized duplicate audits are part of release validation.

### [v1.2.60](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.60) — Compact drop details, five-day quotes and clear Endgame selection

- Shortened all six in-game profile summaries to at most 85 characters. Replaced vague gear wording with Magic/Rare guidance, `Perf gems`, and clear Endgame exclusions. Full details remain in the Cube and specification.
- Compact ground tags now show actual identified equipment, charm and jewel bonuses, e.g. `BarbSk1`, `DruSumm1`, `PoisDmg4%`, `IAS30%` and `STR24`. Identified charms/jewels use short base labels, with important skill/damage bonuses before secondary stats.
- Endgame hides all ordinary magic equipment, identified or not, including ETH items, rings and amulets. Charms, jewels, protected PD2 maps/materials and all completed orange crafted items remain visible at every profile. Farming retains useful magic equipment combinations/potential, but crafting potential alone no longer keeps a blue base after Baal Runs.
- White/gray ETH runeword bases remain separate: Farming uses looser advanced-base selection; Endgame requires maximum relevant bonuses and actual matching sockets. Magic equipment cannot be made into a runeword.
- Refreshed charm/skiller data using five days (120 hours) of official listing/bump activity. Added bounded magic-jewel samples and normal Monarch quotes. Quotes expire after five days; exact-stat matches precede clearly labeled approximate mod groups.
- Supported charm/jewel/base quotes now also appear on the ground without erasing bonus tags. Missing supported quotes are explained explicitly; NPC gold is separate. A missing quote does not mean no market listings exist. Other baseline prices retain their original dates.
- Preserved all unidentified rare equipment at Farming/Endgame, all uniques for grail collecting, runes, Perfect gems, completed crafts and protected PD2 drops. Added regressions for screenshot labels, five-day expiry, price matching and Endgame magic exclusion.

### [v1.2.59](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.59) — Clear magic and runeword descriptions

- Expanded the filter description and in-game profile text to explain the existing magic/RW selection. This release changes descriptions, not item visibility.
- Normal/Nightmare show all magic equipment; Hell/Baal use cautious candidate selection. Farming keeps selected exceptional/elite ETH craft bases and strong combinations such as skills + IAS, sockets + block or sockets + life. Endgame narrows ETH crafting to elite bases while retaining strong magic exceptions. All charms and jewels remain visible, including jewels for crafting.
- Farming RW bases must suit advanced recipes; starter-only bases such as Lore candidates are excluded. Useful low-requirement CTA sword/HOTO flail exceptions remain. Endgame requires maximum relevant base bonuses and actual recipe-compatible sockets; high item level alone is insufficient.
- Class-recommended runewords and recipe help are green; generic compatible options are gray. The filter recognizes class, not the exact build.
- Farming/Endgame keep all unidentified rare equipment. Identified rares use useful combinations; Endgame adds 90% where reliable grading is supported. Farming keeps all sets; Endgame selects useful sets with supported 90% grading and conservative identity/roll exceptions. All uniques remain for grail collecting; runes and protected PD2 special drops remain visible.

### [v1.2.58](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.58) — Six profiles, safer rare visibility and lighter initialization

- Simplified strictness to Normal, Nightmare, Hell, Baal Runs, Farming Strict and Endgame. Short English in-game summaries now explain set selection, Perfect gems and late RW bases without the Melindaa/version prefix.
- Farming and Endgame preserve all unidentified rare equipment to reduce the risk of losing a valuable item before identification. Some stricter approaches hide more unidentified rare bases and accept that risk; Melindaa deliberately favors greater visibility. Hidden rolls are never guessed.
- Farming evaluates identified gear by useful slot-specific combinations. Endgame requires stronger combinations and 90%+ for identified rare/set rolls where reliable grading is supported. Unsupported/modified cases retain conservative exceptions.
- Farming shows all sets. Endgame selects higher-tier/useful sets, preserves ambiguous shared-base candidates and requires 90% where applicable. All uniques remain visible even in Endgame for unique grail collecting.
- All charms, jewels, jewel fragments, runes, maps, PD2 orbs, crafting/map-upgrade materials, essences and protected special drops remain visible at every profile.
- Farming retains selected exceptional/elite ETH craft candidates and valuable skill/socket magic exceptions; Endgame narrows ETH crafting to elite candidates. Anti potions are hidden from Farming. Gold minimums are 2,000 at Farming and 3,000 at Endgame; both show only Perfect gems.
- Farming RW bases must suit advanced recipes, with useful caster/buff exceptions such as CTA/HOTO. Endgame requires perfect relevant bonuses and matching actual sockets. Starter-only bases and late Lore recommendations are excluded.
- Reduced first-load rule expansion and repeated expression compilation using shared formulas and compact runeword dispatch. This reduces initialization work; actual loading time and connection interruptions still require an in-game test after fully restarting PD2.
- Preserved dated HR/WSS data, the owned ROLL engine, crafting/socket help, ground bonus labels, stack-only counts and item level at the bottom of descriptions. Added a bilingual filter specification.

### [v1.2.57](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.57) — Category-based strictness

- Replaced universal modifier counts with Melindaa combinations for eleven categories: gloves, boots, belts, circlets, helmets, shields, body armor, weapons, quivers, rings and amulets.
- Identified items are assessed by relevant core/support combinations. Strong items with fewer properties can survive, while many weak properties do not make an item valuable.
- Unidentified candidates use installed game-table affix availability and native ALVL. Farming retains broader craft-only magic candidates using CRAFTALVL. The filter does not assume unidentified rolled stats.
- Added strong magic exceptions throughout late profiles, including skill/speed gloves, socket/block shields, socket/life armor, socket/movement circlets and stacked skill equipment.
- Profile 5 is balanced, 6–7 focused, and 8–11 require top combinations. Selected numeric stat thresholds are 5% more lenient than Melindaa's chosen baseline, rounded up; socket, skill and actual affix availability requirements remain exact.
- Preserved progressive runeword base selection, all uniques and runes, PD2 special-drop protection, potion/gem/gold policies, HR/WSS data, ROLL and stack labels.
- Added category regressions and checked exact and normalized duplicate directives in readable and distributed filters. No duplicate directives were found.

### [v1.2.56](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.56) — English profiles and compact stack labels

- Strictness names and descriptions are now in English. Removed the Melindaa name and version from profile lines to save space.
- Ground quantities appear only for stacks of two or more: `2x Key`, `5x Worldstone Shard`.
- Removed `x1` from single items, nonstackable equipment and single potions. Gold retains its usual amount display.
- Class-appropriate runeword ground recommendations are green. If no class recommendation matches, `Possible RW` lists compatible generic runeword names in gray.
- Item selection and PD2 special-drop protections are preserved.

### [v1.2.55](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.55) — PD2 special-drop protection

- Added explicit protection at every strictness for maps, map-upgrade materials and orbs, WSS, Puzzlebox, Puzzlepiece, Malus, crafting materials, fragments, essences, boss keys and other cataloged special items.
- Equipment modifier-count and set-roll requirements do not hide these items.
- Checked 180 game-table records, including 42 maps, at levels 0–11 across five qualities. Native map-tier detection also protects map codes outside the catalog.
- Quantities, prices and help continue processing. All 131 automated tests passed.

### [v1.2.54](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.54) — Item level in descriptions

- Final item descriptions end with plain text such as `Item level: 85`, using the item's actual level.
- Item level is displayed in the description rather than beside the item name.
- Quantity, price, recipe and ROLL information is preserved.

### [v1.2.53](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.53) — Stricter set selection

- From Endgame – Strict, level 9, known lower-tier sets no longer bypass selection through skill bonuses.
- This also covers corrupted lower-tier items when their set identity can be determined.
- Selected higher-tier sets retain a 90% minimum where their variable roll is supported and can be evaluated reliably.
- Ambiguous shared-base candidates and unsupported rolls remain conservative. Inventory items remain inspectable; unique visibility is preserved.

### [v1.2.52](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.52) — Ground quantities and gold thresholds

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

### [v1.2.51](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.51) — Useful-property selection

- From Farming Strict, identified magic equipment, rings and amulets require a combination of at least two useful properties.
- Identified rare equipment, rings and amulets require **3 / 4 / 4 / 5 / 6 / 6 / 6** useful properties at levels 5–11.
- This counts useful property categories, not exact affix slots. Multiple skill fields count once; weak incidental bonuses do not satisfy the thresholds.
- From Endgame, level 7, ordinary magic equipment is hidden, including skill items. Charms, jewels, rings and amulets have separate selection rules.
- Unidentified rare candidates retain separate base-selection checks because their actual bonuses cannot yet be evaluated.
- Identified magic/rare ground labels show actual bonuses, such as `+3 Bow skills` and `+20% IAS`.
- Runeword recommendations use full names; class recommendations and ordered rune recipes are highlighted in green in descriptions.

### [v1.2.50](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.50) — Clearer profiles and 90% set rolls

- Set a uniform **90%** minimum for supported identified set rolls in the last three profiles.
- A known lower roll cannot bypass the threshold through skill bonuses. Eligible fixed templates have no variable roll to grade.
- Unidentified, ambiguous or modified candidates retain conservative handling.
- Replaced terse profile abbreviations with full category names and clearer descriptions.

### [v1.2.49](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.49) — Visibility fixes and runeword bases

- Corrected rule-expansion order to match the actual PD2 filter engine. The previous error could leave hidden potions, scrolls, small gold piles and weak bases visible.
- Added regressions for observed Oil, HP, MP, Thawing, scroll and weak-equipment cases.
- Runeword base requirements become stricter from Farming: enhanced damage/defense thresholds at levels 5–11 are **5 / 8 / 10 / 12 / 15 / 18 / 20%**, with increasing relevant class and Paladin-shield requirements.
- The final profile requires maximum relevant base bonuses and actual recipe-compatible sockets. These base requirements do not apply to completed runewords.
- From Farming, `Possible RW` recommendations require a base that passes the selected profile's requirements.
- Narrowed ordinary magic and identified jewelry selection. Introduced late-profile set selection, refined by later releases.

### [v1.2.48](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.48) — Progression and reduced clutter

- Normal and Nightmare show all items.
- Hell and Baal Runs use cautious item-level guidance with useful-property and affix-potential exceptions. There is no hard ilvl-85 cutoff.
- Hell and Baal Runs retain Flawless and Perfect gems; Farming and higher retain Perfect gems. Runes, uniques and Perfect gems remain visible at every level.
- From Hell, hide Stamina, Thawing and Oil potions and loose Identify/Town Portal scrolls. Keep tomes.
- From Farming, hide Freezing/cold throwing potions.
- Restored purple rejuvenation labels: **35%** and **☺FULL☺**.

### [v1.2.47](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.47) — Initial skill-item protection

- Added protection for +2-or-higher all/class/tree/single-skill and oskill bonuses, and conservative unidentified-equipment handling.
- Protection continued through price, ROLL and help processing.
- Later releases replaced this blanket protection with specific magic, rare, set and runeword-base selection policies.

### [v1.2.46](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.46) — Original Melindaa selection engine

- Built a new Melindaa selection generator without using other filters as build inputs or rule templates.
- Runeword, crafting and item facts are derived from PD2 game tables.
- Preserved Melindaa HR/WSS displays, ROLL ratings, crafting help, class recommendations and visual features.
- Added generation-time duplicate-rule removal while preserving processing order.
- Current generator checks report zero duplicate complete ItemDisplay rules and zero external-filter runtime inputs. Those checks alone do not establish authorship of the entire project.

### Public licensing and distribution cleanup

- Removed Melindaa-specific usage restrictions and the separate restrictive Melindaa license from the public filter.
- Preserved required MIT rights, license notices and [MIT notice](./MIT-NOTICE.txt).
- The public repository distributes the prepared filter and documentation; authoring sources are maintained separately.
- Releases are available as ZIP and RAR archives. Filter updates are also installed locally and checked for matching contents.

Price dates change only when the price data itself is updated. Documentation-only changes do not increment the filter version.

---

## Lietuviškai

Melindaa naudoja mūsų sukurtas atrankos taisykles ir funkcijas. Čia aprašomi strictness, kainų, ROLL vertinimo, receptų ir daiktų žymų pakeitimai.

Įrašai pateikti nuo naujausio. Ankstesnių versijų taisykles gali pakeisti vėlesni atnaujinimai.

### v1.2.74 — Launcher metaduomenys ir aiškesnės trūkstamos kainos

- Pridėtas filter_definitions.json su vieninteliu Melindaa.filter įrašu; jis įtrauktas į būsimus viešus paketus ir atsisiuntimus.
- Daiktams be palaikomo įverčio rodoma "Estimated price: in development". Esamos skaitinės HR/WSS kainos ir jų duomenų datos išsaugotos.
- Paruoštas launcher registracijos įrašas oficialiu name/url/author formatu su dabartiniu Melindaa repozitoriumo adresu.

### v1.2.73 — Supaprastinti vieši dokumentai

- Iš dabartinio viešo paketo pašalinti atskiri ORIGINALITY ir THIRD-PARTY-NOTICES dokumentai bei jų README nuorodos. Vidinės patikros lieka privačios.
- Privalomas MIT autorių teisių ir leidimų tekstas išlaikytas nepakeistas **MIT-NOTICE.txt** bei atskiro filtro antraštėje. Žaidimo elgesys, atranka, kainos ir Melindaa pavadinimas nepakeisti nuo v1.2.72.

### v1.2.72 — Melindaa pavadinimas, siauresnė mėlynų atranka ir aiškus socketinimas

- Viešas projektas pervadintas į **Melindaa**: Melindaa.filter, žaidimo būsena, repozitoriumas, aprašymai ir Melindaa ZIP/RAR archyvai. Vietinis launcher pasirinkimas perkeliamas iš seno failo; senos kopijos išsaugomos atsarginėse kopijose ir pašalinamos.
- Farming with Blue slepia neidentifikuotus Magic throwing knives, throwing axes ir javelins, nebent bazė ETH ir elite. Esama potencialo ir identifikuotų statų patikra lieka; bendros craft išimties nepridėta. Rare, Crafted, Unique, saugomi kolekciniai daiktai ir ankstesni lygiai išsaugoti.
- RW rekomendacijos visuose lygiuose tikrina caster/merc bazės paskirtį. Žemesniuose lygiuose lieka daugiau tinkamų starter receptų, įskaitant Lore šalmus, bet staff nebesiūlomas Insight ar HOTO. Atrinktos Fury/Wind/Obsession bazės turi konkrečią paskirtį, ne bendrą techninį suderinamumą.
- Neaiškūs socketų metodų trumpiniai pakeisti į **Larzuk quest (Act 5)**, **Larzuk's Puzzlebox**, **Larzuk's Puzzlepiece** ir **Cube + Larzuk's Malus**. Talpos ribojami rezultatai ir esami socketai nepakeisti. Pagrindiniame aprašyme pridėti abiejų kalbų metodų pavyzdžiai.

### v1.2.71 — Endgame RW bazės be socketų

- Endgame leidžia atrinktas perf RW bazes su **0 socketų**, jei talpa leidžia atrinktą praktišką receptą. Jau socketintos bazės vis tiek turi tiksliai atitikti atrinkto recepto socketų skaičių.
- Žyma pervadinta į **[owned grail]** prie vardų ant žemės ir inventoriuje. Pridėta atskira abiejų kalbų Owned Grail lentelė apie native turėjimą, neidentifikuotų variantų ribas, pardavimo būsenos atnaujinimą ir turimos kopijos roll palyginimo nebuvimą.
- Perf aktualių bonusų patikros, abu Farming, gold ribos, kainos, owned inventoriuje ir PD2 apsaugos nepakeisti. Talpa negarantuoja socketinimo rezultato.

### v1.2.70 — Du Farming pasirinkimai, atsargesnės charmų kainos ir trumpesnė craft pagalba

- Pridėtas 5 lygio **Farming with Blue** su savarankiškai parašytais naudingais Magic deriniais ir affix potencialo kandidatais bei 6 lygio **Farming without Blue**, slepiantis visą įprastą Magic įrangą/jewelry. Charmai, jewels ir saugomi PD2 daiktai lieka. Abu Farming turi tą pačią Rare/Set/RW atranką; visi pagaminti craft matomi.
- Endgame dabar 7 lygis: įprasta mėlyna įranga paslėpta, palaikomas identifikuotų Rare/atrinktų Set roll 90%+, maksimalūs aktualūs RW bonusai ir tinkami socketai. Visi unique, neidentifikuoti rare ir saugomi kolekciniai daiktai išlieka. Ankstesnis Endgame vieną kartą perkeliamas į 7.
- Nuo Farming RW pagalba naudoja konkrečius praktinius bazės/recepto derinius. Caster staff nebesiūlomas Insight, bet kokiems melee nebesiūlomi Wind/Fury. Išsaugotos įprastos caster/buff, merc ir konkrečių buildų bazės pagal žaidimo receptus. Merc kandidatams ant žemės rodoma **Merc RW**, aprašyme **Possible merc RW**. Ankstesni lygiai palieka platesnius receptus; kokybės/socket ribos galioja.
- Gold ribos: 2 000 / 3 000 / 4 000 abiem Farming ir Endgame. Ankstesnių lygių ribos nepakeistos.
- Tik Gold Find turintys Magic charmai rodo **Estimated price: no reliable price for these mods**, be skaitinės ar skillerio kainos. Kiti pilnų modų derinių palyginimai išlieka atskiri.
- Atsparumai ant žemės rašomi **Fire res / Cold res / Light res / Poison res**, vietoj FR/CR/LR/PR.
- Craft ingredientai žymimi **Crafting material**, Perfect gemų receptai jų spalvomis. Receptai, ROLL ir kainos išsaugoti. Socketai rodo tik **Sockets: N/M**, be cannot add more.
- Išsaugota v1.2.69 [owned] prie inventoriaus vardo, ankstesnės poison/stat žymos, kainų pataisos ir apsaugos. Native nuosavybė negrąžina laikomos kopijos statų, todėl automatinis geresnio roll skirtumas neteikiamas.

### v1.2.69 — Nuosavybės žymos inventoriuje

- Unique/Set daiktai dabar žymimi **[owned]** prie vardo inventoriuje ir ant žemės pagal tą pačią atsargią native ALLOWNED patikrą. Vardai, ROLL ir kainų aprašymai išsaugoti.
- Žyma nurodo dabartinį turėjimą, bet ne turimos kopijos status ar roll. Automatinis roll palyginimas su laikomomis kopijomis neteikiamas. Ankstesni v1.2.63–68 atrankos, kainų ir išvaizdos atnaujinimai išsaugoti.

### v1.2.68 — Grąžinta kubo informacija ir kainų pastaba

- Farming Strict slepia visus Magic ginklus, šalmus, diržus, batus, pirštines ir skydus, taip pat circlet/klasių šalmus, ID ir unID, nepaisant bonusų. Žiedai, amuletai, kūno šarvai ir quiver išlaiko atrinktus Farming kandidatus. Endgame papildomai slepia visus Magic žiedus ir amuletus.
- Pataisyta charmų/jewel craft pagalba, kuri perrašydavo sukauptą ROLL informaciją. Palaikomas kintamas roll išlieka kartu su receptais ir kainomis, įskaitant parodytą 4% fire resist Small Charm (Roll 36%).

- Pataisyta kubo/tome aprašymų klaida, kai nauja eilutė pakeisdavo ankstesnes. Trumpos tęstinės taisyklės dabar išsaugo visą informaciją: filtro versiją, atnaujinimo laiką, bazinių kainų datą ir pasirinktą profilį. Kubo santrauka telpa į native aprašymo ribą.
- Kube pridėta trumpa pastaba, kad prašomos kainos gali būti nerealios ir negarantuoja pardavimo. Pagrindiniame README paaiškinta nerealių pardavėjų kainų įtaka įverčiams.
- Dvikalbis pagrindinis aprašymas perrašytas pagal visus šešis strictness profilius, tiksliai išvardijant Farming/Endgame skirtumus ir pakeitimus po v1.2.62.

### v1.2.67 — Poison damage žymos ant žemės

- Identifikuotų magic/rare/crafted daiktų žymos ant žemės rodo papildomą poison damage ir trukmę. Vidinis poison greitis perskaičiuojamas į bendrą žalą. Pataisyti vien poison turintys charmai, kuriems buvo rodomas tik dydžio žymėjimas.

### v1.2.66 — Be FIXED žymų ir vienoda socketų spalva

- Daiktai be kintamų roll neberodo FIXED. Fiksuoti runeword atpažįstami tyliai, kad negautų nepalaikomo roll įspėjimo.
- Antidote potionai vėl rodomi visuose strictness lygiuose.
- Socketų kiekiai, ribos, Larzuk/Puzzle/WSS/Cube būdai ir socketų išvalymo pagalba naudoja tą pačią šviesiai mėlyną TEAL spalvą kaip socketų žymos ant žemės. Taip pat nuspalvintos RW socketų kiekio antraštės ir talpos priminimai; klasės receptų pavadinimai lieka žali.

### v1.2.65 — Kiekio žymos ir kubo pagalba

- Pašalintos arrows, bolts ir mėtomų ginklų, įskaitant javelin, kiekio žymos visoms kokybėms bei ID/unID būsenoms. Kitų sunaudojamų daiktų ir medžiagų kiekiai išlieka.
- Kubo/tome būsena ir profilio pagalba suskaidyta į trumpas tęstines taisykles, kad būtų išvengta native BuildAction regex ribos, susijusios su pranešta kubo pavadinimo klaida. Patvirtinimas žaidime dar laukiamas.

### v1.2.64 — Endgame magic įrangos slėpimas

- Endgame slepia visus magic žiedus, amuletus, skydus, ginklus, diržus, pirštines, batus ir šalmus (įskaitant circlet ir klasių šalmus), identifikuotus ir neidentifikuotus, nepriklausomai nuo skill, socketų, ETH ar kitų bonusų. Farming išlaiko ankstesnę atranką. Magic kūno šarvų ir quiver atranka išlieka; charmai, jewel ir saugomi PD2 specialūs daiktai lieka matomi.

### v1.2.63 — Viso modų derinio kainų palyginimas

- Charmų ir magic jewel kainai pirmiausia naudojamas visas sutampantis modų derinys, sujungiant skirtingas skaitines roll reikšmes. Skill medžiai atskiriami; vieno modo charmams netaikomos dviejų modų skillerių kainos. Į visas charmų kainų sąlygas įtrauktos trūkstamos PD2 large charm bonusų išimtys.
- Rare/crafted palyginimuose išlieka pagrindiniai modai ir stipriausių papildomų modų roll intervalai; platesnės kainos be šių roll palyginimo nebetaikomos. Nepakankama imtis aiškiai paliekama be kainos. Atnaujinta ribota charmų modų derinių skelbimų imtis.

### [v1.2.62](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.62) — Silpnų RW bazių skill išimties pataisa

- Farming ir Endgame ta pati atrinktų RW bazių patikra taikoma ir vieno socketo bei socketų neturinčiai baltai/pilkai įrangai. Vien skill bonusas nebepalieka netinkamos bazės, įskaitant parodytą vieno socketo Burnt Wand. Ankstesni lygiai, pagaminti craft, unique ir saugomos PD2 medžiagos nepakeisti.
- Įtrauktos toliau aprašytos owned žymos, praktiški RW patarimai, trumpi statai, Item class aprašymai ir apytikslių kainų patobulinimai.

### [v1.2.61](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.61) — Owned žymos, praktiškos RW bazės ir aiškesni kainų įverčiai

- Pridėta **[owned]** žyma unique/set daiktams ant žemės, kai PD2 native kolekcijos būsena rodo, kad turimos visos galimos kandidatų grupės. Tai dabartinis turėjimas, ne radimo istorija ar radimų skaitiklis. Neaiškūs neidentifikuoti variantai vertinami atsargiai; owned niekada neslepia unique. Pardavus paskutinę kopiją žyma dingsta, kai PD2 praneša, kad daikto nebeturi; likus kitai kopijai žyma lieka. Ar būsena atsinaujina iškart, ar po naujo prisijungimo, dar reikia patikrinti žaidime.
- Magic atranka pakeista savarankiškais deriniais: Farming palieka platesnius naudingos įrangos derinius/potencialą; Endgame – siauresnes stiprių skill/speed, socket/block/life, sudėtų skill ir elite ETH kovinių kandidatų išimtis. Mėlynos craft-only bazės baigiasi po Baal. Visi pagaminti oranžiniai craft, charmai, jewels ir saugomi PD2 daiktai lieka matomi.
- Bendri techniškai galimų receptų sąrašai pakeisti praktiškomis bazės paskirties rekomendacijomis. Great Poleaxe taikiniai apima merc 4 socketų Insight/Infinity/Pride ir 5 socketų Obedience/Doomsayer; CTA naudoja žemų reikalavimų Crystal Sword/Flail. Klasei tinkamos rekomendacijos lieka žalios. Ant žemės rodoma iki trijų trumpų RW vardų ir likusių kiekis; pilnesnė receptų pagalba lieka aprašyme.
- Paaiškintas skirtumas tarp maksimalios talpos ir reikiamų socketų. Superior bazėms pašalintas tik normal kokybei tinkamas random socket Cube receptas. Reikia tikslaus recepto socketų skaičiaus; talpa negarantuoja socketinimo rezultato.
- Pridėtos paprastos Item class žymos įrangai ir palaikomoms kategorijoms, atskiriant Hammer/Mace/Club/Scepter/Polearm/Staff.
- Sutrumpinti bonusai ant žemės, pvz., **max dmg 1**, **min dmg 8**, **Ltng1-5** ir **GF8%**. Charmų/jewels kainų atitikimui pridėtas elementinio damage intervalų išskaidymas, išlaikant elemento ir skill tapatybę.
- Visos rinkos žymos pervadintos į **Estimated price**. Bendri unique/set įverčiai aiškiai nurodo, kad konkretus roll/socket/corruption neatitiktas. Datuotos prašomos kainos nėra garantuota pardavimo vertė.
- Pridėti 5 parų rare/crafted palyginamų daiktų intervalai pagal bazę/kokybę/ETH/socket ir pagrindinius modus bei jų ribas; platesni palyginimai aiškiai sujungia antrines savybes. Be pakankamai nepriklausomų skelbimų kaina neišgalvojama.
- Žinomiems baziniams daiktams nuo 1 HR suteiktas prioritetas tikslesniems 5 parų unique/set palyginimams pagal class/tree skills, pagrindinius roll, ETH ir tuščių socketų skaičių, kai duomenų pakanka. Nepalaikomam variantui rodomas paaiškinimas, o senas bendras įvertis pažymimas atskirai. Corrupted/užpildyti variantai nekainuojami kaip nepakeisti.
- Išplėstos RW bazių imtys pagal socketus, ETH, Normal/Superior ir ED/durability ribas. Pridėtos paprastų mapų ir mapų medžiagų/įrankių imtys iš aiškių vieneto pasiūlymų. Išridenti/pakeisti mapai nekainuojami kaip paprasti.
- Išsaugotas visos neidentifikuotos rare įrangos matomumas Farming/Endgame, visi unique grail kolekcijai, runos, Perfect gemai, pagaminti craft ir specialių drop apsauga. Pridėtos native owned, magic griežtumo, RW/socket, elementų bei brangių variantų patikros. Galutiniai tikslūs/normalizuoti dublikatų auditai įtraukti į leidimo patikrą.

### [v1.2.60](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.60) — Trumpi drop bonusai, 5 parų kainos ir aiškesnis Endgame

- Šešių profilių žaidimo santraukos sutrumpintos iki ne daugiau kaip 85 simbolių. Neaiškūs įrangos terminai pakeisti Magic/Rare gairėmis, `Perf gems` ir aiškiomis Endgame išimtimis. Pilna informacija lieka Cube bei specifikacijoje.
- Ant žemės sutrumpintai rodomi tikri identifikuotos įrangos, charmų ir jewels bonusai, pvz., `BarbSk1`, `DruSumm1`, `PoisDmg4%`, `IAS30%`, `STR24`. Identifikuoti charmai/jewels naudoja trumpas bazės žymas; svarbūs skill/damage bonusai eina prieš antrines savybes.
- Endgame slepia visą įprastą magic įrangą, identifikuotą ir neidentifikuotą, taip pat ETH daiktus, žiedus ir amuletus. Charmai, jewels, saugomi PD2 mapai/medžiagos ir visi pagaminti oranžiniai crafted daiktai lieka visuose profiliuose. Farming palieka naudingus magic įrangos derinius/potencialą, bet po Baal Runs vien craft potencialo mėlynai bazei nepakanka.
- Baltos/pilkos ETH runeword bazės vertinamos atskirai: Farming atranka laisvesnė, Endgame reikia maksimalių aktualių bonusų ir tikrų tinkamų socketų. Iš magic įrangos runeword nepagaminsi.
- Charmų/skillerių duomenys atnaujinti pagal 5 parų (120 val.) oficialių skelbimų/pakėlimų aktyvumą. Pridėta ribota magic jewels imtis ir paprastų Monarch įverčiai. Įverčiai galioja 5 paras; tikslūs stat deriniai turi pirmenybę prieš aiškiai pažymėtas apytiksles modų grupes.
- Palaikomos charmų/jewels/bazių kainos rodomos ir ant žemės, išlaikant bonusų žymas. Nepalaikoma rinkos kaina paaiškinama aiškiai; NPC gold yra atskira kaina. Įverčio nebuvimas nereiškia, kad nėra skelbimų. Kitų bazinių kainų pradinės datos išsaugotos.
- Išsaugotas visos neidentifikuotos rare įrangos matomumas Farming/Endgame, visi unique grail kolekcijai, runos, Perfect gemai, pagaminti craft ir saugomi PD2 daiktai. Pridėtos screenshot žymų, 5 parų galiojimo, kainų atitikimo ir Endgame magic slėpimo patikros.

### [v1.2.59](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.59) — Aiškesni magic ir runeword aprašymai

- Papildyti filtro aprašymas ir profilių tekstas žaidime: aiškiau paaiškinta esama magic/RW atranka. Šis leidimas keičia aprašymus, ne daiktų matomumą.
- Normal/Nightmare rodo visą magic įrangą; Hell/Baal taiko atsargią kandidatų atranką. Farming palieka atrinktas exceptional/elite ETH craft bazes ir stiprius derinius, pvz., skills + IAS, socketai + block ar socketai + life. Endgame ETH craft bazes siaurina iki elite, išlaikydamas stiprių magic derinių išimtis. Visi charmai ir jewels lieka matomi, taip pat jewels craftinimui.
- Farming RW bazės turi tikti pažangiems receptams; tik starter receptams, pvz., Lore, tinkamos bazės slepiamos. Lieka naudingos žemų reikalavimų CTA kardų/HOTO flailų išimtys. Endgame reikia maksimalių aktualių bazės bonusų ir tikrų receptui tinkamų socketų; vien aukšto item level nepakanka.
- Klasei rekomenduojami RW ir receptų pagalba žali; bendri tinkami variantai pilki. Atpažįstama klasė, ne tikslus build.
- Farming/Endgame palieka visą neidentifikuotą rare įrangą. Identifikuoti rare atrenkami pagal naudingus derinius; Endgame taiko 90%, kai galima patikimai vertinti. Farming palieka visus set; Endgame atrenka naudingus set su palaikoma 90% riba ir atsargiomis tapatybės/roll išimtimis. Visi unique lieka grail kolekcijai; runos ir saugomi PD2 specialūs daiktai matomi visada.

### [v1.2.58](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.58) — Šeši profiliai, platesnis rare matomumas ir lengvesnis inicializavimas

- Palikti Normal, Nightmare, Hell, Baal Runs, Farming Strict ir Endgame. Trumpi angliški žaidimo aprašymai paaiškina set atranką, Perfect gemus ir vėlyvas RW bazes be Melindaa/versijos prierašo.
- Farming ir Endgame palieka visą neidentifikuotą rare įrangą, kad sumažintume gero daikto praradimo riziką prieš identifikavimą. Kai kurie griežtesni atrankos būdai slepia daugiau tokių bazių ir priima šią riziką; mes sąmoningai pasirenkame didesnį matomumą. Paslėptų roll neatspėjame.
- Farming identifikuotą įrangą atrenka pagal kategorijai naudingus derinius. Endgame reikalauja stipresnių derinių ir 90%+ identifikuotiems rare/set, kai roll palaikomas ir patikimai įvertinamas. Nepalaikomiems/pakeistiems atvejams lieka atsargios išimtys.
- Farming rodo visus set. Endgame atrenka aukštesnio lygio/naudingus set, palieka neaiškias bendras bazes ir taiko 90%, kai galima. Visi unique lieka ir Endgame, kad žaidėjai galėtų rinkti unique grail kolekciją.
- Visuose profiliuose lieka charmai, jewels, jewel fragmentai, runos, mapai, PD2 orbai, craft/map-upgrade medžiagos, essences ir saugomi specialūs daiktai.
- Farming palieka atrinktas exceptional/elite ETH craft bazes bei vertingas skill/socket magic išimtis; Endgame ETH craft atranka siaurinama iki elite. Nuo Farming slepiami anti potionai. Gold minimumai: Farming 2 000, Endgame 3 000; abu rodo tik Perfect gemus.
- Farming RW bazės turi tikti pažangiems receptams, su naudingomis CTA/HOTO caster/buff išimtimis. Endgame reikia maksimalių aktualių bonusų ir tikrų tinkamų socketų. Starter-only bazės bei vėlyvos Lore rekomendacijos pašalintos.
- Bendros formulės ir kompaktiškas RW apdorojimas sumažino pirmo krovimo taisyklių išplėtimą bei pasikartojantį išraiškų kompiliavimą. Tikrą krovimo laiką ir ryšio nutrūkimą dar reikia patikrinti visiškai iš naujo paleidus PD2.
- Išsaugotos datuotos HR/WSS kainos, mūsų ROLL variklis, craft/socket pagalba, bonusai ant žemės, tik krūvelių kiekiai ir item level aprašymo apačioje. Pridėta dvikalbė filtro specifikacija.

### [v1.2.57](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.57) — Atranka pagal daikto kategoriją

- Bendrą modų skaičiavimą pakeitė Melindaa deriniai vienuolikai kategorijų: pirštinėms, batams, diržams, circlet tipo šalmams, kitiems šalmams, skydams, šarvams, ginklams, strėlinėms, žiedams ir amuletams.
- Identifikuotiems daiktams vertinamas aktualus pagrindinių ir papildomų bonusų derinys. Stiprus daiktas gali likti su mažiau savybių; daug silpnų savybių savaime vertės nesuteikia.
- Neidentifikuotų kandidatų atranka remiasi žaidimo lentelių affix galimybėmis ir native ALVL. Farming palieka platesnę magic crafting bazių atranką pagal CRAFTALVL. Nežinomi bonusai nėra spėjami.
- Vėlyvuose profiliuose paliktos stiprių magic derinių išimtys: skill/greičio pirštinės, socket/bloko skydai, socket/life šarvai, socket/judėjimo circlet ir besisumuojančių skill bonusų įranga.
- 5 lygis subalansuotas, 6–7 griežtesni, 8–11 reikalauja geriausių derinių. Mūsų pasirinktoms statų riboms taikomas 5% atlaidumas, apvalinant aukštyn; socketų, skill ir tikrų affix galimybių reikalavimai išlieka tikslūs.
- Išsaugota progresyvi RW bazių atranka, visų unique ir runų rodymas, PD2 specialių daiktų apsauga, potionų/gemų/goldo taisyklės, HR/WSS, ROLL ir krūvelių žymos.
- Pridėti kategorijų patikrinimai ir tikslių bei normalizuotų dublikatų auditas privačiame ir platinamame filtre. Pasikartojančių direktyvų nerasta.

### [v1.2.56](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.56) — Angliški profiliai ir trumpesnis kiekių rodymas

- Strict lygių pavadinimai ir aprašymai pakeisti į anglų kalbą. Iš profilių eilučių pašalintas Melindaa pavadinimas ir versija, kad tekstas užimtų mažiau vietos.
- Kiekis ant žemės rodomas tik tikroms krūvelėms nuo 2 vienetų: `2x Key`, `5x Worldstone Shard`.
- Nuo pavienių ir nesikaupiančių daiktų bei pavienių potionų pašalintas `x1`.
- Goldo pavadinimas išlaiko įprastą sumos rodymą. Atrankos taisyklės ir PD2 specialių daiktų apsauga išsaugotos.

- Klasei rekomenduojami runeword ant žemės rodomi žaliai. Kai klasei tinkamos rekomendacijos nėra, `Possible RW` rodo kitus suderinamus runeword pavadinimus pilkai.

### [v1.2.55](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.55) — PD2 specialių daiktų apsauga

- Visuose strict lygiuose atskirai apsaugoti mapai, jų gerinimo medžiagos ir orbai, WSS, Puzzlebox, Puzzlepiece, Malus, crafting medžiagos, fragmentai, essences, boss raktai bei kiti kataloge esantys specialūs daiktai.
- Šiems daiktams netaikomi įrangos modų skaičiaus ar set roll atrankos reikalavimai.
- Patikrinta 180 žaidimo lentelių įrašų, įskaitant 42 mapus. Apsauga tikrinta visuose 0–11 lygiuose ir penkiose kokybės kategorijose.
- Mapai papildomai apsaugoti pagal žaidimo map tier požymį, net jei jų kodo dar nėra kataloge.
- Išsaugotas tolesnis kiekių, kainų ir pagalbos rodymas. Praėjo 131 automatinis testas.

### [v1.2.54](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.54) — Item level aprašymuose

- Galutinio daikto aprašymo apačioje pridėta paprasta eilutė `Item level: 85` su tikru daikto lygiu.
- Item level žyma nededama prie daikto pavadinimo.
- Išsaugotas kiekio, kainų, receptų ir ROLL rodymas.

### [v1.2.53](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.53) — Griežtesnė set atranka

- Nuo **Endgame – Strict**, 9 lygio, atpažinti žemesnės kategorijos set daiktai nebepraeina atrankos vien dėl +skill bonusų.
- Tai taikoma ir corrupted daiktams, kai jų žemesnės kategorijos set tapatybę galima nustatyti.
- Atrinktiems geresniems set daiktams paliktas 90% minimumas, kai jų roll palaikomas ir patikimai įvertinamas.
- Neaiškūs bendros bazės kandidatai ir nepalaikomi roll atvejai saugomi atsargiai. Inventoriaus daiktai neslepiami; unique rodymas išsaugotas.

### [v1.2.52](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.52) — Daiktų kiekiai ir goldo ribos

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

### [v1.2.51](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.51) — Naudingų savybių atranka

- Nuo Farming Strict identifikuotiems magic įrangos daiktams ir žiedams/amuletams reikia bent 2 naudingų savybių derinio.
- Identifikuotai rare įrangai ir žiedams/amuletams 5–11 lygiuose reikia atitinkamai **3 / 4 / 4 / 5 / 6 / 6 / 6** naudingų savybių.
- Skaičiuojamos naudingos savybės, o ne tikslus affixų skaičius. Keli skill laukai skaičiuojami kaip viena savybė; silpni atsitiktiniai bonusai nepadeda pasiekti ribos.
- Nuo Endgame, 7 lygio, slepiama įprasta magic įranga, įskaitant +skill daiktus. Charms, jewels, žiedams ir amuletams taikoma atskira atranka.
- Neidentifikuoti rare kandidatai paliekami pagal atskiras bazės taisykles, nes jų tikrų bonusų dar negalima įvertinti.
- Ant žemės prie identifikuotų magic/rare daiktų pridėti tikri skill ir stat bonusai, pvz., `+3 Bow skills` ir `+20% IAS`.
- Runeword rekomendacijoms naudojami pilni pavadinimai; klasei rekomenduojami receptai ir runų eilė aprašyme pažymėti žaliai.

### [v1.2.50](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.50) — Aiškesni profiliai ir 90% set roll

- Paskutiniuose trijuose lygiuose palaikomiems identifikuotiems set roll nustatytas vienodas **90%** minimumas.
- Žinomas mažesnis roll nepraeina vien dėl +skill bonuso. Fiksuotiems tinkamiems šablonams, neturintiems kintamo roll, procentas nepriskiriamas.
- Neaiškūs, neidentifikuoti ar modifikuoti kandidatai vertinami atsargiai.
- Profilių aprašymuose trumpiniai pakeisti pilnais kategorijų pavadinimais ir aiškesniais paaiškinimais.

### [v1.2.49](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.49) — Slėpimo pataisos ir runeword bazės

- Pataisyta taisyklių išplėtimo tvarka pagal tikrą PD2 filtro veikimą. Ankstesnė klaida galėjo palikti matomus slepiamus potionus, scrolls, mažas goldo krūveles ir silpnas bazes.
- Pridėtos patikros pagal žaidime pastebėtus Oil, HP, MP, Thawing, scrolls ir silpnų įrangos daiktų atvejus.
- Runeword bazių atranka nuo Farming palaipsniui griežtinama: ED/defense ribos 5–11 lygiuose yra **5 / 8 / 10 / 12 / 15 / 18 / 20%**, kartu griežtinami aktualūs klasės ir Paladin shield bonusai.
- Paskutiniame lygyje reikia maksimalių aktualių bazės bonusų ir tikrų receptui tinkamų socketų. Jau pagamintiems runewords šios bazių taisyklės netaikomos.
- Nuo Farming `Possible RW` rekomendacijos rodomos tik bazėms, praeinančioms pasirinkto profilio atranką.
- Susiaurinta paprastų magic daiktų ir identifikuotos juvelyrikos atranka. Pradėta set atranka paskutiniuose trijuose lygiuose; vėlesnės versijos ją patikslino.

### [v1.2.48](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.48) — Progresija ir mažiau nereikalingų daiktų

- Normal ir Nightmare rodo visus daiktus.
- Hell ir Baal Runs naudoja atsargias item level gaires bei naudingų savybių ir affix potencialo išimtis. Griežto ilvl 85 slenksčio nėra.
- Hell ir Baal Runs rodo Flawless bei Perfect gemus; nuo Farming — tik Perfect. Runos, unique ir Perfect gemai rodomi visuose lygiuose.
- Nuo Hell slepiami Stamina, Thawing, Oil potionai ir palaidi Identify/Town Portal scrolls. Tomes paliekami.
- Nuo Farming slepiami Freezing/cold throwing potionai.
- Grąžintas violetinis rejuvenation rodymas: **35%** ir **☺FULL☺**.

### [v1.2.47](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.47) — Pradinė skill daiktų apsauga

- Pridėta +2 ar didesnių all/class/tree/single skill ir oskill bonusų apsauga bei neidentifikuotos įrangos saugojimas.
- Apsauga leido tęsti kainų, ROLL ir pagalbos apdorojimą.
- Vėlesnės versijos šią bendrą apsaugą pakeitė konkrečiomis magic, rare, set ir runeword bazių atrankos taisyklėmis.

### [v1.2.46](https://github.com/Melly87s/Melindaa/releases/tag/v1.2.46) — Originalus Melindaa atrankos pagrindas

- Sukurtas naujas Melindaa atrankos generatorius, nenaudojantis kitų filtrų kaip kūrimo įvesties ar taisyklių šablono.
- Runeword, crafting ir daiktų faktai imami iš PD2 žaidimo lentelių.
- Išsaugotas Melindaa HR/WSS kainų rodymas, ROLL vertinimas, crafting pagalba, klasės rekomendacijos ir vaizdinės funkcijos.
- Pridėtas pasikartojančių taisyklių šalinimas generavimo metu, išsaugant jų apdorojimo tvarką.
- Dabartinio generatoriaus patikros fiksuoja 0 vienodų pasikartojančių ItemDisplay taisyklių ir 0 kitų filtrų kaip vykdymo įvesčių. Šios patikros savaime nėra viso projekto autorystės įrodymas.

### Viešo filtro licencijos ir platinimo sutvarkymas

- Iš viešo filtro pašalinti Melindaa specifiniai naudojimo apribojimai ir atskira ribojanti Melindaa licencija.
- Išsaugoti privalomi MIT teisių ir licencijos įrašai bei [MIT įrašas](./MIT-NOTICE.txt).
- Viešame repozitoriume platinamas paruoštas filtras ir dokumentacija; generatoriaus šaltiniai palaikomi atskirai.
- Leidimai platinami ZIP ir RAR archyvais. Pakeitimai taip pat diegiami į vietines žaidimo filtro kopijas ir tikrinamas jų sutapimas.

Kainų datos atnaujinamos tik atnaujinus pačius kainų duomenis. Dokumentacijos pataisa filtro versijos nekeičia.
