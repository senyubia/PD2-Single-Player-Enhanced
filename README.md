# PD2-Single-Player-Enhanced
Updated to: **S14 patch 2**
## What is it
Mod for Project Diablo 2 to enhance single player experience, mainly by improving drop rates of certain items and adding some QoL™ changes, while maintaining fairness.

Inspired by [Project Diablo 2 Single Player+ mod by Lukaszpg](https://github.com/Lukaszpg/PD2-Single-Player-Plus-mod) v11.0.3.

## How to use it
1. Patch the game to the supported version. For other versions you'll have to manually merge differences into corresponding files. If you don't, any of these can happen: game will work fine, game will crash on character load, game will launch but you won't have access to newest changes from PD2 patch.
2. Download ``data`` folder and ``loot.filter`` and place them in ``<YOUR D2 INSTALL PATH>/ProjectD2/``.
3. Create a new shortcut to ``<YOUR D2 INSTALL PATH>/ProjectD2/Diablo II.exe`` and include ``-direct -txt`` option string. You might also want to include ``-3dfx`` option if you plan on using D2GL.
4. Use the newly created shortcut to play the game.
5. If you want to play vanilla PD2, run the exe without ``-direct -txt`` options (or use the official launcher).

Existing characters are compatible with this mod, the other way around can work if you don't have custom items in the inventory and stash.

You might also be interested in [patched BH.dll with additional features](https://github.com/senyubia/PD2-BH).

## What do new items do
Check their notes from the loot filter.

## What is changed
- NoLimit flag for not-encounter-locked uniques set to 1 (the same unique may drop multiple times in a single game),
- modified rarity of uniques with the same base (e.g. Tyrael's Might or high-level jewelery is more common),
- quest bug always active on all act bosses (achieved by using the same drop table),
- greatly improved drop rates for runes,
- greatly improved drop rates for almost all PD2 exclusive items,
- improved drop rates for uniques/sets,
- improved roll chances for desired charm and jewel affixes (e.g. skillers, life, %elemental dmg),
- improved sell values on higher difficulties - they continue on increasing by 5k per act,
- new items: Exalted Orb (used to craft set items), Mythic Orb (used to craft unique items), Gheed's Curious Box (contains batch of pgems of random type), Eternal Coin (used in cubing recipes), Transient Coin (used in armour/weapon set/unique crafting), Fragment of Potential (qol recipes), Worldstone Sliver (downgrade item to magic), Dye (item dyeing),
- added safe unsocketting recipe (don't eat socketed items) - item + Ist + tp scroll,
- new unique grand charm: Cain's Wisdom (bonus to xp, req clvl 88),
- qol crafting recipes (craftable infusions, ppiece upgrading, corrupting pbox to demonic cube),
- map multiplication using scarabs (same restrictions as with lilith's mirror),
- qol shop at anya,
- changed launch splash, main menu, tcp/ip menu and character select screens to lod (delete ``data/global/ui`` to revert).

## Bugs / limitations
- when safe unsocketing, resulting runes and gems have quantity equal to 0; they function as normal items (can be socketed and give correct bonuses, can create runewords), but trying to stack them with others of the same type (including putting them back to the stash) eats them - bug with pd2 code, not this mod
