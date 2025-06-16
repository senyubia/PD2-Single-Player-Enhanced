# PD2-Single-Player-Enhanced
## What is it
Mod for Project Diablo 2 to enhance single player experience, mainly by improving drop rates of certain items and adding some QoL™ changes, while maintaining fairness.

Based on [Project Diablo 2 Single Player+ mod by Lukaszpg](https://github.com/Lukaszpg/PD2-Single-Player-Plus-mod) v11.0.3. Check it out!

## How to use it
If you haven't done it already, run the official PD2 launcher and set up your desired loot filter. Then:

1. Get **PD2 S11 patch 2. This is important!** For other versions you'll have to manually merge differences into corresponding .txt files.
2. Download ``data`` folder and place it in ``<YOUR D2 INSTALL PATH>/ProjectD2/``. Due to git quirkiness, on Windows (and *maybe* while using wine on *nix) you might have to change line endings to CRLF if your game crashes on launch.
3. Create a new shortcut to ``<YOUR D2 INSTALL PATH>/ProjectD2/Diablo II.exe`` and include ``-direct -txt`` option string. You might also want to include ``-3dfx`` option if you plan on using D2GL.
4. Use the newly created shortcut to play the game.

If you want to play vanilla PD2, run the exe without ``-direct -txt`` options (or use the official launcher).

If for some reason you don't want to deal with the separate shortcut to run the game, you could always patch ``pd2data.mpq`` yourself with generated .bin files from running with above options. Of course by doing that you'll lose the ability to easily switch between the mod and vanilla PD2.

Your existing characters *should* be compatible with the mod. As long as your characters don't hold mod-exclusive items, modded characters *should* be compatible with vanilla PD2. As always, doing a backup of your characters before running the mod is highly recommended.

Using this mod online with the official PD2 gateway will *most likely* result in a ban.

## What is changed
For the complete list of changes, get official PD2 (or SP+) .txt files and diff them with included files.

**Main changes compared to vanilla PD2:**
- cubing DClone, Rathma and Lucion ingredients give 3 separate entry talismans,
- slightly improved drop rate of maps scrolls in maps,
- NoLimit flag for not-encounter-locked uniques set to 1 (the same unique may drop multiple times in a single game),
- modified rarity of uniques with the same base (e.g. Tyrael's Might or high-level jewelery is more common),
- improved drop rates for runes (r1-r8 vanilla, r9-r16 3x, r17-r24 5x, r25-r33 20x),
- improved drop rate for Horadrim Scarabs,
- improved drop rates for uber ingredients,
- improved drop rates for super-rare utility items (e.g. puzzlepieces, mirrors, vials),
- improved roll chances for desired charm affixes (e.g. skillers, life),
- new items: Exalted Orb (used to craft set items), Mythic Orb (used to craft unique items), Gheed's Curious Box (contains random 50 pgems), Eternal Coin (used in cubing recipes),
- added safe unsocketting recipe (don't eat socketed items) - item + Ist + tp scroll,
- Token of Absolution from Akara costs 2.5m, up from 500k,
- new charm: Cain's Wisdom, cube any grand charm with 1 of each essence.

**Main changes compared to PD2 Single Player+:**
- Cain's Wisdom is now a grand charm,
- Cain's Wisdom can drop starting from alvl 67; rarity set to 1, while Gheed's Fortune has rarity 9 (and alvl 70 as in vanilla),
- modified improved drop rates (in general, rates are lower compared to SP+),
- ItemType for new items changed to ``Single Player Orb`` with ID ``spob``,
- Eternal Coin ID changed to ``ecoi``,
- Eternal Coin ItemType changed from ``scro`` to ``spob``,
- Eternal Coin costs 1m,
- Eternal Coin used in most cubing recipes (3/2 used for uniques, 1 for sets, 3/2/1 used to downgrade HRs, 2 used to combine 3 puzzlepieces into a box, 1 used to combine 6 Exalted Orbs into a Mythic Orb, 1 used to open Gheed's Curious Box),
- mob resists in t4s are the same as in vanilla.
