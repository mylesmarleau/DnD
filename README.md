# D&D Character Manager

A single-file, offline-first character sheet manager for in-person D&D sessions. No install, no server, no internet connection required at the table.

## Using it

Open `index.html` in any browser (double-click the file, or host it — e.g. with GitHub Pages — and open the URL). Everything autosaves to your browser's local storage as you type.

**Recommended:** since local storage lives in one browser, use **Export** regularly to download your character as a `.json` backup file, and **Import** to load it on another device or after clearing browser data.

## Features

- Character info: name, class, level, race, background, alignment, XP, proficiency bonus (auto-calculated)
- Ability scores with auto-computed modifiers, and one-click ability checks
- Saving throws and all 18 skills with proficiency/expertise toggles, auto-computed bonuses, and one-click rolls
- Passive Perception (auto-computed)
- Combat panel: AC, initiative, speed, hit dice
- HP tracker with quick damage/heal buttons (temp HP is consumed first), death save pips, concentration tracker, and a condition/exhaustion tracker
- Attacks & Spellcasting list with a "Roll" button per attack
- Spellcasting: save DC and attack bonus (auto-computed), spell slots by level with click-to-mark-used pips, and a free-text spell list
- Equipment: currency (CP/SP/EP/GP/PP) and an inventory list
- Features & Traits, Proficiencies & Languages, and Personality/Notes sections
- Built-in dice roller (d4–d100, multiple dice, modifiers, advantage/disadvantage) with a roll log
- Short Rest / Long Rest buttons that reset HP, hit dice, and spell slots per the 5e rules
- Manage multiple characters (New / Duplicate / Delete / switch), all stored locally in your browser

## Backing up / moving between devices

Use **Export** to download the active character as a JSON file, and **Import** to load a JSON file back in (on this device or any other browser). This is your safety net — local storage can be cleared by the browser, so back up before and after sessions if your character matters to you.
