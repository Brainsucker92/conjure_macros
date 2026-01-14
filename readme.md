# Usage Guide for Conjure Spells

This guide explains how to use the conjure spells scripts provided in this repository. These scripts are written in Lua and are designed to be used with World of Warcraft's macro system.

## Files Description

- `conjure_drink.txt`: Contains a script for the Conjure Water spell. This script calculates the rank of the spell based on your character level, whether you hold down specific modifier keys (Alt and Shift), and whether you have a target or not. If no target is specified, it will cast the spell on yourself.
- `conjure_food.txt`: Contains a script for the Conjure Food spell. Similarly to `conjure_drink.txt`, this script calculates the rank of the spell based on your character level and whether you hold down specific modifier keys (Alt and Shift). It will cast the spell on your target if one is specified, or on yourself if no target is specified.
- `conjure_refreshment.txt`: Contains a script for the Conjure Refreshment spell. This spell has two ranks depending on your character level (1 for levels 1-74 and 2 for levels 80+). If you hold down the Shift key while using this macro, it will cast the lower rank spell; otherwise, it will cast the higher rank spell.
- `helpers.txt`: Contains helper functions used by the conjure scripts. The `GHSR` function is used to determine the highest rank of a given spell that your character can cast. The `GSNBR` function is used to generate the full name of a spell with its rank.
- `init.txt`: Initializes a secure action button that is used by the conjure scripts. This button is created if it doesn't exist already and is then configured to cast spells.

## Usage Instructions

1. Copy the contents of each script into a new macro in your World of Warcraft Macro interface. To do this, open the game's Interface > Macros panel, click "Create Macro", give it a name (e.g., "Conjure Water"), and paste the contents of `conjure_drink.txt` into the macro body. Repeat this step for each script.
2. When you use a macro in-game, it will cast the corresponding Conjure spell on your target or player based on certain conditions. For example, if you use the "Conjure Water" macro while holding down the Alt key and without having a target, it will cast the spell on yourself at its highest possible rank.