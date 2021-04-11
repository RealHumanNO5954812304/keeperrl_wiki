---
title: Build Menu.txt 0
permalink: Build_Menu.txt_0/
layout: wiki
---
 # &quot;structure&quot;, &quot;doors&quot;, etc are groups that are then used in the last column in player_creatures.txt.
 # (they do not necessarily correspond to how menu items are grouped into submenus, you can join several
 # groups into a submenu, like beds, cages, pigsty and coffins are in the &quot;living&quot; submenu)

 {
   &quot;structure&quot;
   {
  { Dig                                                      &quot;Dig or cut tree&quot;   &quot;Structure&quot;  
    &quot;&quot; d {} true DIG_OR_CUT_TREES}
  { Furniture {{ MOUNTAIN }                   STONE 5 }      &quot;Soft rock&quot;         &quot;Structure&quot; }
  { Furniture {{ MOUNTAIN2 }                  STONE 10 }     &quot;Hard rock&quot;         &quot;Structure&quot; }

  { Furniture {{ DUNGEON_WALL DUNGEON_WALL2 } STONE 3}       &quot;Reinforce wall&quot;    &quot;Structure&quot;
    &quot;Reinforced walls are better at stopping enemies from digging into your dungeon.&quot;}

  { Furniture {{ PIT }                        STONE 0 }      &quot;Dig a pit&quot;         &quot;Structure&quot;
    &quot;Dig a pit in the ground. Building next to water or lava will cause it to fill up.&quot; }

  { Furniture {{ WOOD_WALL }                  WOOD 5 }       &quot;Wooden building&quot;   &quot;Structure&quot;
    &quot;Outdoor building. Tiles covered by the roof are considered territory and can be built on.&quot; }

  { Furniture {{ CASTLE_WALL }                STONE 5 }      &quot;Stone building&quot;    &quot;Structure&quot;
    &quot;Outdoor building. Tiles covered by the roof are considered territory and can be built on.&quot; }

  { Furniture {{ BRIDGE }                     WOOD 5 }       &quot;Bridge&quot;            &quot;Structure&quot;
    &quot;Build to pass over water of lava.&quot; }
   }

   &quot;doors&quot;
   {
  { Furniture {{ WOOD_DOOR }                  WOOD 5 }       &quot;Wooden door&quot;       &quot;Doors&quot;
    &quot;Stops enemies. Your minions can pass freely unless you lock it.&quot;  o {} true BUILD_DOOR}

  { Furniture {{ IRON_DOOR }                  IRON 5 }       &quot;Iron door&quot;         &quot;Doors&quot;
    &quot;Stops enemies. Your minions can pass freely unless you lock it.&quot; }

  { Furniture {{ ADA_DOOR }                   ADA 5 }        &quot;Adamantine door&quot;   &quot;Doors&quot;
    &quot;Stops enemies. Your minions can pass freely unless you lock it.&quot;}
   }

   &quot;floors&quot;
   {
  { Furniture {{ FLOOR_WOOD1 }                WOOD 2 }       &quot;Wooden&quot;            &quot;Floors&quot;
   &quot;&quot; f {} true BUILD_FLOOR}
  { Furniture {{ FLOOR_WOOD2 }                WOOD 2 }       &quot;Wooden&quot;            &quot;Floors&quot;
   &quot;&quot; 0 {} true BUILD_FLOOR}
  { Furniture {{ FLOOR_STONE1 }               STONE 2 }      &quot;Stone&quot;             &quot;Floors&quot; }
  { Furniture {{ FLOOR_STONE2 }               STONE 2 }      &quot;Stone&quot;             &quot;Floors&quot; }
  { Furniture {{ FLOOR_CARPET1 }              GOLD 2 }       &quot;Carpet&quot;            &quot;Floors&quot; }
  { Furniture {{ FLOOR_CARPET2 }              GOLD 2 }       &quot;Carpet&quot;            &quot;Floors&quot; }
  { DestroyLayers {FLOOR}                                    &quot;Remove floor&quot;      &quot;Floors&quot; }
   }
   
   &quot;storage&quot;
   {
  { Zone STORAGE_RESOURCES                                   &quot;Resources&quot;         &quot;Storage&quot; 
   &quot;Only wood, iron, granite, and adamantium can be stored here.&quot; s {} true RESOURCE_STORAGE}

  { Zone STORAGE_EQUIPMENT                                   &quot;Equipment&quot;         &quot;Storage&quot;
   &quot;All equipment for your minions can be stored here.&quot; 0 {} false EQUIPMENT_STORAGE }

  { Furniture {{ TREASURE_CHEST }             WOOD 5  }      &quot;Treasure chest&quot;    &quot;Storage&quot;
   &quot;All your gold is stored here.&quot; }

  { Furniture {{ GRAVE }                      STONE 5 }      &quot;Grave&quot;             &quot;Storage&quot;
   &quot;All corpses are stored here.&quot;}
   }

   &quot;quarters&quot;
   {
  { Zone QUARTERS1                                           &quot;Quarters 1&quot;        &quot;Quarters&quot;
   &quot;Designate separate quarters for chosen minions.&quot; q {} true}

  { Zone QUARTERS2                                           &quot;Quarters 2&quot;        &quot;Quarters&quot;
   &quot;Designate separate quarters for chosen minions.&quot;}

  { Zone QUARTERS3                                           &quot;Quarters 3&quot;        &quot;Quarters&quot;
   &quot;Designate separate quarters for chosen minions.&quot;}
   }

   &quot;library&quot;
   {
  { Furniture {{ BOOKCASE_WOOD }   WOOD 15 }                 &quot;Wooden bookcase&quot;   &quot;Library&quot;  
   &quot;Train your minions' magical powers here.&quot; y          {TechId &quot;sorcery&quot;} true BUILD_LIBRARY }
  
  { Furniture {{ BOOKCASE_IRON }   IRON 15 }                 &quot;Iron bookcase&quot;     &quot;Library&quot;
   &quot;Train your minions' magical powers here.&quot; 0          {TechId &quot;advanced sorcery&quot;} }
  
  { Furniture {{ BOOKCASE_GOLD }   GOLD 15 }                 &quot;Golden bookcase&quot;   &quot;Library&quot;
   &quot;Train your minions' magical powers here.&quot;0           {TechId &quot;master sorcery&quot;}}
   }
  
   &quot;throne&quot;
   {
  { Furniture { types = { THRONE } cost = GOLD 500 limit = 1} &quot;Throne&quot; &quot;&quot; &quot;&quot;  0   {DungeonLevel 10} }
   }
  
   &quot;beds&quot;
   {
  { Furniture {{ BED1 }       WOOD 12 }                      &quot;Basic bed&quot;         &quot;Living&quot;
   &quot;Humanoid minions sleep here.&quot; v {} true  BUILD_BED }
  
  { Furniture {{ BED2 }       IRON 12 }                      &quot;Fine bed&quot;          &quot;Living&quot;
   &quot;Humanoid minions sleep here.&quot; }

  { Furniture {{ BED3 }       GOLD 12 }                      &quot;Luxurious bed&quot;     &quot;Living&quot;
   &quot;Humanoid minions sleep here.&quot;}
   }

   &quot;beast_cage&quot;
   {
  { Furniture {{ BEAST_CAGE } WOOD 8 }                       &quot;Beast cage&quot;        &quot;Living&quot;
   &quot;Beasts sleep here.&quot;}
   }
    
   &quot;pigsty&quot;
   {
  { Furniture {{ PIGSTY }     WOOD 5 }                       &quot;Pigsty&quot;            &quot;Living&quot;}
   }

   &quot;coffins&quot;
   {
  { Furniture {{ COFFIN1 }    WOOD 15 }                      &quot;Basic coffin&quot;      &quot;Living&quot;
   &quot;Undead creatures sleep here.&quot;}

  { Furniture {{ COFFIN2 }    STONE 15 }                     &quot;Fine coffin&quot;       &quot;Living&quot;
   &quot;Undead creatures sleep here.&quot;}

  { Furniture {{ COFFIN3 }    GOLD 15 }                      &quot;Luxurious coffin&quot;  &quot;Living&quot;
   &quot;Undead creatures sleep here.&quot;}
   }


   &quot;training&quot;
   {
  { Furniture {{ TRAINING_WOOD } WOOD 12 }                   &quot;Wooden dummy&quot;      &quot;Training room&quot;
   &quot;Train your minions' melee skills here.&quot; r {} true  TRAINING_ROOM}

  { Furniture {{ TRAINING_IRON } IRON 12 }                   &quot;Iron dummy&quot;        &quot;Training room&quot;
   &quot;Train your minions' melee skills here.&quot;   0 { TechId &quot;iron working&quot; } }

  { Furniture {{ TRAINING_ADA }  ADA  12 }                   &quot;Adamantine dummy&quot;  &quot;Training room&quot;
   &quot;Train your minions' melee skills here.&quot;   0 { TechId &quot;iron working&quot; }}

  { Furniture {{ ARCHERY_RANGE } WOOD 12 }                   &quot;Archery target&quot;    &quot;Training room&quot;
   &quot;Train your minions' archery skills here.&quot; 0 { TechId &quot;archery&quot; }}
   }

   &quot;crafting&quot;
   {
  { Furniture {{ WORKSHOP }   WOOD 15 }                      &quot;Workshop&quot;          &quot;Crafting&quot;
   &quot;Produces leather equipment, traps, first-aid kits and other.&quot; m {} true  BUILD_WORKSHOP}

  { Furniture {{ FORGE }      IRON 20 }                      &quot;Forge&quot;             &quot;Crafting&quot;
   &quot;Produces metal weapons and armor.&quot;    0 { TechId &quot;iron working&quot; }}

  { Furniture {{ LABORATORY } STONE 10 }                     &quot;Laboratory&quot;        &quot;Crafting&quot;
   &quot;Produces magical potions.&quot;            0 { TechId &quot;alchemy&quot; }}

  { Furniture {{ JEWELLER }   WOOD 12 }                      &quot;Jeweller&quot;          &quot;Crafting&quot;
   &quot;Produces magical rings and amulets.&quot;  0 { TechId &quot;jewellery&quot; }}
   }

   &quot;demon_shrine&quot;
   {
  { Furniture {{ DEMON_SHRINE } GOLD 30 }                    &quot;Demon shrine&quot;      &quot;&quot;
   &quot;Undead creatures sleep here.&quot; 0 { TechId &quot;demonology&quot; }}
   }

   &quot;prison&quot;
   {
  { Furniture {{ PRISON }        IRON 15 }                   &quot;Prison&quot;            &quot;Prison&quot;
   &quot;Required to capture enemies.&quot; p {} true}

  { Furniture {{ TORTURE_TABLE } IRON 15 }                   &quot;Torture table&quot;     &quot;Prison&quot;
   &quot;Can be used to torture prisoners. Free population slot required for torturing.&quot;}
   }


   &quot;orders&quot;
   {
  { ClaimTile                                                &quot;Claim tile&quot;        &quot;Orders&quot;
   &quot;Claim a dungeon tile as your own. Building anything on it has the same effect.&quot; }

  { Zone FETCH_ITEMS                                         &quot;Fetch items&quot;       &quot;Orders&quot;
   &quot;Order imps to fetch items from locations outside the dungeon. This is a one-time order.&quot;}

  { Zone PERMANENT_FETCH_ITEMS                               &quot;Fetch items persistently&quot; &quot;Orders&quot;
   &quot;Order imps to fetch items from locations outside the dungeon. This is a persistent order.&quot;}

  { Dispatch                                                 &quot;Prioritize task&quot;   &quot;Orders&quot;
   &quot;Click on an existing task to give it a high priority.&quot; a }

  { DestroyLayers {CEILING MIDDLE}                           &quot;Remove construction&quot; &quot;Orders&quot;
   &quot;&quot; e {} false REMOVE_CONSTRUCTION }
  
  { ForbidZone                                               &quot;Forbind zone&quot;      &quot;Orders&quot;
   &quot;Mark tiles to keep minions from entering.&quot;}
   }

   &quot;installations&quot;
   {
  { Furniture {{ BARRICADE }     WOOD 5 }                    &quot;Barricade&quot;         &quot;Installations&quot;
   &quot;Blocks enemy movement, but projectiles and spells can pass over it.&quot; }

  { Furniture {{ TORCH_N TORCH_E TORCH_S TORCH_W }}          &quot;Torch&quot;             &quot;Installations&quot;
   &quot;Place it on tiles next to a wall.&quot; c {} false BUILD_TORCH}

  { Furniture {{ CANDELABRUM_N CANDELABRUM_E CANDELABRUM_S CANDELABRUM_W } GOLD 5 }
   &quot;Candelabrum&quot;             &quot;Installations&quot;       &quot;Place it on tiles next to a wall.&quot; }

  { Furniture {{ GROUND_TORCH }  WOOD 10  }                  &quot;Standing torch&quot;    &quot;Installations&quot;
   &quot;&quot; 0 {} false BUILD_TORCH }

  { Furniture {{ KEEPER_BOARD }  WOOD 15 }                   &quot;Message board&quot;     &quot;Installations&quot;
   &quot;A board where you can leave a message for other players.&quot; }

  { Furniture {{ FOUNTAIN }      STONE 30 }                  &quot;Fountain&quot;          &quot;Installations&quot; }

  { Furniture {{ WHIPPING_POST } WOOD  20 }                  &quot;Whipping post&quot;     &quot;Installations&quot;
   &quot;A place to whip your minions if they need a morale boost.&quot; }

  { Furniture {{ GALLOWS }       WOOD  20 }                  &quot;Gallows&quot;           &quot;Installations&quot;
   &quot;For hanging prisoners.&quot;}

  { Furniture {{ IMPALED_HEAD }  PRISONER_HEAD 1 true}       &quot;Prisoner head&quot;     &quot;Installations&quot;
   &quot;Impaled head of an executed prisoner. Aggravates enemies.&quot;}
   }

   &quot;magical_installations&quot;
   {
  { Furniture {{ EYEBALL }              WOOD   30 }                   &quot;Eyeball&quot;           &quot;Installations&quot;
   &quot;Makes the area around it visible.&quot;}

  { Furniture {{ MINION_STATUE }        GOLD   50  }                  &quot;Golden statue&quot;     &quot;Installations&quot; &quot;&quot;}
  { Furniture {{ STONE_MINION_STATUE }  STONE  250 }                  &quot;Stone statue&quot;      &quot;Installations&quot; &quot;&quot;}
  { Furniture {{ PORTAL }               STONE  60 }                   &quot;Portal&quot;            &quot;Installations&quot;
   &quot;Opens a connection if another portal is present.&quot;}
   }

   &quot;tutorial&quot;
   {
  { Furniture {{ TUTORIAL_ENTRANCE } }                  &quot;Tutorial Entrance&quot;           &quot;Installations&quot;}
   }


   &quot;traps&quot;
   {
  { Trap TERROR TERROR_TRAP                                  &quot;Terror trap&quot;       &quot;Traps&quot;
   &quot;Causes the trespasser to panic.&quot; 0                   { TechId &quot;traps&quot; }}

  { Trap POISON_GAS GAS_TRAP                                 &quot;Gas trap&quot;          &quot;Traps&quot;
   &quot;Releases a cloud of poisonous gas.&quot; 0                { TechId &quot;traps&quot; }}

  { Trap ALARM ALARM_TRAP                                    &quot;Alarm trap&quot;        &quot;Traps&quot;
   &quot;Summons all minions&quot; 0                               { TechId &quot;traps&quot; }}

  { Trap WEB WEB_TRAP                                        &quot;Web trap&quot;          &quot;Traps&quot;
   &quot;Immobilises the trespasser for some time.&quot; 0         { TechId &quot;traps&quot; }}

  { Trap BOULDER BOULDER                                     &quot;Boulder trap&quot;      &quot;Traps&quot;
   &quot;Causes a huge boulder to roll towards the enemy.&quot; 0  { TechId &quot;traps&quot; }}

  { Trap SURPRISE SURPRISE_TRAP                              &quot;Surprise trap&quot;     &quot;Traps&quot;
   &quot;Teleports nearby minions to deal with the trespasser.&quot; 0 { TechId &quot;traps&quot; }}
   }
 }

[MainPage](/keeperrl_wiki/ "wikilink")>>[Old_Wiki](/keeperrl_wiki/Old_Wiki "wikilink")>>[Old_Build_Menu.txt](/keeperrl_wiki/Old_Build_Menu.txt "wikilink")

Other items in this section
-    [Build Menu.txt 1](/keeperrl_wiki/Build_Menu.txt_1 "wikilink")
-    [Build Menu.txt 2](/keeperrl_wiki/Build_Menu.txt_2 "wikilink")
-    [Build Menu.txt 3](/keeperrl_wiki/Build_Menu.txt_3 "wikilink")