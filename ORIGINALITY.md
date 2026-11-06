# Kiela v1.2.70: selection engine and preserved features

Kiela v1.2.46 replaces the former Kassahi-derived selection layer with a new
Kiela generator. The build does not load another author's filter, transform its
rules, expand its aliases or reuse its filtering expressions.

## What remains from Kiela

- HR / WSS market estimates in ground labels and item descriptions, with the
  original price-data dates and an explicit distinction from NPC gold prices.
- Exact and grouped charm, skiller and class-specific Torch estimates where
  the collected trade listings support them.
- The existing Kiela roll engine, including supported unique/set, rare, charm,
  magic jewel and runeword scalar ratings. Fixed properties do not inflate a
  variable roll percentage. Modified/unsupported cases retain CHECK.
- Class recommendations, socket counts and methods, base upgrades, and
  runeword guidance for both socketed and unsocketed equipment.
- Perfect-gem Caster, Blood, Hitpower, Safety, Bountiful, Brilliant and Vampiric
  crafting help, including the appropriate rune for each supported item slot.
- Charm reroll help, gem/rune upgrade help, potion recipes, compact ground
  labels, gem colors, rune numbers, charm size markers, built-in drop sounds,
  minimap markers and the cube's version/profile/build-time information.
- Eleven named Kiela strictness levels; Farming keeps only Perfect gems and
  hides ordinary HP/Mana potions; antidotes are hidden only at levels 10-11.

## New inputs and selection policy

119 runeword recipes, accepted bases and seven crafting families are derived
directly from the installed PD2 game tables. Source-file SHA-256 hashes are
recorded in the private build report. Recipes, item codes and game mechanics
are game facts, not claims of Kiela authorship.

Ground selection now uses explicit Kiela gates before any price/help return.
Inventory, quest items, uniques, sets, runes, maps and important materials are
protected. Base quality increases by profile; levels 9-11 require a maximum
relevant base roll or the documented skill/quiver exception. Rare and magic
equipment use separate Kiela progression requirements.

The old copied map-immunity/resistance reference table is omitted. Maps still
receive Kiela labels, markers and crafting guidance; no replacement resistance
values have been invented.

## Checks for this release

The readable generated source is compared with the archived Season 14 build
129 source **before** public symbol renaming:

- 0 identical complete ItemDisplay rules.
- 0 identical complete rules after ignoring whitespace and letter case.
- 0 exactly duplicated ItemDisplay rules in the new filter.
- 0 external-filter inputs in the runtime dependency graph.
- All 557 migrated Kiela core market quotes retain both their HR and WSS values.
- Existing roll regression fixtures and the native BH formula replacement
  syntax are tested alongside selection behavior across all eleven profiles.

Some simple conditions coincide: native quality checks such as UNI/SET, gem
grades, cube profile numbers and individual item codes. Text comparison alone
does not prove independent authorship or guarantee that no similarity exists.
This report concerns the current release; it does not rewrite the provenance
of earlier releases. Automated checks do not replace an in-game playtest.

## v1.2.47: skill safety

All strictness levels exempt +2-or-higher all/class/tree/single-skill and oskill
items from every hide gate. Unidentified magic and rare equipment is retained
until its affixes can be assessed. The protection is an exception to hiding,
not an early display return, so Kiela prices, roll ratings and help still run.

## v1.2.48: early progression

Normal/Nightmare show all items. Hell and Baal use cautious magic/rare ilvl
guidance (35/20 and 55/35), with protected categories, visible useful stats and
native-ALVL affix-potential exceptions. No ilvl-85 cutoff is used. Potential
+2 skills and selected useful modifiers are derived from PD2 affix/type tables,
including rare eligibility, staffmods and automagic. These exceptions may keep
weak rolls; they do not predict an unidentified item's actual affixes.

Hell/Baal retain Flawless and Perfect gems; Farming+ retain Perfect only.
Runes, uniques and Perfect gems remain visible at every level. From Hell,
hide Stamina/Thawing/Oil potions and loose ID/TP scrolls; keep tomes. Restored
purple rejuvenation ground and inventory labels: 35% and smiling FULL.

Freezing/cold throwing potions (all three sizes) remain visible through Baal Runs
and are hidden from Farming Strict (level 5) onward. Thawing potions remain
hidden from Hell as specified separately.

## v1.2.49: actual BH rule expansion and late selection

Corrected alias dependency order to match the one-pass BH engine. Added tests
that reproduce the old unresolved-alias failure and verify every published
condition resolves. Screenshot fixtures cover Oil/HP/MP/Thawing/scroll hiding,
weak magic shields/crossbow, the retained +3 Phoenix/+2 Blade Fury dagger, and
the excluded plain Chain Mail base.

Curated RW bases progressively require ED/defense 5/8/10/12/15/18/20 in profiles
5–11, Paladin resistance 20/22/24/26/28/29/30 or scaled physical automagic, and
skill tiers 1/2/2/2/3/3/3. Final candidates must have actual recipe-compatible
sockets and perfect relevant base bonuses; a visible +3 staffmod does not
excuse other displayed +1/+2 staffmods or partial ED/defense at that level.
Completed runewords are unaffected. Inventory is never hidden. Possible RW
recommendations from Farming now require a qualifying base even in inventory.

The final three set tiers use supported roll minima 70/80/90 on higher-level,
endgame-family, market-supported or explicitly useful templates. Unidentified
and unsupported candidate rolls are not guessed. Fixed eligible set templates
are not penalized for lacking a variable roll. Skill safety remains in place.

Farming magic candidates and identified jewelry are narrower. Final profiles
retain useful rare/charm/jewel exceptions, not blanket unidentified ordinary
blue equipment. Every profile name describes U/R/S/RW; read the menu legend in
the README. Automated checks do not replace an in-game playtest.

## v1.2.50: uniform 90% set threshold

Profiles 9, 10 and 11 now require 90% or better on supported identified set
rolls. A known lower roll no longer bypasses that requirement through a skill
bonus. Unknown/unidentified/modified candidate safeguards and fixed eligible
templates remain. Unique selection and other rarity policies are unchanged.

Profile summaries in this release use full category names and plain Lithuanian
words instead of U/R/S/RW shorthand or numeric rarity abbreviations.


## v1.2.51: useful properties and clear ground labels

Farming magic equipment/jewelry needs two useful properties. Identified rares need 3/4/4/5/6/6/6 useful properties at levels 5–11. From level 7 ordinary blue gear is hidden, including +skill items; charms/jewels/jewelry remain separately selected. These explicit requests supersede universal skill protection. Unidentified rare candidates remain because their stats cannot be graded. The score counts useful properties, not affix slots, and does not estimate market value. Ground labels expose actual identified bonuses; class RW labels use full names and green recipe text. HR/WSS snapshots and the 156 owned roll formulas are preserved.


## v1.2.52: quantities on every ground label

Every visible ground item now shows its actual stack count, or x1 for a nonstackable item. The count precedes the name to remain visible within the native name-length limit. Gem labels avoid double counts; potion and identified-equipment name replacements retain the count. HR/WSS figures remain the existing per-item estimates and are not multiplied by stack size.


From v1.2.52, Farming Strict gold minimum is 2000, rising by exactly 1000 at every subsequent level: profiles 5–11 use 2000/3000/4000/5000/6000/7000/8000. Earlier profiles retain their previous gold behavior. Every ground item shows an actual quantity or x1; gold shows its actual amount once.


## v1.2.53: enforce late set selection

From Endgame Strict (profile 9), lower-tier set templates no longer bypass set selection through +skill bonuses. This also applies to corrupted lower-tier items when their identity is known. Selected higher-tier/market-supported set candidates and the supported 90% roll requirement remain as before. Ambiguous shared-base or unsupported-roll candidates remain conservative; inventory and unique visibility are preserved. Levels 1–8 retain their existing set behavior.


## v1.2.54: item levels at the bottom of descriptions

Every final item description ends with plain text Item level: N. Item level is not included in ground or inventory names. This follows the user’s clarification; quantities, selection, prices, recipes and roll processing remain unchanged.


## v1.2.55: unconditional PD2 special-drop protection

Every hide gate explicitly excludes PD2 maps (including any native MAPTIER > 0), map modification materials/orbs, corruption shards, puzzle tools, crafting ingredients, fragments, boss keys/organs/essences, special books/keys, event/PvP maps and runes. Selection is based on installed game-table types and includes inactive/event records. The protected catalog contains 180 records, including 42 maps. Protection continues into quantity, price, recipe and roll handling; it is not an early terminal display return. Ordinary chest keys, consumable potions, lesser gems and equipment selection retain their requested policies.


## v1.2.56: English profiles and compact stack counts

Strictness names/descriptions use English and omit the Kiela/version prefix. Keep full readable category names. Quantity labels appear only when QTY > 1, with the number before x (2x Key, 5x Worldstone Shard). Single/nonstackable items and single potions have no 1x/x1 marker. Native gold labels keep their original amount. Quantity behavior must also survive potion and identified-equipment name resets. Other selection and PD2 special protections remain unchanged.

Class runeword ground recommendations are green. If no class-specific recommendation matches the base, display compatible generic runeword names in gray. Generic fallback still requires the same selected base and recipe-compatible socket/capacity checks.


## v1.2.57: category-based equipment selection

Replaced universal modifier counts with independently authored signatures for eleven equipment categories. Identified items need relevant core/support combinations; unidentified candidates use installed game-table affix availability and native ALVL/CRAFTALVL. Balanced selection at level 5, focused at 6–7, top combinations at 8–11. Selected numeric quality minima receive 5% leniency with whole-unit rounding; exact socket, skill and affix availability facts are preserved. Strong magic exceptions remain at every late profile. Progressive RW bases, all uniques/runes, PD2 special protection, gold/consumables, quantities, prices and the owned ROLL formulas remain. This entry supersedes the universal counts and blanket late-magic exclusion described in v1.2.51.

## v1.2.58

Six profiles now separate Farming and Endgame. Unidentified rare equipment remains visible to reduce loss risk; supported identified Endgame rare/set rolls require 90%. All uniques remain for grail collecting, and all charms/jewels and protected PD2 drops remain visible. Advanced RW purpose, selected ETH crafting and strong magic exceptions use our generator and game facts. Shared named expressions and compact recipe dispatch reduce initialization work without adding external filter inputs. See FILTER-SPECIFICATION.md for the bilingual current policy.

Šeši profiliai atskiria Farming ir Endgame. Neidentifikuota rare įranga lieka matoma praradimo rizikai mažinti; palaikomiems identifikuotiems Endgame rare/set reikia 90%. Visi unique lieka grail kolekcijai; charmai/jewels ir saugomi PD2 daiktai rodomi visada. Pažangios RW bazės, atrinktos ETH craft bazės ir magic išimtys remiasi mūsų generatoriumi ir žaidimo faktais. Bendros vardinės išraiškos ir kompaktiškas receptų apdorojimas mažina inicializavimo darbą. Dabartinė dvikalbė politika pateikta FILTER-SPECIFICATION.md.

## v1.2.60

Compact labels and five-day charm/jewel/base quote matching are independently implemented from owned models and official listing data. Endgame ordinary magic exclusion, permanent completed-craft visibility and post-Baal removal of craft-only blue bases follow the current product policy. Runtime builds still have no external-filter input.

Trumpi bonusai ir 5 parų charmų/jewels/bazių kainų atitikimas įgyvendinti savarankiškai iš mūsų modelių bei oficialių skelbimų. Endgame įprastų magic slėpimas, pagamintų craft matomumas ir mėlynų craft-only bazių atranka atitinka dabartinę politiką. Kiti filtrai nėra kūrimo įvestis.

## v1.2.62

The practical RW base-role shortlist, stricter late-Magic signatures, collection ownership labels, five-day comparable/variant models and compact names are independently authored. Inputs are retained owned models, installed PD2 facts, native BH condition documentation and official market observations. Other filters remain isolated comparison fixtures only.

Praktiškos RW bazių paskirtys, griežtesni vėlyvi Magic deriniai, kolekcijos turėjimo žymos, 5 parų palyginimų/variantų modeliai ir trumpi vardai parašyti savarankiškai. Naudojami mūsų modeliai, įdiegto PD2 faktai, native BH sąlygų dokumentacija ir oficialūs rinkos stebėjimai. Kiti filtrai lieka tik izoliuotais palyginimo pavyzdžiais.
