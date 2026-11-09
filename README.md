# AutoLoot

Pick up creature loot without opening a loot window. **AutoLoot** collects eligible loot for solo players as soon as they kill a creature, so they can get back to the adventure sooner.

## What it does

- Adds the creature's gold directly to the player's money.
- Puts loot items in the player's bags when there is room.
- Sends items by in-game mail when the bags cannot hold them.
- Keeps creature skinning available after the loot has been collected.
- Fires AzerothCore's `OnPlayerLootItem` hook for items stored in the player's bags.

## When AutoLoot runs

AutoLoot only handles creatures the player is allowed to loot. It skips players who are in a group, leaving normal group-loot rules in place. There is currently no configuration file or in-game toggle.

## Installation

1. Place this module in your AzerothCore `modules` directory. The folder should be named `mod-autoloot`.
2. Re-run CMake configuration for your AzerothCore build.
3. Build AzerothCore and start the worldserver.

For example, the module path should look like:

```text
azerothcore-wotlk/modules/mod-autoloot/
```

## Acknowledgment

This module is based on an older TrinityCore C++ script. The original author's name was not available when this module was published; attribution will be added if it becomes known.
