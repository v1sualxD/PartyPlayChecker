# Party Play Checker

POEFixer plugin source (SDK v6). It measures horizontal distance to nearby player entities and compares it with a configurable threshold.

## Features

- Draws a range circle around your character. It turns green when the selected minimum number of players (1-5) is in range, and red otherwise.
- Shows a draggable window with player distances and `IN ZONE` / `OUT OF ZONE` status.
- Optional entry and exit sound alerts.
- Named configuration profiles that can be saved and loaded.
- Optional performance debug window with average and peak update time, entity scan time, and entity/player counts.
- Optional map-only display mode that hides the range UI in towns and hideouts.
- Optional `PARTY PLAY` preset at 13 m. This value is provisional for PoE 2.

## Source

Download [PartyPlayChecker-source-v0.1.2.zip](./PartyPlayChecker-source-v0.1.2.zip) and extract it. It contains the Visual Studio solution, plugin source, POEFixer SDK headers, ImGui sources, README, and license.

## Build

Open `PartyPlayChecker.sln` in Visual Studio 2022 with the C++ desktop workload, select `Release | x64`, and build. The output is `x64/Release/Plugins/PartyPlayChecker/PartyPlayChecker.dll`.

## Range accuracy

Distances use horizontal player world coordinates and are rounded to 0.1 m. Public PoE 2 references do not confirm one universal numeric party range for XP and loot. The 13 m preset is an unverified reference from Path of Exile 1's party loot range. The plugin reports detected player positions and does not expose actual party membership or reward eligibility.
