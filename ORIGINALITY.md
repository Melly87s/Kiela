# Kiela v1.2.46: selection engine and preserved features

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
