---
title: CreatureIDs 6
permalink: CreatureIDs_6/
layout: wiki
---
=Usage=
Used to specify what keepers and adventurers appear in games and also what immigrants appear in games.

=Example from player_creatures.txt=
From: [[Player_Creatures.txt]]
 creatureId = { '''KEEPER_MAGE KEEPER_MAGE_F''' }

=Example from immigration.txt=
 ids = { '''IMP''' }

=Valid values=
*KEEPER_MAGE
*KEEPER_MAGE_F
*KEEPER_KNIGHT
*KEEPER_KNIGHT_F
*KEEPER_KNIGHT_WHITE
*KEEPER_KNIGHT_WHITE_F
*ADVENTURER
*ADVENTURER_F
*UNICORN
*BANDIT
*RAT_SOLDIER
*RAT_LADY
*RAT_KING
*GHOST
*SPIRIT
*LOST_SOUL
*SUCCUBUS
*DOPPLEGANGER
*WITCH
*WITCHMAN
*CYCLOPS
*DEMON_DWELLER
*DEMON_LORD
*MINOTAUR
*SOFT_MONSTER
*HYDRA
*SHELOB
*GREEN_DRAGON
*RED_DRAGON
*KNIGHT_PLAYER
*JESTER_PLAYER
*ARCHER_PLAYER
*PRIEST_PLAYER
*GNOME_PLAYER
*PESEANT_PLAYER
*KNIGHT
*JESTER
*DUKE
*ARCHER
*PRIEST
*WARRIOR
*SHAMAN
*PESEANT
*CHILD
*SPIDER_FOOD
*PESEANT_PRISONER
*HALLOWEEN_KID
*CLAY_GOLEM
*STONE_GOLEM
*IRON_GOLEM
*LAVA_GOLEM
*ADA_GOLEM
*AUTOMATON
*ZOMBIE
*SKELETON
*VAMPIRE
*VAMPIRE_LORD
*MUMMY
*ORC
*ORC_SHAMAN
*HARPY
*KOBOLD
*GNOME
*GNOME_CHIEF
*GOBLIN
*IMP
*OGRE
*CHICKEN
*DWARF
*DWARF_FEMALE
*DWARF_BARON
*LIZARDMAN
*LIZARDLORD
*ELF
*ELF_ARCHER
*ELF_CHILD
*ELF_LORD
*DARK_ELF
*DARK_ELF_WARRIOR
*DARK_ELF_CHILD
*DARK_ELF_LORD
*DRIAD
*HORSE
*COW
*DONKEY
*PIG
*GOAT
*JACKAL
*DEER
*BOAR
*FOX
*CAVE_BEAR
*RAT
*SPIDER
*FLY
*ANT_WORKER
*ANT_SOLDIER
*ANT_QUEEN
*SNAKE
*RAVEN
*VULTURE
*WOLF
*WEREWOLF
*DOG
*FIRE_SPHERE
*ELEMENTALIST
*FIRE_ELEMENTAL
*WATER_ELEMENTAL
*EARTH_ELEMENTAL
*AIR_ELEMENTAL
*ENT
*ANGEL
*BAT
*DEATH
*SHOPKEEPER

As of Alpha 27, the below CreatureIds are not present in the creatures.txt, but readable by the game engine. They are still present and utilized in the immigration.txt file. 

*SPECIAL_BLBN
*SPECIAL_BLBW
*SPECIAL_BLGN
*SPECIAL_BLGW
*SPECIAL_BMBN
*SPECIAL_BMBW
*SPECIAL_BMGN
*SPECIAL_BMGW
*SPECIAL_HLBN
*SPECIAL_HLBW
*SPECIAL_HLGN
*SPECIAL_HLGW
*SPECIAL_HMBN
*SPECIAL_HMBW
*SPECIAL_HMGN
*SPECIAL_HMGW

Special note is taken to point out the below Ids are not present in either files (Alpha27), but still present and reachable in most games. This is either due to in-game generation done by the engine, or some unknown means.

*KRAKEN
*SOKOBAN_BOULDER

Lastly, the below Id is again not found in either file (Alpha27). For game purposes, the practice of putting _PLAYER at the end of the Id is for immigration. This allows a player to recruit a minion while also encountering the creature during adventures (or invasions). Note, that any name will do, as long as the viewId is valid.

*DUKE_PLAYER

[[Category: Modding Reference Data]]

[MainPage](/keeperrl_wiki/ "wikilink")>>[Old_Wiki](/keeperrl_wiki/Old_Wiki "wikilink")>>[Old_CreatureIDs](/keeperrl_wiki/Old_CreatureIDs "wikilink")

Other items in this section
-    [CreatureIDs 0](/keeperrl_wiki/CreatureIDs_0 "wikilink")
-    [CreatureIDs 1](/keeperrl_wiki/CreatureIDs_1 "wikilink")
-    [CreatureIDs 2](/keeperrl_wiki/CreatureIDs_2 "wikilink")
-    [CreatureIDs 3](/keeperrl_wiki/CreatureIDs_3 "wikilink")
-    [CreatureIDs 4](/keeperrl_wiki/CreatureIDs_4 "wikilink")
-    [CreatureIDs 5](/keeperrl_wiki/CreatureIDs_5 "wikilink")