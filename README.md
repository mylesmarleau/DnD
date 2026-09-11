# D&D Character Manager

A single-file, offline-first character sheet manager for in-person D&D sessions. No install, no server, no internet connection required at the table.

## Using it

Open `index.html` in any browser (double-click the file, or host it — e.g. with GitHub Pages — and open the URL). Everything autosaves to your browser's local storage as you type.

**Recommended:** since local storage lives in one browser, use **Export** regularly to download your character as a `.json` backup file, and **Import** to load it on another device or after clearing browser data.

### New to D&D?

Turn on **Beginner Mode** in the top bar to show short explanations under each section of the sheet (what a saving throw is, how to attack, what AC means, what to do on your turn, etc.). Click **New Player Guide** any time for a fuller one-page walkthrough of the basics — the three kinds of rolls, how a combat turn works, and what to do when you take damage. Neither of these need to be memorized; they're there to glance at mid-session.

## Features

- Character info: name, class, level, race, background, alignment, XP (with an auto "XP to next level" readout and a level-up flag once you've earned enough), proficiency bonus (auto-calculated), inspiration tracker
- Ability scores with auto-computed modifiers, and one-click ability checks
- Saving throws and all 18 skills with proficiency/expertise toggles, auto-computed bonuses, and one-click rolls
- Passive Perception (auto-computed)
- Combat panel: AC, initiative, speed, hit dice
- HP tracker with quick damage/heal buttons (temp HP is consumed first), death save pips, concentration tracker, and a condition/exhaustion tracker
- Attacks & Spellcasting list with a "Roll" button per attack
- Spellcasting: save DC, attack bonus, and spells-prepared count (all auto-computed), spell slots by level with click-to-mark-used pips, and a free-text spell list
- Class Resources tracker (Rage, Ki, Sorcery Points, Bardic Inspiration, etc.) with a reset rule per resource (manual / short rest / long rest)
- Equipment: currency (CP/SP/EP/GP/PP) and an inventory list
- Features & Traits, Proficiencies & Languages, and Personality/Notes sections
- **Roll Reference** log: click any Roll button (ability, save, skill, attack, initiative) to see the modifier to add — you roll your own physical dice and add it yourself
- Short Rest / Long Rest buttons that reset HP, hit dice, spell slots, and resources per the 5e rules
- Manage multiple characters (New / Duplicate / Delete / switch), all stored locally in your browser

### Level Up system

Click **Level Up** to walk through leveling up: choose to take the average HP gain, or roll your own physical hit die and type in the result, note any new features/ASI/feat gained (auto-appended to Features & Traits), and confirm. This updates your level, proficiency bonus, HP max/current, and hit dice, and logs the level-up in a **Level History** list on the Character panel.

### Artificer support

- **Infusions & Attunement panel**: known infusions list with the max-known count auto-computed from your level, an infused-items list capped by level (2/3/4/5/6 at levels 2/6/10/14/18), and an attunement tracker with an editable max slots (base 3, +2 more if attuning to your own infusions) — separate from the max infused-items count since not every infusion needs attunement.
- **Spells Prepared**: auto-computed (½ level, rounded down, + spellcasting ability modifier, minimum 1) next to Save DC and Attack Bonus.
- **Companion / Construct panel**: a mini stat block for a Steel Defender, Eldritch Cannon, or Homunculus Servant — AC, speed, its own HP tracker, attack bonus/damage with a roll button, and a notes field for special reactions like Deflect Attack or Repair.
- **Class Resources** doubles as a tracker for Infuse Item uses (if you track them separately), Flash of Genius, or any subclass-specific resource, with per-resource short/long rest reset rules.

### Combat Tracker

A dedicated panel for running your turns at the table:
- Round counter with **Next Round** (resets your action economy and ticks down active effect durations) and **Reset Combat**
- **Roll Initiative** button using your DEX modifier (or manual initiative bonus if set)
- Action / Bonus Action / Reaction toggles that reset automatically each round, plus a movement-used tracker
- A turn sequence reference (move, action, bonus action, reactions, end-of-turn effects) so you don't miss a step
- An Active Effects list for ongoing conditions/buffs with a rounds-remaining counter that counts down as you advance rounds

## Backing up / moving between devices

Use **Export** to download the active character as a JSON file, and **Import** to load a JSON file back in (on this device or any other browser). This is your safety net — local storage can be cleared by the browser, so back up before and after sessions if your character matters to you.

## Included characters

- `characters/nine.json` — Nine, a level 1 Artificer (Artillerist path). Open `index.html`, click **Import**, and select this file to load him in.
