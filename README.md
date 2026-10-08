<p align="center"><img src="mod/one_click_vassal_transfer/thumbnail.png" width="256" alt="One-Click Vassal Transfer"></p>

# One-Click Vassal Transfer

A Crusader Kings III mod that lets you reorganize your realm in a single click: grant your counties to brand-new vassals, create every title you are entitled to, and hand duchies, kingdoms and empires to the vassals who rule their de jure capitals.

- **Game version:** 1.20.x
- **Mod version:** 1.1.0
- **Author:** [Sourenics](https://github.com/Sourenics)
- **Steam Workshop:** [One-Click Vassal Transfer](https://steamcommunity.com/sharedfiles/filedetails/?id=3816024693)

## Features

A new **Title Distribution** group in the Decisions tab. Each decision is independent and acts on a single rank, all at once:

| Decision | What it does | Shown to |
|---|---|---|
| **Transfer Vassals to their De Jure Liege** | Every direct vassal swears fealty to the vassal who holds their de jure liege title. | Dukes and above |
| **Grant Counties (Your Culture)** | Every county in your domain goes to a **brand-new character** of your culture, faith and rite: one county, one new vassal. Courtiers, family and councillors are never used. | Dukes and above |
| **Grant Counties (Local Culture)** | Same, with a new character of each county's culture, faith and rite. | Dukes and above |
| **Create Duchies / Kingdoms / Empires** | Creates every title of that rank the game currently lets you create, using the game's own list of creatable titles. Free of charge. | Duchies: dukes and above. Kingdoms: emperors. Empires: hegemons. |
| **Distribute Duchies / Kingdoms / Empires** | Each title goes to the vassal who holds its **de jure capital sub-title**, working down until someone qualifies: an empire to the holder of its capital kingdom, then of its capital duchy, then of its capital county; a kingdom to the holder of its capital duchy, then of its capital county; a duchy to the holder of its capital county. As a last resort, it goes to the vassal with the most counties in it. Its de jure vassals then move under the new holder and are sorted beneath them. | Duchies: kings and above. Kingdoms: emperors. Empires: hegemons. |

The **Effects** section of every grant and distribution decision lists each title that will be handed out and who will receive it, before you confirm.

### Excluding titles

Open any title you hold: a new round button next to **Make Primary** toggles it between ✓ (included) and ✗ (excluded). Excluded titles are never granted or distributed.

### No bordergore

A title is only given to a vassal whose **primary title lies de jure within it**. Where a vassal physically lives does not matter: a Duke of Bavaria who resides in a Saxon county receives the Kingdom of Bavaria, never the Kingdom of Saxony. If no vassal qualifies, you keep the title, and the Effects preview tells you so before you confirm.

### What is never handed out

- Your capital county.
- Your primary title, and any title that contains your capital de jure.
- Titles marked as excluded.

### Who can receive titles

Only adult, free, capable vassals who are not at war with you. Theocratic vassals only receive titles if you are a theocracy yourself. Vassals at war with you, or with a vassal of theirs at war with you, are never moved to a new liege.

## Installation

### Steam Workshop

Subscribe on the Steam Workshop page and enable the mod in the Paradox launcher.

### Manual

1. Download this repository (green **Code** button → **Download ZIP**).
2. Copy the contents of the `mod/` folder (`one_click_vassal_transfer/` and `one_click_vassal_transfer.mod`) into:
   - **Windows:** `Documents/Paradox Interactive/Crusader Kings III/mod/`
   - **Linux:** `~/.local/share/Paradox Interactive/Crusader Kings III/mod/`
   - **macOS:** `~/Documents/Paradox Interactive/Crusader Kings III/mod/`
3. Enable **One-Click Vassal Transfer** in the Paradox launcher.

## Compatibility

- No DLC required.
- Can be added to or removed from an existing save.
- Overrides one vanilla file, `gui/window_title.gui`, with a single button added for the exclusion toggle. Other mods that replace the same file, such as **Rise and Fall**, will conflict: only the button of the mod loaded last will appear.
- All decisions are player-only. The AI never uses them.

## Reporting bugs

Please open an [issue](../../issues/new/choose) using the **Bug report** template. To be able to fix the problem we need:

1. **The `error.log` file** from the session where the problem happened:
   - **Windows:** `Documents/Paradox Interactive/Crusader Kings III/logs/error.log`
   - **Linux:** `~/.local/share/Paradox Interactive/Crusader Kings III/logs/error.log`
   - **macOS:** `~/Documents/Paradox Interactive/Crusader Kings III/logs/error.log`

   The log is overwritten every time the game starts, so copy it right after the problem happens, before launching the game again. Ideally, reproduce the problem in a session with **only One-Click Vassal Transfer enabled**.
2. **The game version** (shown in the main menu, for example 1.20.0.4) and **the mod version**.
3. **Your active DLCs** and **your full mod list in load order**.
4. **Which decision** was involved, and your rank (duke, king, emperor…).
5. **Steps to reproduce:** what you clicked and what happened, compared to what you expected.
6. **Screenshots**, if the problem is visual (wrong text, missing button, empty tooltip).

## Credits

The idea comes from the title automation decisions of the **Rise and Fall** mod. This mod is an independent reimplementation written from scratch: it does not include Rise and Fall code and does not depend on it. The main difference is that counties always go to newly created characters, never to existing courtiers.

## License

**One-Click Vassal Transfer** © 2026 Sourenics, licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).

Forks, translations and alternative versions are welcome, provided that you:

- **Credit the original author** (Sourenics) and link to this repository.
- **Indicate the changes** you made.
- **Release your version under the same license** (CC BY-SA 4.0).

### Paradox Interactive content

Crusader Kings III and its content are © Paradox Interactive AB and are **not** covered by this license. This includes the vanilla localization keys referenced by the mod and the vanilla file `gui/window_title.gui`, which is included with one button added. This project is an unofficial fan-made mod, not affiliated with or endorsed by Paradox Interactive. Like every CK3 mod, it must be distributed free of charge.
