# Team V10 Rank System Enhanced

Advanced rank/XP system for CS 1.6 with VIP/Admin multipliers, RGB HUD effects (Static/Rainbow/Pulse), spectator HUD, and persistent storage via nVault.

- **Game:** Counter-Strike 1.6 (AMX Mod X)
- **Version:** 1.0
- **Authors:** ZAKI (AAA DZ) & ITS_ZAKI ALM
- **Repository:** https://github.com/its-zaki-dz/Level-Plugin-Cs1.6-1.0V

## Features
- 50 Ranks with progressive XP requirements (up to 5,000,000 XP).
- XP rewards for kills, headshots, knife, grenade, bomb plant/defuse; teamkill penalty.
- VIP and Admin XP multipliers (VIP ×1.5, Admin ×2.0).
- RGB HUD with Static / Rainbow / Pulse modes.
- Spectator HUD follows the observed player.
- nVault saving by SteamID (robust to name changes).
- Auto-save every 5s, save on disconnect, manual save/load.
- Screen fade + sound feedback on level up/down.
- Debug tools for SteamID, flags, data state.

## Requirements
- **AMX Mod X:** 1.9+ recommended
- **Modules:** `amxmodx`, `amxmisc`, `cstrike`, `fakemeta`, `hamsandwich`, `nvault`
- **Include:** `colorchat.inc`
- **Sound:** Uses `XP/levelupcaster.wav`
  - Path: `cstrike/sound/XP/levelupcaster.wav`
  - You can change the sound via the defines in the source.

## Installation
1. Clone or download the repo.
2. Place `scripting/TeamV10_RankSystem_Enhanced.sma` into your AMXX `scripting` folder.
3. Ensure `colorchat.inc` is in `scripting/include/`.  
   - If you don’t have it, install the ColorChat include from AlliedModders.
4. Compile with AMXX Compiler (preferably the local 1.9+ compiler).
5. Copy the compiled `TeamV10_RankSystem_Enhanced.amxx` to `cstrike/addons/amxmodx/plugins/`.
6. Add this line to `configs/plugins.ini`:
