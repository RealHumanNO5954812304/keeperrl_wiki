---
title: Alpha21
permalink: Alpha21/
layout: wiki
---

Gameplay changes

`   New immigration system and UI, which lets the player accept or reject minions, and unifies immigration, recruitment, breeding, and imp spawning.`  
`   New campaign game mode with fixed keeper position and villains.`  
`   In games where the player has won, highscores are only based on the number of turns.`  
`   Old campaign mode renamed to “free play”. Highscores disabled for this mode.`  
`   The “your evilness” trigger replaced by one based on the number of conquered villains.`  
`   Added kraken enemy on keeper’s base map.`  
`   Removed some attack triggers from retired keepers to make them less aggressive.`  
`   Invisible friendly creatures are visible in creature control mode.`  
`   Only humanoids are allowed to be whipped.`  
`   Non-humanoids are not allowed to open chests and coffins.`  
`   “Escape” spell won’t teleport creature to an inaccessible area.`  
`   Minerals won’t spawn next to dug out tiles.`

UI changes

`   Female keepers and adventurers! Gender currently has no effect on gameplay.`  
`   Single map mode is available through the campaign setup window.`  
`   Smooth scrolling through lists. Fixed various scrolling issues.`  
`   New UI for firing ranged weapons using the mouse.`  
`   Added team go-to order by drag and dropping team from the minion menu onto the map.`  
`   Display a guard post sprite when minion is dropped onto the map to go somewhere.`  
`   Added “drop everything” command in creature control mode.`  
`   Added tooltips with item descriptions to workshop UI.`  
`   New interface for paying in shops both for individual items and in bulk.`  
`   Added information on item weight in creature control mode.`  
`   Fixed various glitches involving tooltips.`  
`   Lesser villains are highlighted yellow on campaign map.`  
`   Allowed rectangle selection when claiming tiles.`  
`   Won’t draw selection rectangle when active order or building doesn’t allow it.`  
`   Tweaked some inconsistent room names in the UI.`  
`   Some player messages have a higher priority color. Changed “critically wounded” status to “bleeding”.`

Bugfixes

`   Fixed a common compatibility issue with Intel Express and similar video cards due to lack of support of non-power-of-two texture sizes.`  
`   Fixed capturing of prisoners.`  
`   Fixed torturing of prisoners.`  
`   Fixed an issue with loading save files on some Linux systems.`  
`   Fixed a common crash caused by duplicate item ids due to a bug in RNG seeding.`  
`   Re-implemented minion equipment tracking, which fixes various issues and removes lag.`  
`   Fixed save file erasing so that an autosave and normal save can’t exist at the same time.`  
`   Fixed updating of creature effects and resistances when equipment is taken off.`  
`   Fixed hiding command.`  
`   Fixed furniture removal from claimed squares.`  
`   Fixed various issues with dungeon retirement.`  
`   Fixed visibility updating glitches in both real-time and turn-based modes.`  
`   Fixed various issues and crashes in the throwing UI in creature control mode.`  
`   Fixed issues with some characters in the message board text.`  
`   Fixed map scrolling glitch in creature control mode.`  
`   Fixed some glitches involving rectangle selection in real-time mode.`  
`   Prevented overflowing keyboard queue and game lock-up by holding space.`  
`   Fixed issues with clicking on minions on the map.`  
`   Fixed crash involving a creature getting killed right after traveling to another map.`  
`   Fixed a crash involving bandits not able to find gold (usually caused by a player using cheats).`

Other

`   Changed format of highscores file to binary.`  
`   Added versioning to highscores, so they can be cleared after major gameplay changes.`  
`   The “UI zoom” setting is not available at lower resolutions to prevent crashes.`  
`   Replaced “no fullscreen” option in Steam launcher with “clear settings”.`