# Kiela v1.2.45

Project Diablo 2 loot filter with clear item labels, graded symbol accents and
automatic player-class runeword recommendations.

**[Download Kiela.rar](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.rar)** · **[Download Kiela.zip](https://github.com/Melly87s/Kiela/releases/latest/download/Kiela.zip)**

**[Lietuviška instrukcija](#diegimas-lietuviškai)** · **[English instructions](#installation-english)**

Official project: https://github.com/Melly87s/Kiela

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
lygį turi būti rodomas profilio pavadinimas su **Kiela v1.2.45**.

Pasirink norimą **Filter level / strictness**. Pradėk nuo žemesnio lygio ir kelk
jį pagal poreikį: aukštesnis strict slepia daugiau paprastų daiktų ir reikalauja
geresnių atrinktų runeword bazių statų. Nuo 5 lygio nišinės bazės slepiamos;
kovinėms bazėms taikomi 5 / 10 / 15 ED slenksčiai, paladino skydams –
20 / 25 / 30 res. Naudingi +3 skill bazių variantai išlaikomi. Tinkamų socketų
Crystal / Broad / Long Sword, Flail ir Monarch išimtys nereikalauja ED.
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
   look for **Kiela v1.2.45** in the displayed profile name. Start with a
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
  Exact-roll matches take priority; pooled estimates are labeled **Approx. / all rolls**.
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

## Authorship and use

Copyright (c) 2026 Melinda Kiela, original Kiela contributions only.
Kiela builds on the third-party work acknowledged in
**[THIRD-PARTY-NOTICES.md](./THIRD-PARTY-NOTICES.md)**.

Free to download and use for PD2 under the scoped
**[Kiela terms](./LICENSE-KIELA.md)**. Do not pass off Kiela's original contributions
as your own work or rebrand modified copies without permission. Upstream MIT
rights remain unchanged; the standalone filter embeds the MIT notice.

This repository contains the prepared filter and release documents. The generator
and readable authoring sources are maintained separately.
