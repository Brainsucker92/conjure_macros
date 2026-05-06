# Usage Guide for Conjure Spells

This guide explains how to use the conjure spells scripts provided in this repository. These scripts are written in Lua and are designed to be used with World of Warcraft's macro system.

## Key Features and Advantages

These macros offer significant improvements over traditional spellcasting methods:

1. **Dynamic Rank Calculation**  
   Automatically selects the optimal spell rank based on your character level, ensuring you always use the most powerful available version of the spell.

2. **Smart Targeting**  
   - Casts on your target if selected  
   - Falls back to self-casting if no target is present  

3. **Modifier Key Customization**  
   - **Alt** key: Forces self-casting even with a target selected  
   - **Shift** key: Increases spell potency by 1 rank (where applicable)  
   - Enables fine-grained control over spell effects

4. **Secure Action Button**  
   Uses WoW's secure action button framework for proper UI integration and compatibility with game mechanics.

## Files Description

- `conjure_drink.txt`:  
  Conjure Water spell with dynamic rank calculation based on level, modifiers, and targeting state.

- `conjure_food.txt`:  
  Conjure Food spell with similar dynamic behavior and modifier-based adjustments.

- `conjure_refreshment.txt`:  
  Conjure Refreshment spell with automatic rank selection (Rank 1 for levels 1-79, Rank 2 for level 80+).

- `helpers.txt`:  
  **Mandatory dependency** for all macros. Contains reusable functions for spell rank detection and formatting.

- `init.txt`:  
  **Mandatory dependency** for all macros. Sets up a secure action button framework used by all macros.

## Usage Instructions

1. **First**, create macros in-game for `helpers.txt` and `init.txt` — these are required for any conjure macro to function.
2. Then, create macros for each conjure spell (`conjure_drink.txt`, `conjure_food.txt`, `conjure_refreshment.txt`).
3. Use the macros **outside of combat** with the following controls:
   - Left-click: Cast on target (or self if no target)
   - Hold Alt: Force self-casting
   - Hold Shift: Increase spell potency by 1 rank (where applicable)

> **Important Note:** These macros are **not compatible with combat scenarios** and will not function while in combat. They are designed for use in safe zones, auction houses, or other non-combat situations.

## How to Contribute

If you find these macros helpful, please consider donating to support continued development and maintenance:

### Crypto

[**bitcoin**](bitcoin:BC1QUT9WDUGUNSHYWDQF7DXMF73AR2EAFSR2HWSPEJ?label=WoW%20Conjure%20Macros&message=Thank%20you%20so%20much%20for%20your%20contribution%21): bc1qut9wdugunshywdqf7dxmf73ar2eafsr2hwspej

All donations are appreciated and help keep these tools free for the community!

