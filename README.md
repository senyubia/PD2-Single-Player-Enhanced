# PD2-Single-Player-Enhanced
Updated to: **S12 patch 2**
## What is it
Mod for Project Diablo 2 to enhance single player experience, mainly by improving drop rates of certain items and adding some QoL™ changes, while maintaining fairness.

Based on [Project Diablo 2 Single Player+ mod by Lukaszpg](https://github.com/Lukaszpg/PD2-Single-Player-Plus-mod) v11.0.3. Check it out!

## How to use it
1. Patch the game to the supported version. For other versions you'll have to manually merge differences into corresponding .txt files. If you don't, any of these can happen: game will work fine, game will crash on character load, game will launch but you won't have access to newest changes from PD2 patch.
2. Download ``data`` folder and ``loot.filter`` and place them in ``<YOUR D2 INSTALL PATH>/ProjectD2/``.
3. Create a new shortcut to ``<YOUR D2 INSTALL PATH>/ProjectD2/Diablo II.exe`` and include ``-direct -txt`` option string. You might also want to include ``-3dfx`` option if you plan on using D2GL.
4. Use the newly created shortcut to play the game.

If you want to play vanilla PD2, run the exe without ``-direct -txt`` options (or use the official launcher).

If for some reason you don't want to deal with the separate shortcut to run the game, you could always patch ``pd2data.mpq`` yourself with generated .bin files from running with above options. Of course by doing that you'll lose the ability to easily switch between the mod and vanilla PD2.

Existing characters should be compatible between vanilla and modded (and backwards). There might be some issues with unique/set items with changed ID, so after transfer if you see items with wrong names or wrong sprites/types, you should either delete them, regenerate them using a custom cube recipe, or keep them at your own risk.

Using this mod online with the official PD2 gateway might result in a ban.

## What do new items do
Check their notes from the loot filter.

## What is changed
For the complete list of changes, get official PD2 (or SP+) .txt files and diff them with included files. Also check release info for more up to date changes.

**Main changes compared to vanilla PD2:**
- NoLimit flag for not-encounter-locked uniques set to 1 (the same unique may drop multiple times in a single game),
- modified rarity of uniques with the same base (e.g. Tyrael's Might or high-level jewelery is more common),
- quest bug always active on all act bosses,
- improved drop rates for runes (r1-r8 vanilla, r9-r16 3x, r17-r24 7x, r25-r33 20x),
- improved drop rate for Horadrim Scarabs,
- improved drop rates for uber ingredients,
- improved drop rates for super-rare utility items (e.g. puzzlepieces, mirrors, vials),
- improved drop rates for uniques/sets,
- improved roll chances for desired charm affixes (e.g. skillers, life),
- improved sell values on higher difficulties - they continue on increasing by 5k per act,
- new items: Exalted Orb (used to craft set items), Mythic Orb (used to craft unique items), (Opened) Gheed's Curious Box (contains random 50 pgems), Eternal Coin (used in cubing recipes), Transient Coin (used in armour/weapon set/unique crafting),
- added safe unsocketting recipe (don't eat socketed items) - item + Ist + tp scroll,
- new grand charm: Cain's Wisdom,
- crafting infusions can be crafted - 1 corresponding pgem + 1 jewel fragment + Fal,
- using 3 Larzuk's Puzzlepieces and Eternal Coins you can upgrade them to Larzuk's Puzzlebox,
- Anya sells HRs, rejuvs, rare misc items (including ToA moved from Akara) and mod items; you might need Gheed's Fortune to buy some of them,
- changed launch splash, main menu, tcp/ip menu and character select screens to LoD (delete ``data/global/ui`` if you don't want that).

**Main changes compared to PD2 Single Player+:**
- removed recipes to downgrade runes,
- Cain's Wisdom is now a grand charm requiring clvl 88 to use,
- Cain's Wisdom can drop starting from alvl 87,
- removed the recipe to turn essences into Cain's Wisdom,
- modified improved drop rates (in general, rates are lower/worse compared to SP+, still more reasonable than vanilla),
- ItemType for new items changed to ``Single Player Orb`` with ID ``spob``,
- Eternal Coin ID changed to ``ecoi``,
- Eternal Coin ItemType changed from ``scro`` to ``spob``,
- Eternal Coin used in most cubing recipes (check lootfilter notes on orbs),
- deterministic unique/set creation - cube a base with an orb (and a Transient Coin if base is armour/weapon) to create a random unique with +100 lvl req, pick the desired item by repeating the transmutation with the orb only (the orb gets refunded), then cube with Eternal Coins to finalize the transmutation (the orb and coins get consumed, the item gets rerolled into a proper version),
- mob resists in t4s are the same as in vanilla.
