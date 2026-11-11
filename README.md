MOD: Finals Week - up to 8 players
==================================

Raises the multiplayer room limit from 4 to 8 players.

Mod version: 1.0
Made for the game build from November 5, 2026.


HOW TO INSTALL
1. On Steam, right-click "Finals Week: Descolado"
   > Manage > Browse local files.
2. Open the folder: CopyGirls\Content\Paks
3. Copy the file "CopyGirls-Windows_MorePlayers_P.pak" into this folder
   (next to CopyGirls-Windows.pak). DO NOT delete or replace anything.
4. Open the game normally.


HOW TO REMOVE
Delete the file CopyGirls-Windows_MorePlayers_P.pak from that folder.
The game goes back to normal right away.


WHAT THE MOD CHANGES
The 4-player limit is a fixed number used when the game creates the
multiplayer room (in the game's BP_GameInstance blueprint). The mod
changes that one number from 4 to 8. Nothing else is changed.

The mod contains a single game file (BP_GameInstance). It is identical
to the original except for 1 byte (4 -> 8). Unreal Engine loads
"_P.pak" files on top of the original game files. Your original game
files are never modified.

The lobby lists, player list and results board build one row per
connected player, so they should show every player.


IS IT SAFE?
- A .pak file is not a program. Windows cannot run it. Only the game
  reads it, like a data archive.
- The mod adds no new behavior. It is the game's own logic with one
  number changed.
- Removing the file fully undoes the mod.

Only download this mod from the original source. To make sure your
file has not been tampered with, check its SHA-256 hash.
In PowerShell, run:

    Get-FileHash .\CopyGirls-Windows_MorePlayers_P.pak

It must be exactly:

    051FEF174FF9113B279483E24E09D34423C18AC586FC2E43FD30D3B6E107DFA1

If the hash is different, delete the file.


NOTES
- The person who creates the room (host) MUST have the mod.
  It is recommended that everyone has it.
- Not yet tested with more than 4 players. Possible issues:
  * Exam rooms may not have enough chairs for everyone. Extra players
    may end up standing or stuck.
  * With many players, names on boards and lists may look cramped or
    get cut off at the edges. This is visual only.
- If the game updates and something breaks, remove the mod and wait
  for an updated version.
- This is an unofficial fan mod. It is not made or supported by the
  game's developers. Please don't report bugs to them while using it.
