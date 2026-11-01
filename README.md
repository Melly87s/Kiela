# Kiela v1.2.40

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
lygį turi būti rodomas profilio pavadinimas su **Kiela v1.2.40**.

Pasirink norimą **Filter level / strictness**. Pradėk nuo žemesnio lygio ir kelk
jį pagal poreikį: aukštesnis strict slepia daugiau paprastų daiktų ir reikalauja
geresnių runeword bazių statų. Aukščiausias lygis nėra skirtas parodyti viską.

Filtro griežtumo didinimo ir mažinimo klavišus priskirk pačiame žaidime per
**Configure Controls**. Pavyzdžiui, gali pasirinkti **F7** mažinimui ir **F8**
didinimui, jei jie nesikerta su tavo įgūdžių klavišais. Filtras pats klavišų nekeičia.

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
   look for **Kiela v1.2.40** in the displayed profile name. Start with a
   lower level; higher strictness intentionally hides more items and weaker bases.
5. Assign increase/decrease strictness keys in the game's **Configure Controls**
   if desired. F7/F8 are an example, not automatic bindings supplied by the filter.

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
- **Possible RW: ...** on a ground base recommends a compatible runeword for the
  current player class. Recommended runeword names are **green** in item tooltips.
  Class detection is automatic; build detection is not. Druid preferences are
  tuned for **Summon**. Add the required sockets before inserting runes.
- In the possible-runeword list, **2s / 3s / 4s / 5s / 6s** mean the required
  number of sockets. Ordinary entries are dark gray; class recommendations are green.
- Green recommendations include the runes in insertion order. On unsocketed bases,
  very long lists may end with **+N other RW** to fit PD2's tooltip limit.
  Socketed bases show matching recipes for their exact socket count.
- Socket tips show the base cap and method limits: **Larzuk** = quest,
  **Piece / Box** = Larzuk's Puzzlepiece / Puzzlebox, **Malus** = Larzuk's Malus.
  **WSS max** is a possible corruption result, not a guaranteed safe outcome.
- Gem tooltips list all crafting slots and their runes by gem family. Crafting
  requires a **Perfect** gem; lower grades show the upgrade reminder.
- **Price** is the NPC vendor sell-price field. **Global price** is an available
  market estimate, not the amount an NPC pays and not a guaranteed sale.
- **Roll %** rates tracked variable stats; it is not a universal build score or
  a guarantee that an item is valuable.
- Red and blue potion labels show recovery amounts, for example **+320** and **+250**.

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
