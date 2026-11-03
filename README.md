# Party Play Checker

Plugin source for POEFixer, built against SDK v6. It shows the horizontal world-coordinate distance to detected player entities, rounded to 0.1 m, and compares that distance with an adjustable threshold.

## Source

Download [PartyPlayChecker-source.zip](./PartyPlayChecker-source.zip) and extract it. The archive includes the Visual Studio solution, plugin project, source code, POEFixer SDK headers, ImGui sources, README, and license.

## Build

Open `PartyPlayChecker.sln` in Visual Studio 2022 with the C++ desktop workload, select `Release | x64`, and build. Copy `x64/Release/Plugins/PartyPlayChecker/PartyPlayChecker.dll` into `POEFixer/Plugins/PartyPlayChecker/`, then enable the plugin in POEFixer.

## Range note

The displayed distance is measured from player coordinates. The threshold is configurable and only reports whether another detected player is inside that chosen value. Public references do not establish one universal numeric party range for Path of Exile 2; the initial 13 m setting is an unverified reference carried over from Path of Exile 1's party loot range.
