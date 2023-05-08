# Comparing `tmp/pmdsky_debug_py-5.1.8-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-5.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 773347 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Apr-01 04:25 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Apr-01 04:25 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   712779 b- defN 23-Apr-01 04:25 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   680684 b- defN 23-Apr-01 04:25 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   701749 b- defN 23-Apr-01 04:25 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   680684 b- defN 23-Apr-01 04:25 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   718907 b- defN 23-Apr-01 04:25 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   680695 b- defN 23-Apr-01 04:25 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   227398 b- defN 23-Apr-01 04:25 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-01 04:25 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Apr-01 04:25 pmdsky_debug_py-5.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 04:25 pmdsky_debug_py-5.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-01 04:25 pmdsky_debug_py-5.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Apr-01 04:25 pmdsky_debug_py-5.1.8.dist-info/RECORD
-14 files, 4407340 bytes uncompressed, 771449 bytes compressed:  82.5%
+Zip file size: 784105 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Apr-03 04:25 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Apr-03 04:25 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   720789 b- defN 23-Apr-03 04:25 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   688659 b- defN 23-Apr-03 04:25 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   709748 b- defN 23-Apr-03 04:25 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   688659 b- defN 23-Apr-03 04:25 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   727240 b- defN 23-Apr-03 04:25 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   688670 b- defN 23-Apr-03 04:25 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   229717 b- defN 23-Apr-03 04:25 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:25 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/RECORD
+14 files, 4457926 bytes uncompressed, 782207 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.8.dist-info/METADATA
+Filename: pmdsky_debug_py-5.1.9.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.8.dist-info/WHEEL
+Filename: pmdsky_debug_py-5.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.8.dist-info/top_level.txt
+Filename: pmdsky_debug_py-5.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.8.dist-info/RECORD
+Filename: pmdsky_debug_py-5.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.5.1+36b947cb66"
+RELEASE = "v0.5.1+f276906247"
```

## pmdsky_debug_py/eu.py

```diff
@@ -12086,14 +12086,20 @@
         "The chance of Steel Wing boosting defense, as a percentage (20%).",
     )
 
     GOLD_THORN_POWER = Symbol(
         [0x7A68], [0x22C4E28], 0x2, "Attack power for Golden Thorns."
     )
 
+    BURN_DAMAGE = Symbol(None, None, None, "Damage dealt by the burn status condition.")
+
+    POISON_DAMAGE = Symbol(
+        None, None, None, "Damage dealt by the poison status condition."
+    )
+
     SPAWN_COOLDOWN = Symbol(
         [0x7A74],
         [0x22C4E34],
         0x2,
         "The number of turns between enemy spawns under normal conditions.",
     )
 
@@ -12257,14 +12263,28 @@
         ),
     )
 
     SONICBOOM_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by SonicBoom (20)."
     )
 
+    RAIN_ABILITY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is rain for the"
+            " abilities rain dish and dry skin."
+        ),
+    )
+
+    LEECH_SEED_HP_DRAIN = Symbol(
+        None, None, None, "The amount of health drained by leech seed status."
+    )
+
     EXCLUSIVE_ITEM_EXP_BOOST = Symbol(
         [0x7B24],
         [0x22C4EE4],
         0x2,
         "The percentage increase in experience from exp-boosting exclusive items.",
     )
 
@@ -12341,14 +12361,24 @@
 
     STICK_POWER = Symbol([0x7BBC], [0x22C4F7C], 0x2, "Attack power for Sticks.")
 
     BUBBLE_LOWER_SPEED_CHANCE = Symbol(
         None, None, None, "The chance of Bubble lowering speed, as a percentage (10%)."
     )
 
+    ICE_BODY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        0x2,
+        (
+            "The passive bonus health regen given when the weather is hail for the"
+            " ability ice body."
+        ),
+    )
+
     POWDER_SNOW_FREEZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Powder Snow (and others, see DoMoveDamageFreeze15) freezing,"
             " as a percentage (15%)."
@@ -12375,14 +12405,24 @@
         ),
     )
 
     POISON_FANG_POISON_CHANCE = Symbol(
         None, None, None, "The chance of Poison Fang poisoning, as a percentage (30%)."
     )
 
+    WEATHER_MOVE_TURN_COUNT = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The number of turns the moves rain dance, hail, sandstorm, sunny day and"
+            " defog change the weather for. (3000)"
+        ),
+    )
+
     THUNDER_PARALYZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Thunder (and others, see DoMoveDamageParalyze20) paralyzing,"
             " as a percentage (20%)"
@@ -12501,14 +12541,18 @@
         ),
     )
 
     POISON_DAMAGE_COOLDOWN = Symbol(
         [0x7C40], [0x22C5000], 0x2, "The number of turns between passive poison damage."
     )
 
+    LEECH_SEED_DAMAGE_COOLDOWN = Symbol(
+        None, None, None, "The number of turns between leech seed health drain."
+    )
+
     GEO_PEBBLE_DAMAGE = Symbol(
         [0x7C4C], [0x22C500C], 0x2, "Damage dealt by Geo Pebbles."
     )
 
     GRAVELEROCK_DAMAGE = Symbol(
         [0x7C50], [0x22C5010], 0x2, "Damage dealt by Gravelerocks."
     )
@@ -12544,14 +12588,18 @@
     CALCIUM_STAT_BOOST = Symbol(
         [0x7C64],
         [0x22C5024],
         0x2,
         "The permanent special attack boost from ingesting a Calcium.",
     )
 
+    WISH_BONUS_REGEN = Symbol(
+        None, None, None, "The passive bonus regen given by the wish status condition."
+    )
+
     DRAGON_RAGE_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by Dragon Rage (30)."
     )
 
     CORSOLA_TWIG_POWER = Symbol(
         [0x7C70], [0x22C5030], 0x2, "Attack power for Corsola Twigs."
     )
@@ -13095,14 +13143,25 @@
         (
             "Maps each weather type (by index, see enum weather_id) to the"
             " corresponding Castform type and form.\n\ntype: struct"
             " castform_weather_attributes[8]"
         ),
     )
 
+    BAD_POISON_DAMAGE_TABLE = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Table for how much damage each tick of badly poisoned should deal. The"
+            " table is filled with 0x0006, but could use different values for each"
+            " entry."
+        ),
+    )
+
     TYPE_MATCHUP_COMBINATOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "Table of type matchup combinations.\n\nEach row corresponds to a single"
             " type matchup that results from combining two individual type matchups"
@@ -16688,14 +16747,53 @@
         (
             "A convenience wrapper around SpawnTrap and BindTrapToTile. Always passes 0"
             " for the team parameter (making it an enemy trap).\n\nr0: trap ID\nr1: x"
             " position\nr2: y position\nr3: flags\nstack[0]: visibility flag"
         ),
     )
 
+    PrepareTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Saves the relevant information in the dungeon struct to later place a trap"
+            " at the\nlocation of the entity. (Only called with trap ID 0x19"
+            " (TRAP_NONE), but could be used \nwith others).\n\nr0: entity pointer\nr1:"
+            " trap ID\nr2: team (see struct trap::team)"
+        ),
+    )
+
+    TrySpawnTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the a trap can be placed on the tile. If the trap ID is >="
+            " TRAP_NONE (the\nlast value for a trap), randomly select another trap"
+            " (except for wonder tile). After\n30 failed attempts to select a"
+            " non-wonder tile trap ID, default to chestnut trap.\nIf the checks pass,"
+            " spawn the trap.\n\nr0: position\nr1: trap ID\nr2: team (see struct"
+            " trap::team)\nr3: visibility flag\nreturn: true if a trap was spawned"
+            " succesfully"
+        ),
+    )
+
+    TrySpawnTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the flag for a trapper trap is set, handles spawning a trap based upon"
+            " the\ninformation inside the dungeon struct. Uses the entity for logging a"
+            " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
+            " true if a trap was spawned succesfully"
+        ),
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x138A0],
         [0x22F0420],
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16934,14 +17032,25 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: target entity"
             " pointer\nr1: current_id\nreturn: ?"
         ),
     )
 
+    TryActivateTraceAndColorChange = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to activate the abilities trace and color change if possible. Called"
+            " after using\na move.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer\nr2: move pointer"
+        ),
+    )
+
     DefenderAbilityIsActive = Symbol(
         [0x1D558, 0x258B8, 0x2E834, 0x35A74, 0x46C4C, 0x568CC],
         [0x22FA0D8, 0x2302438, 0x230B3B4, 0x23125F4, 0x23237CC, 0x233344C],
         None,
         (
             "Checks if a defender has an active ability that isn't disabled by an"
             " attacker's Mold Breaker.\n\nThere are two versions of this function,"
@@ -16979,14 +17088,25 @@
         None,
         (
             "Checks if an entity is a monster (entity type 1).\n\nr0: entity"
             " pointer\nreturn: bool"
         ),
     )
 
+    TryActivateConversion2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks for the conversion2 status and applies the type change if"
+            " applicable. Called\nafter using a move.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr2: move pointer"
+        ),
+    )
+
     TryActivateTruant = Symbol(
         [0x1D67C],
         [0x22FA1FC],
         None,
         (
             "Checks if an entity has the ability Truant, and if so tries to apply the"
             " pause status to it.\n\nr0: pointer to entity"
@@ -18280,14 +18400,24 @@
             " spawn cooldown, it will try to spawn an enemy if the number of enemies is"
             " below the spawn cap.\n\nIf the spawn counter is greater than 900, it will"
             " instead perform the special spawn caused by the ability Illuminate.\n\nNo"
             " params."
         ),
     )
 
+    TryNonLeaderItemPickUp = Symbol(
+        [0x33058],
+        [0x230FBD8],
+        None,
+        (
+            "Similar to TryLeaderItemPickUp, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: entity pointer"
+        ),
+    )
+
     AuraBowIsActive = Symbol(
         [0x335BC],
         [0x231013C],
         None,
         (
             "Checks if a monster is holding an aura bow that isn't disabled by"
             " Klutz.\n\nr0: entity pointer\nreturn: bool"
@@ -18964,14 +19094,25 @@
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    MirrorMoveIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
+            " the effects is a status, 2 if it comes from an exclusive item, 0"
+            " otherwise.\n\nr0: pointer to entity\nreturn: int"
+        ),
+    )
+
     Conversion2IsActive = Symbol(
         [0x3D6F4],
         [0x231A274],
         None,
         (
             "Checks if the monster is under the effect of Conversion 2 (its type was"
             " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
@@ -19152,14 +19293,36 @@
             " item is sticky, or if the monster is under the STATUS_MUZZLED status and"
             " the item is edible.\nAlso prints failure messages if required.\n\nr0:"
             " Monster entity pointer\nr1: Item pointer\nreturn: True if the monster can"
             " use the item, false otherwise"
         ),
     )
 
+    ApplyGrimyFoodEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly inflicts poison, shadow hold, burn, paralysis, or an offensive"
+            " stat debuff\nto the target. If the survivalist iq skill or gluttony"
+            " ability is active, the target\nhas a 50% chance not to be"
+            " affected.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyMixElixirEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a Linoone, restores all the PP of all the"
+            " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         [0x42878],
         [0x231F3F8],
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -19249,14 +19412,39 @@
         (
             "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
             " target entity pointer\nr2: warp type\nr3: position (if warp type is"
             " position-based)"
         ),
     )
 
+    TryActivateNondamagingDefenderAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's ability on an attacker. After a move"
+            " is used,\nthis function is called to see if any of the bitflags for an"
+            " ability were set and\napplies the corresponding effect. (The way leech"
+            " seed removes certain statuses is\nalso handled here.)\n\nr0: entity"
+            " pointer"
+        ),
+    )
+
+    TryActivateNondamagingDefenderExclusiveItem = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's item on an attacker. After a move is"
+            " used,\nthis function is called to see if any of the bitflags for an item"
+            " were set and\napplies the corresponding effect.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer"
+        ),
+    )
+
     GetMoveRangeDistance = Symbol(
         [0x4618C],
         [0x2322D0C],
         None,
         (
             "Returns the maximum reach distance of a move, based on its AI range"
             " value.\n\nIf the move doesn't have an AI range value of RANGE_FRONT_10,"
@@ -19417,14 +19605,26 @@
         None,
         (
             "Gets the lower 2 bytes of a 4-byte number and interprets it as a signed"
             " short.\n\nr0: 4-byte number x\nreturn: (short) x"
         ),
     )
 
+    PlayMoveAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Handles the process of getting and playing all the animations for a move."
+            " Waits\nuntil the animation has no more frames before returning.\n\nr0:"
+            " Pointer to the entity that used the move\nr1: Pointer to the entity that"
+            " is the target\nr2: Move pointer\nr3: position"
+        ),
+    )
+
     GetMoveAnimationId = Symbol(
         [0x499F8],
         [0x2326578],
         None,
         (
             "Returns the move animation ID that should be played for a move.\nIt"
             " contains a check for weather ball. After that, if the parameter"
@@ -19580,14 +19780,27 @@
         (
             "Activates the Mud Sport or Water Sport condition on the dungeon floor for"
             " some number of turns.\n\nr0: water sport flag (false for Mud Sport, true"
             " for Water Sport)"
         ),
     )
 
+    TryActivateWeather = Symbol(
+        [0x59384],
+        [0x2335F04],
+        None,
+        (
+            "Tries to change the weather based upon the information for each weather"
+            " type in the\ndungeon struct. Returns whether the weather was succesfully"
+            " changed or not.\n\nr0: bool to not play the weather change"
+            " animation?\nr1: bool to force weather change? Like play the animation and"
+            " text for the weather?\nreturn: True if the weather changed"
+        ),
+    )
+
     DigitCount = Symbol(
         [0x59530],
         [0x23360B0],
         None,
         (
             "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
             " negative, it is cast to a uint16_t before counting digits.\n\nr0:"
@@ -20781,14 +20994,25 @@
         None,
         (
             "Wrapper around GenerateItem with quantity set to 0 and stickiness type set"
             " to SPAWN_STICKY_NEVER.\n\nr0: pointer to item to initialize\nr1: item ID"
         ),
     )
 
+    TryLeaderItemPickUp = Symbol(
+        [0x690C0],
+        [0x2345C40],
+        None,
+        (
+            "Checks the tile at the specified position and determines if the leader"
+            " should pick up an item.\n\nr0: position\nr1: flag for whether or not a"
+            " message should be logged upon the leader failing to obtain the item"
+        ),
+    )
+
     SpawnItem = Symbol(
         [0x695A0],
         [0x2346120],
         None,
         (
             "Spawns an item on the floor. Fails if there are more than 64 items already"
             " on the floor.\n\nThis calls SpawnItemEntity, fills in the item info"
@@ -22256,14 +22480,45 @@
             " is only used for the cardinal directions. The elements at odd indexes are"
             " unused and unconditionally set to 0.\n\nThis array is used by the dungeon"
             " generation algorithm when generating room imperfections. See"
             " GenerateRoomImperfections."
         ),
     )
 
+    GUMMI_LIKE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster liked a gummi in"
+            " decreasing order."
+        ),
+    )
+
+    GUMMI_IQ_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster's IQ was raised by"
+            " in decreasing order."
+        ),
+    )
+
+    DAMAGE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that matches the damage_message ID to their corresponding message ID."
+            " The null entry at 0xE in the middle is for hunger. The last entry is"
+            " null."
+        ),
+    )
+
     DUNGEON_PTR = Symbol(
         [0x775B8],
         [0x2354138],
         0x4,
         (
             "[Runtime] Pointer to the dungeon struct in dungeon mode.\n\nThis is a"
             " 'working copy' of DUNGEON_PTR_MASTER. The main dungeon engine uses this"
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -11817,14 +11817,20 @@
         None,
         None,
         "The chance of Steel Wing boosting defense, as a percentage (20%).",
     )
 
     GOLD_THORN_POWER = Symbol(None, None, None, "Attack power for Golden Thorns.")
 
+    BURN_DAMAGE = Symbol(None, None, None, "Damage dealt by the burn status condition.")
+
+    POISON_DAMAGE = Symbol(
+        None, None, None, "Damage dealt by the poison status condition."
+    )
+
     SPAWN_COOLDOWN = Symbol(
         None,
         None,
         None,
         "The number of turns between enemy spawns under normal conditions.",
     )
 
@@ -11988,14 +11994,28 @@
         ),
     )
 
     SONICBOOM_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by SonicBoom (20)."
     )
 
+    RAIN_ABILITY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is rain for the"
+            " abilities rain dish and dry skin."
+        ),
+    )
+
+    LEECH_SEED_HP_DRAIN = Symbol(
+        None, None, None, "The amount of health drained by leech seed status."
+    )
+
     EXCLUSIVE_ITEM_EXP_BOOST = Symbol(
         None,
         None,
         None,
         "The percentage increase in experience from exp-boosting exclusive items.",
     )
 
@@ -12069,14 +12089,24 @@
 
     STICK_POWER = Symbol(None, None, None, "Attack power for Sticks.")
 
     BUBBLE_LOWER_SPEED_CHANCE = Symbol(
         None, None, None, "The chance of Bubble lowering speed, as a percentage (10%)."
     )
 
+    ICE_BODY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is hail for the"
+            " ability ice body."
+        ),
+    )
+
     POWDER_SNOW_FREEZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Powder Snow (and others, see DoMoveDamageFreeze15) freezing,"
             " as a percentage (15%)."
@@ -12103,14 +12133,24 @@
         ),
     )
 
     POISON_FANG_POISON_CHANCE = Symbol(
         None, None, None, "The chance of Poison Fang poisoning, as a percentage (30%)."
     )
 
+    WEATHER_MOVE_TURN_COUNT = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The number of turns the moves rain dance, hail, sandstorm, sunny day and"
+            " defog change the weather for. (3000)"
+        ),
+    )
+
     THUNDER_PARALYZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Thunder (and others, see DoMoveDamageParalyze20) paralyzing,"
             " as a percentage (20%)"
@@ -12229,14 +12269,18 @@
         ),
     )
 
     POISON_DAMAGE_COOLDOWN = Symbol(
         None, None, None, "The number of turns between passive poison damage."
     )
 
+    LEECH_SEED_DAMAGE_COOLDOWN = Symbol(
+        None, None, None, "The number of turns between leech seed health drain."
+    )
+
     GEO_PEBBLE_DAMAGE = Symbol(None, None, None, "Damage dealt by Geo Pebbles.")
 
     GRAVELEROCK_DAMAGE = Symbol(None, None, None, "Damage dealt by Gravelerocks.")
 
     RARE_FOSSIL_DAMAGE = Symbol(None, None, None, "Damage dealt by Rare Fossils.")
 
     GINSENG_CHANCE_3 = Symbol(
@@ -12257,14 +12301,18 @@
         None, None, None, "The permanent defense boost from ingesting an Iron."
     )
 
     CALCIUM_STAT_BOOST = Symbol(
         None, None, None, "The permanent special attack boost from ingesting a Calcium."
     )
 
+    WISH_BONUS_REGEN = Symbol(
+        None, None, None, "The passive bonus regen given by the wish status condition."
+    )
+
     DRAGON_RAGE_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by Dragon Rage (30)."
     )
 
     CORSOLA_TWIG_POWER = Symbol(None, None, None, "Attack power for Corsola Twigs.")
 
     CACNEA_SPIKE_POWER = Symbol(None, None, None, "Attack power for Cacnea Spikes.")
@@ -12800,14 +12848,25 @@
         (
             "Maps each weather type (by index, see enum weather_id) to the"
             " corresponding Castform type and form.\n\ntype: struct"
             " castform_weather_attributes[8]"
         ),
     )
 
+    BAD_POISON_DAMAGE_TABLE = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Table for how much damage each tick of badly poisoned should deal. The"
+            " table is filled with 0x0006, but could use different values for each"
+            " entry."
+        ),
+    )
+
     TYPE_MATCHUP_COMBINATOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "Table of type matchup combinations.\n\nEach row corresponds to a single"
             " type matchup that results from combining two individual type matchups"
@@ -16247,14 +16306,53 @@
         (
             "A convenience wrapper around SpawnTrap and BindTrapToTile. Always passes 0"
             " for the team parameter (making it an enemy trap).\n\nr0: trap ID\nr1: x"
             " position\nr2: y position\nr3: flags\nstack[0]: visibility flag"
         ),
     )
 
+    PrepareTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Saves the relevant information in the dungeon struct to later place a trap"
+            " at the\nlocation of the entity. (Only called with trap ID 0x19"
+            " (TRAP_NONE), but could be used \nwith others).\n\nr0: entity pointer\nr1:"
+            " trap ID\nr2: team (see struct trap::team)"
+        ),
+    )
+
+    TrySpawnTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the a trap can be placed on the tile. If the trap ID is >="
+            " TRAP_NONE (the\nlast value for a trap), randomly select another trap"
+            " (except for wonder tile). After\n30 failed attempts to select a"
+            " non-wonder tile trap ID, default to chestnut trap.\nIf the checks pass,"
+            " spawn the trap.\n\nr0: position\nr1: trap ID\nr2: team (see struct"
+            " trap::team)\nr3: visibility flag\nreturn: true if a trap was spawned"
+            " succesfully"
+        ),
+    )
+
+    TrySpawnTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the flag for a trapper trap is set, handles spawning a trap based upon"
+            " the\ninformation inside the dungeon struct. Uses the entity for logging a"
+            " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
+            " true if a trap was spawned succesfully"
+        ),
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16490,14 +16588,25 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: target entity"
             " pointer\nr1: current_id\nreturn: ?"
         ),
     )
 
+    TryActivateTraceAndColorChange = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to activate the abilities trace and color change if possible. Called"
+            " after using\na move.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer\nr2: move pointer"
+        ),
+    )
+
     DefenderAbilityIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a defender has an active ability that isn't disabled by an"
             " attacker's Mold Breaker.\n\nThere are two versions of this function,"
@@ -16515,14 +16624,25 @@
         None,
         (
             "Checks if an entity is a monster (entity type 1).\n\nr0: entity"
             " pointer\nreturn: bool"
         ),
     )
 
+    TryActivateConversion2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks for the conversion2 status and applies the type change if"
+            " applicable. Called\nafter using a move.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr2: move pointer"
+        ),
+    )
+
     TryActivateTruant = Symbol(
         None,
         None,
         None,
         (
             "Checks if an entity has the ability Truant, and if so tries to apply the"
             " pause status to it.\n\nr0: pointer to entity"
@@ -17790,14 +17910,24 @@
             " spawn cooldown, it will try to spawn an enemy if the number of enemies is"
             " below the spawn cap.\n\nIf the spawn counter is greater than 900, it will"
             " instead perform the special spawn caused by the ability Illuminate.\n\nNo"
             " params."
         ),
     )
 
+    TryNonLeaderItemPickUp = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to TryLeaderItemPickUp, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: entity pointer"
+        ),
+    )
+
     AuraBowIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is holding an aura bow that isn't disabled by"
             " Klutz.\n\nr0: entity pointer\nreturn: bool"
@@ -18474,14 +18604,25 @@
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    MirrorMoveIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
+            " the effects is a status, 2 if it comes from an exclusive item, 0"
+            " otherwise.\n\nr0: pointer to entity\nreturn: int"
+        ),
+    )
+
     Conversion2IsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Conversion 2 (its type was"
             " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
@@ -18662,14 +18803,36 @@
             " item is sticky, or if the monster is under the STATUS_MUZZLED status and"
             " the item is edible.\nAlso prints failure messages if required.\n\nr0:"
             " Monster entity pointer\nr1: Item pointer\nreturn: True if the monster can"
             " use the item, false otherwise"
         ),
     )
 
+    ApplyGrimyFoodEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly inflicts poison, shadow hold, burn, paralysis, or an offensive"
+            " stat debuff\nto the target. If the survivalist iq skill or gluttony"
+            " ability is active, the target\nhas a 50% chance not to be"
+            " affected.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyMixElixirEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a Linoone, restores all the PP of all the"
+            " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -18759,14 +18922,39 @@
         (
             "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
             " target entity pointer\nr2: warp type\nr3: position (if warp type is"
             " position-based)"
         ),
     )
 
+    TryActivateNondamagingDefenderAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's ability on an attacker. After a move"
+            " is used,\nthis function is called to see if any of the bitflags for an"
+            " ability were set and\napplies the corresponding effect. (The way leech"
+            " seed removes certain statuses is\nalso handled here.)\n\nr0: entity"
+            " pointer"
+        ),
+    )
+
+    TryActivateNondamagingDefenderExclusiveItem = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's item on an attacker. After a move is"
+            " used,\nthis function is called to see if any of the bitflags for an item"
+            " were set and\napplies the corresponding effect.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer"
+        ),
+    )
+
     GetMoveRangeDistance = Symbol(
         None,
         None,
         None,
         (
             "Returns the maximum reach distance of a move, based on its AI range"
             " value.\n\nIf the move doesn't have an AI range value of RANGE_FRONT_10,"
@@ -18927,14 +19115,26 @@
         None,
         (
             "Gets the lower 2 bytes of a 4-byte number and interprets it as a signed"
             " short.\n\nr0: 4-byte number x\nreturn: (short) x"
         ),
     )
 
+    PlayMoveAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Handles the process of getting and playing all the animations for a move."
+            " Waits\nuntil the animation has no more frames before returning.\n\nr0:"
+            " Pointer to the entity that used the move\nr1: Pointer to the entity that"
+            " is the target\nr2: Move pointer\nr3: position"
+        ),
+    )
+
     GetMoveAnimationId = Symbol(
         None,
         None,
         None,
         (
             "Returns the move animation ID that should be played for a move.\nIt"
             " contains a check for weather ball. After that, if the parameter"
@@ -19090,14 +19290,27 @@
         (
             "Activates the Mud Sport or Water Sport condition on the dungeon floor for"
             " some number of turns.\n\nr0: water sport flag (false for Mud Sport, true"
             " for Water Sport)"
         ),
     )
 
+    TryActivateWeather = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to change the weather based upon the information for each weather"
+            " type in the\ndungeon struct. Returns whether the weather was succesfully"
+            " changed or not.\n\nr0: bool to not play the weather change"
+            " animation?\nr1: bool to force weather change? Like play the animation and"
+            " text for the weather?\nreturn: True if the weather changed"
+        ),
+    )
+
     DigitCount = Symbol(
         None,
         None,
         None,
         (
             "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
             " negative, it is cast to a uint16_t before counting digits.\n\nr0:"
@@ -20276,14 +20489,25 @@
         None,
         (
             "Wrapper around GenerateItem with quantity set to 0 and stickiness type set"
             " to SPAWN_STICKY_NEVER.\n\nr0: pointer to item to initialize\nr1: item ID"
         ),
     )
 
+    TryLeaderItemPickUp = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile at the specified position and determines if the leader"
+            " should pick up an item.\n\nr0: position\nr1: flag for whether or not a"
+            " message should be logged upon the leader failing to obtain the item"
+        ),
+    )
+
     SpawnItem = Symbol(
         None,
         None,
         None,
         (
             "Spawns an item on the floor. Fails if there are more than 64 items already"
             " on the floor.\n\nThis calls SpawnItemEntity, fills in the item info"
@@ -21634,14 +21858,45 @@
             " is only used for the cardinal directions. The elements at odd indexes are"
             " unused and unconditionally set to 0.\n\nThis array is used by the dungeon"
             " generation algorithm when generating room imperfections. See"
             " GenerateRoomImperfections."
         ),
     )
 
+    GUMMI_LIKE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster liked a gummi in"
+            " decreasing order."
+        ),
+    )
+
+    GUMMI_IQ_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster's IQ was raised by"
+            " in decreasing order."
+        ),
+    )
+
+    DAMAGE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that matches the damage_message ID to their corresponding message ID."
+            " The null entry at 0xE in the middle is for hunger. The last entry is"
+            " null."
+        ),
+    )
+
     DUNGEON_PTR = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Pointer to the dungeon struct in dungeon mode.\n\nThis is a"
             " 'working copy' of DUNGEON_PTR_MASTER. The main dungeon engine uses this"
```

## pmdsky_debug_py/jp.py

```diff
@@ -12048,14 +12048,20 @@
         None,
         None,
         "The chance of Steel Wing boosting defense, as a percentage (20%).",
     )
 
     GOLD_THORN_POWER = Symbol(None, None, None, "Attack power for Golden Thorns.")
 
+    BURN_DAMAGE = Symbol(None, None, None, "Damage dealt by the burn status condition.")
+
+    POISON_DAMAGE = Symbol(
+        None, None, None, "Damage dealt by the poison status condition."
+    )
+
     SPAWN_COOLDOWN = Symbol(
         None,
         None,
         None,
         "The number of turns between enemy spawns under normal conditions.",
     )
 
@@ -12219,14 +12225,28 @@
         ),
     )
 
     SONICBOOM_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by SonicBoom (20)."
     )
 
+    RAIN_ABILITY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is rain for the"
+            " abilities rain dish and dry skin."
+        ),
+    )
+
+    LEECH_SEED_HP_DRAIN = Symbol(
+        None, None, None, "The amount of health drained by leech seed status."
+    )
+
     EXCLUSIVE_ITEM_EXP_BOOST = Symbol(
         None,
         None,
         None,
         "The percentage increase in experience from exp-boosting exclusive items.",
     )
 
@@ -12300,14 +12320,24 @@
 
     STICK_POWER = Symbol(None, None, None, "Attack power for Sticks.")
 
     BUBBLE_LOWER_SPEED_CHANCE = Symbol(
         None, None, None, "The chance of Bubble lowering speed, as a percentage (10%)."
     )
 
+    ICE_BODY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is hail for the"
+            " ability ice body."
+        ),
+    )
+
     POWDER_SNOW_FREEZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Powder Snow (and others, see DoMoveDamageFreeze15) freezing,"
             " as a percentage (15%)."
@@ -12334,14 +12364,24 @@
         ),
     )
 
     POISON_FANG_POISON_CHANCE = Symbol(
         None, None, None, "The chance of Poison Fang poisoning, as a percentage (30%)."
     )
 
+    WEATHER_MOVE_TURN_COUNT = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The number of turns the moves rain dance, hail, sandstorm, sunny day and"
+            " defog change the weather for. (3000)"
+        ),
+    )
+
     THUNDER_PARALYZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Thunder (and others, see DoMoveDamageParalyze20) paralyzing,"
             " as a percentage (20%)"
@@ -12460,14 +12500,18 @@
         ),
     )
 
     POISON_DAMAGE_COOLDOWN = Symbol(
         None, None, None, "The number of turns between passive poison damage."
     )
 
+    LEECH_SEED_DAMAGE_COOLDOWN = Symbol(
+        None, None, None, "The number of turns between leech seed health drain."
+    )
+
     GEO_PEBBLE_DAMAGE = Symbol(None, None, None, "Damage dealt by Geo Pebbles.")
 
     GRAVELEROCK_DAMAGE = Symbol(None, None, None, "Damage dealt by Gravelerocks.")
 
     RARE_FOSSIL_DAMAGE = Symbol(None, None, None, "Damage dealt by Rare Fossils.")
 
     GINSENG_CHANCE_3 = Symbol(
@@ -12488,14 +12532,18 @@
         None, None, None, "The permanent defense boost from ingesting an Iron."
     )
 
     CALCIUM_STAT_BOOST = Symbol(
         None, None, None, "The permanent special attack boost from ingesting a Calcium."
     )
 
+    WISH_BONUS_REGEN = Symbol(
+        None, None, None, "The passive bonus regen given by the wish status condition."
+    )
+
     DRAGON_RAGE_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by Dragon Rage (30)."
     )
 
     CORSOLA_TWIG_POWER = Symbol(None, None, None, "Attack power for Corsola Twigs.")
 
     CACNEA_SPIKE_POWER = Symbol(None, None, None, "Attack power for Cacnea Spikes.")
@@ -13031,14 +13079,25 @@
         (
             "Maps each weather type (by index, see enum weather_id) to the"
             " corresponding Castform type and form.\n\ntype: struct"
             " castform_weather_attributes[8]"
         ),
     )
 
+    BAD_POISON_DAMAGE_TABLE = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Table for how much damage each tick of badly poisoned should deal. The"
+            " table is filled with 0x0006, but could use different values for each"
+            " entry."
+        ),
+    )
+
     TYPE_MATCHUP_COMBINATOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "Table of type matchup combinations.\n\nEach row corresponds to a single"
             " type matchup that results from combining two individual type matchups"
@@ -16494,14 +16553,53 @@
         (
             "A convenience wrapper around SpawnTrap and BindTrapToTile. Always passes 0"
             " for the team parameter (making it an enemy trap).\n\nr0: trap ID\nr1: x"
             " position\nr2: y position\nr3: flags\nstack[0]: visibility flag"
         ),
     )
 
+    PrepareTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Saves the relevant information in the dungeon struct to later place a trap"
+            " at the\nlocation of the entity. (Only called with trap ID 0x19"
+            " (TRAP_NONE), but could be used \nwith others).\n\nr0: entity pointer\nr1:"
+            " trap ID\nr2: team (see struct trap::team)"
+        ),
+    )
+
+    TrySpawnTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the a trap can be placed on the tile. If the trap ID is >="
+            " TRAP_NONE (the\nlast value for a trap), randomly select another trap"
+            " (except for wonder tile). After\n30 failed attempts to select a"
+            " non-wonder tile trap ID, default to chestnut trap.\nIf the checks pass,"
+            " spawn the trap.\n\nr0: position\nr1: trap ID\nr2: team (see struct"
+            " trap::team)\nr3: visibility flag\nreturn: true if a trap was spawned"
+            " succesfully"
+        ),
+    )
+
+    TrySpawnTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the flag for a trapper trap is set, handles spawning a trap based upon"
+            " the\ninformation inside the dungeon struct. Uses the entity for logging a"
+            " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
+            " true if a trap was spawned succesfully"
+        ),
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x13790],
         [0x22F1070],
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16740,14 +16838,25 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: target entity"
             " pointer\nr1: current_id\nreturn: ?"
         ),
     )
 
+    TryActivateTraceAndColorChange = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to activate the abilities trace and color change if possible. Called"
+            " after using\na move.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer\nr2: move pointer"
+        ),
+    )
+
     DefenderAbilityIsActive = Symbol(
         [0x25694],
         [0x2302F74],
         None,
         (
             "Checks if a defender has an active ability that isn't disabled by an"
             " attacker's Mold Breaker.\n\nThere are two versions of this function,"
@@ -16765,14 +16874,25 @@
         None,
         (
             "Checks if an entity is a monster (entity type 1).\n\nr0: entity"
             " pointer\nreturn: bool"
         ),
     )
 
+    TryActivateConversion2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks for the conversion2 status and applies the type change if"
+            " applicable. Called\nafter using a move.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr2: move pointer"
+        ),
+    )
+
     TryActivateTruant = Symbol(
         [0x1D4C8],
         [0x22FADA8],
         None,
         (
             "Checks if an entity has the ability Truant, and if so tries to apply the"
             " pause status to it.\n\nr0: pointer to entity"
@@ -18040,14 +18160,24 @@
             " spawn cooldown, it will try to spawn an enemy if the number of enemies is"
             " below the spawn cap.\n\nIf the spawn counter is greater than 900, it will"
             " instead perform the special spawn caused by the ability Illuminate.\n\nNo"
             " params."
         ),
     )
 
+    TryNonLeaderItemPickUp = Symbol(
+        [0x32DC0],
+        [0x23106A0],
+        None,
+        (
+            "Similar to TryLeaderItemPickUp, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: entity pointer"
+        ),
+    )
+
     AuraBowIsActive = Symbol(
         [0x33324],
         [0x2310C04],
         None,
         (
             "Checks if a monster is holding an aura bow that isn't disabled by"
             " Klutz.\n\nr0: entity pointer\nreturn: bool"
@@ -18724,14 +18854,25 @@
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    MirrorMoveIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
+            " the effects is a status, 2 if it comes from an exclusive item, 0"
+            " otherwise.\n\nr0: pointer to entity\nreturn: int"
+        ),
+    )
+
     Conversion2IsActive = Symbol(
         [0x3D404],
         [0x231ACE4],
         None,
         (
             "Checks if the monster is under the effect of Conversion 2 (its type was"
             " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
@@ -18912,14 +19053,36 @@
             " item is sticky, or if the monster is under the STATUS_MUZZLED status and"
             " the item is edible.\nAlso prints failure messages if required.\n\nr0:"
             " Monster entity pointer\nr1: Item pointer\nreturn: True if the monster can"
             " use the item, false otherwise"
         ),
     )
 
+    ApplyGrimyFoodEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly inflicts poison, shadow hold, burn, paralysis, or an offensive"
+            " stat debuff\nto the target. If the survivalist iq skill or gluttony"
+            " ability is active, the target\nhas a 50% chance not to be"
+            " affected.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyMixElixirEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a Linoone, restores all the PP of all the"
+            " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -19009,14 +19172,39 @@
         (
             "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
             " target entity pointer\nr2: warp type\nr3: position (if warp type is"
             " position-based)"
         ),
     )
 
+    TryActivateNondamagingDefenderAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's ability on an attacker. After a move"
+            " is used,\nthis function is called to see if any of the bitflags for an"
+            " ability were set and\napplies the corresponding effect. (The way leech"
+            " seed removes certain statuses is\nalso handled here.)\n\nr0: entity"
+            " pointer"
+        ),
+    )
+
+    TryActivateNondamagingDefenderExclusiveItem = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's item on an attacker. After a move is"
+            " used,\nthis function is called to see if any of the bitflags for an item"
+            " were set and\napplies the corresponding effect.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer"
+        ),
+    )
+
     GetMoveRangeDistance = Symbol(
         None,
         None,
         None,
         (
             "Returns the maximum reach distance of a move, based on its AI range"
             " value.\n\nIf the move doesn't have an AI range value of RANGE_FRONT_10,"
@@ -19177,14 +19365,26 @@
         None,
         (
             "Gets the lower 2 bytes of a 4-byte number and interprets it as a signed"
             " short.\n\nr0: 4-byte number x\nreturn: (short) x"
         ),
     )
 
+    PlayMoveAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Handles the process of getting and playing all the animations for a move."
+            " Waits\nuntil the animation has no more frames before returning.\n\nr0:"
+            " Pointer to the entity that used the move\nr1: Pointer to the entity that"
+            " is the target\nr2: Move pointer\nr3: position"
+        ),
+    )
+
     GetMoveAnimationId = Symbol(
         [0x496BC],
         [0x2326F9C],
         None,
         (
             "Returns the move animation ID that should be played for a move.\nIt"
             " contains a check for weather ball. After that, if the parameter"
@@ -19340,14 +19540,27 @@
         (
             "Activates the Mud Sport or Water Sport condition on the dungeon floor for"
             " some number of turns.\n\nr0: water sport flag (false for Mud Sport, true"
             " for Water Sport)"
         ),
     )
 
+    TryActivateWeather = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to change the weather based upon the information for each weather"
+            " type in the\ndungeon struct. Returns whether the weather was succesfully"
+            " changed or not.\n\nr0: bool to not play the weather change"
+            " animation?\nr1: bool to force weather change? Like play the animation and"
+            " text for the weather?\nreturn: True if the weather changed"
+        ),
+    )
+
     DigitCount = Symbol(
         [0x5917C],
         [0x2336A5C],
         None,
         (
             "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
             " negative, it is cast to a uint16_t before counting digits.\n\nr0:"
@@ -20538,14 +20751,25 @@
         None,
         (
             "Wrapper around GenerateItem with quantity set to 0 and stickiness type set"
             " to SPAWN_STICKY_NEVER.\n\nr0: pointer to item to initialize\nr1: item ID"
         ),
     )
 
+    TryLeaderItemPickUp = Symbol(
+        [0x68B3C],
+        [0x234641C],
+        None,
+        (
+            "Checks the tile at the specified position and determines if the leader"
+            " should pick up an item.\n\nr0: position\nr1: flag for whether or not a"
+            " message should be logged upon the leader failing to obtain the item"
+        ),
+    )
+
     SpawnItem = Symbol(
         [0x6901C],
         [0x23468FC],
         None,
         (
             "Spawns an item on the floor. Fails if there are more than 64 items already"
             " on the floor.\n\nThis calls SpawnItemEntity, fills in the item info"
@@ -21900,14 +22124,45 @@
             " is only used for the cardinal directions. The elements at odd indexes are"
             " unused and unconditionally set to 0.\n\nThis array is used by the dungeon"
             " generation algorithm when generating room imperfections. See"
             " GenerateRoomImperfections."
         ),
     )
 
+    GUMMI_LIKE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster liked a gummi in"
+            " decreasing order."
+        ),
+    )
+
+    GUMMI_IQ_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster's IQ was raised by"
+            " in decreasing order."
+        ),
+    )
+
+    DAMAGE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that matches the damage_message ID to their corresponding message ID."
+            " The null entry at 0xE in the middle is for hunger. The last entry is"
+            " null."
+        ),
+    )
+
     DUNGEON_PTR = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Pointer to the dungeon struct in dungeon mode.\n\nThis is a"
             " 'working copy' of DUNGEON_PTR_MASTER. The main dungeon engine uses this"
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -11817,14 +11817,20 @@
         None,
         None,
         "The chance of Steel Wing boosting defense, as a percentage (20%).",
     )
 
     GOLD_THORN_POWER = Symbol(None, None, None, "Attack power for Golden Thorns.")
 
+    BURN_DAMAGE = Symbol(None, None, None, "Damage dealt by the burn status condition.")
+
+    POISON_DAMAGE = Symbol(
+        None, None, None, "Damage dealt by the poison status condition."
+    )
+
     SPAWN_COOLDOWN = Symbol(
         None,
         None,
         None,
         "The number of turns between enemy spawns under normal conditions.",
     )
 
@@ -11988,14 +11994,28 @@
         ),
     )
 
     SONICBOOM_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by SonicBoom (20)."
     )
 
+    RAIN_ABILITY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is rain for the"
+            " abilities rain dish and dry skin."
+        ),
+    )
+
+    LEECH_SEED_HP_DRAIN = Symbol(
+        None, None, None, "The amount of health drained by leech seed status."
+    )
+
     EXCLUSIVE_ITEM_EXP_BOOST = Symbol(
         None,
         None,
         None,
         "The percentage increase in experience from exp-boosting exclusive items.",
     )
 
@@ -12069,14 +12089,24 @@
 
     STICK_POWER = Symbol(None, None, None, "Attack power for Sticks.")
 
     BUBBLE_LOWER_SPEED_CHANCE = Symbol(
         None, None, None, "The chance of Bubble lowering speed, as a percentage (10%)."
     )
 
+    ICE_BODY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is hail for the"
+            " ability ice body."
+        ),
+    )
+
     POWDER_SNOW_FREEZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Powder Snow (and others, see DoMoveDamageFreeze15) freezing,"
             " as a percentage (15%)."
@@ -12103,14 +12133,24 @@
         ),
     )
 
     POISON_FANG_POISON_CHANCE = Symbol(
         None, None, None, "The chance of Poison Fang poisoning, as a percentage (30%)."
     )
 
+    WEATHER_MOVE_TURN_COUNT = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The number of turns the moves rain dance, hail, sandstorm, sunny day and"
+            " defog change the weather for. (3000)"
+        ),
+    )
+
     THUNDER_PARALYZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Thunder (and others, see DoMoveDamageParalyze20) paralyzing,"
             " as a percentage (20%)"
@@ -12229,14 +12269,18 @@
         ),
     )
 
     POISON_DAMAGE_COOLDOWN = Symbol(
         None, None, None, "The number of turns between passive poison damage."
     )
 
+    LEECH_SEED_DAMAGE_COOLDOWN = Symbol(
+        None, None, None, "The number of turns between leech seed health drain."
+    )
+
     GEO_PEBBLE_DAMAGE = Symbol(None, None, None, "Damage dealt by Geo Pebbles.")
 
     GRAVELEROCK_DAMAGE = Symbol(None, None, None, "Damage dealt by Gravelerocks.")
 
     RARE_FOSSIL_DAMAGE = Symbol(None, None, None, "Damage dealt by Rare Fossils.")
 
     GINSENG_CHANCE_3 = Symbol(
@@ -12257,14 +12301,18 @@
         None, None, None, "The permanent defense boost from ingesting an Iron."
     )
 
     CALCIUM_STAT_BOOST = Symbol(
         None, None, None, "The permanent special attack boost from ingesting a Calcium."
     )
 
+    WISH_BONUS_REGEN = Symbol(
+        None, None, None, "The passive bonus regen given by the wish status condition."
+    )
+
     DRAGON_RAGE_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by Dragon Rage (30)."
     )
 
     CORSOLA_TWIG_POWER = Symbol(None, None, None, "Attack power for Corsola Twigs.")
 
     CACNEA_SPIKE_POWER = Symbol(None, None, None, "Attack power for Cacnea Spikes.")
@@ -12800,14 +12848,25 @@
         (
             "Maps each weather type (by index, see enum weather_id) to the"
             " corresponding Castform type and form.\n\ntype: struct"
             " castform_weather_attributes[8]"
         ),
     )
 
+    BAD_POISON_DAMAGE_TABLE = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Table for how much damage each tick of badly poisoned should deal. The"
+            " table is filled with 0x0006, but could use different values for each"
+            " entry."
+        ),
+    )
+
     TYPE_MATCHUP_COMBINATOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "Table of type matchup combinations.\n\nEach row corresponds to a single"
             " type matchup that results from combining two individual type matchups"
@@ -16247,14 +16306,53 @@
         (
             "A convenience wrapper around SpawnTrap and BindTrapToTile. Always passes 0"
             " for the team parameter (making it an enemy trap).\n\nr0: trap ID\nr1: x"
             " position\nr2: y position\nr3: flags\nstack[0]: visibility flag"
         ),
     )
 
+    PrepareTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Saves the relevant information in the dungeon struct to later place a trap"
+            " at the\nlocation of the entity. (Only called with trap ID 0x19"
+            " (TRAP_NONE), but could be used \nwith others).\n\nr0: entity pointer\nr1:"
+            " trap ID\nr2: team (see struct trap::team)"
+        ),
+    )
+
+    TrySpawnTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the a trap can be placed on the tile. If the trap ID is >="
+            " TRAP_NONE (the\nlast value for a trap), randomly select another trap"
+            " (except for wonder tile). After\n30 failed attempts to select a"
+            " non-wonder tile trap ID, default to chestnut trap.\nIf the checks pass,"
+            " spawn the trap.\n\nr0: position\nr1: trap ID\nr2: team (see struct"
+            " trap::team)\nr3: visibility flag\nreturn: true if a trap was spawned"
+            " succesfully"
+        ),
+    )
+
+    TrySpawnTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the flag for a trapper trap is set, handles spawning a trap based upon"
+            " the\ninformation inside the dungeon struct. Uses the entity for logging a"
+            " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
+            " true if a trap was spawned succesfully"
+        ),
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16490,14 +16588,25 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: target entity"
             " pointer\nr1: current_id\nreturn: ?"
         ),
     )
 
+    TryActivateTraceAndColorChange = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to activate the abilities trace and color change if possible. Called"
+            " after using\na move.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer\nr2: move pointer"
+        ),
+    )
+
     DefenderAbilityIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a defender has an active ability that isn't disabled by an"
             " attacker's Mold Breaker.\n\nThere are two versions of this function,"
@@ -16515,14 +16624,25 @@
         None,
         (
             "Checks if an entity is a monster (entity type 1).\n\nr0: entity"
             " pointer\nreturn: bool"
         ),
     )
 
+    TryActivateConversion2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks for the conversion2 status and applies the type change if"
+            " applicable. Called\nafter using a move.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr2: move pointer"
+        ),
+    )
+
     TryActivateTruant = Symbol(
         None,
         None,
         None,
         (
             "Checks if an entity has the ability Truant, and if so tries to apply the"
             " pause status to it.\n\nr0: pointer to entity"
@@ -17790,14 +17910,24 @@
             " spawn cooldown, it will try to spawn an enemy if the number of enemies is"
             " below the spawn cap.\n\nIf the spawn counter is greater than 900, it will"
             " instead perform the special spawn caused by the ability Illuminate.\n\nNo"
             " params."
         ),
     )
 
+    TryNonLeaderItemPickUp = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to TryLeaderItemPickUp, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: entity pointer"
+        ),
+    )
+
     AuraBowIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is holding an aura bow that isn't disabled by"
             " Klutz.\n\nr0: entity pointer\nreturn: bool"
@@ -18474,14 +18604,25 @@
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    MirrorMoveIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
+            " the effects is a status, 2 if it comes from an exclusive item, 0"
+            " otherwise.\n\nr0: pointer to entity\nreturn: int"
+        ),
+    )
+
     Conversion2IsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Conversion 2 (its type was"
             " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
@@ -18662,14 +18803,36 @@
             " item is sticky, or if the monster is under the STATUS_MUZZLED status and"
             " the item is edible.\nAlso prints failure messages if required.\n\nr0:"
             " Monster entity pointer\nr1: Item pointer\nreturn: True if the monster can"
             " use the item, false otherwise"
         ),
     )
 
+    ApplyGrimyFoodEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly inflicts poison, shadow hold, burn, paralysis, or an offensive"
+            " stat debuff\nto the target. If the survivalist iq skill or gluttony"
+            " ability is active, the target\nhas a 50% chance not to be"
+            " affected.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyMixElixirEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a Linoone, restores all the PP of all the"
+            " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -18759,14 +18922,39 @@
         (
             "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
             " target entity pointer\nr2: warp type\nr3: position (if warp type is"
             " position-based)"
         ),
     )
 
+    TryActivateNondamagingDefenderAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's ability on an attacker. After a move"
+            " is used,\nthis function is called to see if any of the bitflags for an"
+            " ability were set and\napplies the corresponding effect. (The way leech"
+            " seed removes certain statuses is\nalso handled here.)\n\nr0: entity"
+            " pointer"
+        ),
+    )
+
+    TryActivateNondamagingDefenderExclusiveItem = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's item on an attacker. After a move is"
+            " used,\nthis function is called to see if any of the bitflags for an item"
+            " were set and\napplies the corresponding effect.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer"
+        ),
+    )
+
     GetMoveRangeDistance = Symbol(
         None,
         None,
         None,
         (
             "Returns the maximum reach distance of a move, based on its AI range"
             " value.\n\nIf the move doesn't have an AI range value of RANGE_FRONT_10,"
@@ -18927,14 +19115,26 @@
         None,
         (
             "Gets the lower 2 bytes of a 4-byte number and interprets it as a signed"
             " short.\n\nr0: 4-byte number x\nreturn: (short) x"
         ),
     )
 
+    PlayMoveAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Handles the process of getting and playing all the animations for a move."
+            " Waits\nuntil the animation has no more frames before returning.\n\nr0:"
+            " Pointer to the entity that used the move\nr1: Pointer to the entity that"
+            " is the target\nr2: Move pointer\nr3: position"
+        ),
+    )
+
     GetMoveAnimationId = Symbol(
         None,
         None,
         None,
         (
             "Returns the move animation ID that should be played for a move.\nIt"
             " contains a check for weather ball. After that, if the parameter"
@@ -19090,14 +19290,27 @@
         (
             "Activates the Mud Sport or Water Sport condition on the dungeon floor for"
             " some number of turns.\n\nr0: water sport flag (false for Mud Sport, true"
             " for Water Sport)"
         ),
     )
 
+    TryActivateWeather = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to change the weather based upon the information for each weather"
+            " type in the\ndungeon struct. Returns whether the weather was succesfully"
+            " changed or not.\n\nr0: bool to not play the weather change"
+            " animation?\nr1: bool to force weather change? Like play the animation and"
+            " text for the weather?\nreturn: True if the weather changed"
+        ),
+    )
+
     DigitCount = Symbol(
         None,
         None,
         None,
         (
             "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
             " negative, it is cast to a uint16_t before counting digits.\n\nr0:"
@@ -20276,14 +20489,25 @@
         None,
         (
             "Wrapper around GenerateItem with quantity set to 0 and stickiness type set"
             " to SPAWN_STICKY_NEVER.\n\nr0: pointer to item to initialize\nr1: item ID"
         ),
     )
 
+    TryLeaderItemPickUp = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile at the specified position and determines if the leader"
+            " should pick up an item.\n\nr0: position\nr1: flag for whether or not a"
+            " message should be logged upon the leader failing to obtain the item"
+        ),
+    )
+
     SpawnItem = Symbol(
         None,
         None,
         None,
         (
             "Spawns an item on the floor. Fails if there are more than 64 items already"
             " on the floor.\n\nThis calls SpawnItemEntity, fills in the item info"
@@ -21634,14 +21858,45 @@
             " is only used for the cardinal directions. The elements at odd indexes are"
             " unused and unconditionally set to 0.\n\nThis array is used by the dungeon"
             " generation algorithm when generating room imperfections. See"
             " GenerateRoomImperfections."
         ),
     )
 
+    GUMMI_LIKE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster liked a gummi in"
+            " decreasing order."
+        ),
+    )
+
+    GUMMI_IQ_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster's IQ was raised by"
+            " in decreasing order."
+        ),
+    )
+
+    DAMAGE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that matches the damage_message ID to their corresponding message ID."
+            " The null entry at 0xE in the middle is for hunger. The last entry is"
+            " null."
+        ),
+    )
+
     DUNGEON_PTR = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Pointer to the dungeon struct in dungeon mode.\n\nThis is a"
             " 'working copy' of DUNGEON_PTR_MASTER. The main dungeon engine uses this"
```

## pmdsky_debug_py/na.py

```diff
@@ -12106,14 +12106,22 @@
         "The chance of Steel Wing boosting defense, as a percentage (20%).",
     )
 
     GOLD_THORN_POWER = Symbol(
         [0x7A50], [0x22C44D0], 0x2, "Attack power for Golden Thorns."
     )
 
+    BURN_DAMAGE = Symbol(
+        [0x7A54], [0x22C44D4], 0x2, "Damage dealt by the burn status condition."
+    )
+
+    POISON_DAMAGE = Symbol(
+        [0x7A58], [0x22C44D8], 0x2, "Damage dealt by the poison status condition."
+    )
+
     SPAWN_COOLDOWN = Symbol(
         [0x7A5C],
         [0x22C44DC],
         0x2,
         "The number of turns between enemy spawns under normal conditions.",
     )
 
@@ -12289,14 +12297,28 @@
     SONICBOOM_FIXED_DAMAGE = Symbol(
         [0x7AE8],
         [0x22C4568],
         0x2,
         "The amount of fixed damage dealt by SonicBoom (20).",
     )
 
+    RAIN_ABILITY_BONUS_REGEN = Symbol(
+        [0x7AF8],
+        [0x22C4578],
+        0x2,
+        (
+            "The passive bonus health regen given when the weather is rain for the"
+            " abilities rain dish and dry skin."
+        ),
+    )
+
+    LEECH_SEED_HP_DRAIN = Symbol(
+        [0x7B08], [0x22C4588], 0x2, "The amount of health drained by leech seed status."
+    )
+
     EXCLUSIVE_ITEM_EXP_BOOST = Symbol(
         [0x7B0C],
         [0x22C458C],
         0x2,
         "The percentage increase in experience from exp-boosting exclusive items.",
     )
 
@@ -12379,14 +12401,24 @@
     BUBBLE_LOWER_SPEED_CHANCE = Symbol(
         [0x7BAC],
         [0x22C462C],
         0x2,
         "The chance of Bubble lowering speed, as a percentage (10%).",
     )
 
+    ICE_BODY_BONUS_REGEN = Symbol(
+        [0x7BB0],
+        [0x22C4630],
+        None,
+        (
+            "The passive bonus health regen given when the weather is hail for the"
+            " ability ice body."
+        ),
+    )
+
     POWDER_SNOW_FREEZE_CHANCE = Symbol(
         [0x7BB4],
         [0x22C4634],
         0x2,
         (
             "The chance of Powder Snow (and others, see DoMoveDamageFreeze15) freezing,"
             " as a percentage (15%)."
@@ -12416,14 +12448,24 @@
     POISON_FANG_POISON_CHANCE = Symbol(
         [0x7BC4],
         [0x22C4644],
         0x2,
         "The chance of Poison Fang poisoning, as a percentage (30%).",
     )
 
+    WEATHER_MOVE_TURN_COUNT = Symbol(
+        [0x7BD4],
+        [0x22C4654],
+        0x2,
+        (
+            "The number of turns the moves rain dance, hail, sandstorm, sunny day and"
+            " defog change the weather for. (3000)"
+        ),
+    )
+
     THUNDER_PARALYZE_CHANCE = Symbol(
         [0x7BD8],
         [0x22C4658],
         0x2,
         (
             "The chance of Thunder (and others, see DoMoveDamageParalyze20) paralyzing,"
             " as a percentage (20%)"
@@ -12545,14 +12587,21 @@
         ),
     )
 
     POISON_DAMAGE_COOLDOWN = Symbol(
         [0x7C28], [0x22C46A8], 0x2, "The number of turns between passive poison damage."
     )
 
+    LEECH_SEED_DAMAGE_COOLDOWN = Symbol(
+        [0x7C2C],
+        [0x22C46AC],
+        0x2,
+        "The number of turns between leech seed health drain.",
+    )
+
     GEO_PEBBLE_DAMAGE = Symbol(
         [0x7C34], [0x22C46B4], 0x2, "Damage dealt by Geo Pebbles."
     )
 
     GRAVELEROCK_DAMAGE = Symbol(
         [0x7C38], [0x22C46B8], 0x2, "Damage dealt by Gravelerocks."
     )
@@ -12588,14 +12637,21 @@
     CALCIUM_STAT_BOOST = Symbol(
         [0x7C4C],
         [0x22C46CC],
         0x2,
         "The permanent special attack boost from ingesting a Calcium.",
     )
 
+    WISH_BONUS_REGEN = Symbol(
+        [0x7C50],
+        [0x22C46D0],
+        0x2,
+        "The passive bonus regen given by the wish status condition.",
+    )
+
     DRAGON_RAGE_FIXED_DAMAGE = Symbol(
         [0x7C54],
         [0x22C46D4],
         0x2,
         "The amount of fixed damage dealt by Dragon Rage (30).",
     )
 
@@ -13142,14 +13198,25 @@
         (
             "Maps each weather type (by index, see enum weather_id) to the"
             " corresponding Castform type and form.\n\ntype: struct"
             " castform_weather_attributes[8]"
         ),
     )
 
+    BAD_POISON_DAMAGE_TABLE = Symbol(
+        [0x821C],
+        [0x22C4C9C],
+        0x3C,
+        (
+            "Table for how much damage each tick of badly poisoned should deal. The"
+            " table is filled with 0x0006, but could use different values for each"
+            " entry."
+        ),
+    )
+
     TYPE_MATCHUP_COMBINATOR_TABLE = Symbol(
         [0x8294],
         [0x22C4D14],
         0x40,
         (
             "Table of type matchup combinations.\n\nEach row corresponds to a single"
             " type matchup that results from combining two individual type matchups"
@@ -16767,14 +16834,53 @@
         (
             "A convenience wrapper around SpawnTrap and BindTrapToTile. Always passes 0"
             " for the team parameter (making it an enemy trap).\n\nr0: trap ID\nr1: x"
             " position\nr2: y position\nr3: flags\nstack[0]: visibility flag"
         ),
     )
 
+    PrepareTrapperTrap = Symbol(
+        [0x11994],
+        [0x22EDBD4],
+        None,
+        (
+            "Saves the relevant information in the dungeon struct to later place a trap"
+            " at the\nlocation of the entity. (Only called with trap ID 0x19"
+            " (TRAP_NONE), but could be used \nwith others).\n\nr0: entity pointer\nr1:"
+            " trap ID\nr2: team (see struct trap::team)"
+        ),
+    )
+
+    TrySpawnTrap = Symbol(
+        [0x11A7C],
+        [0x22EDCBC],
+        None,
+        (
+            "Checks if the a trap can be placed on the tile. If the trap ID is >="
+            " TRAP_NONE (the\nlast value for a trap), randomly select another trap"
+            " (except for wonder tile). After\n30 failed attempts to select a"
+            " non-wonder tile trap ID, default to chestnut trap.\nIf the checks pass,"
+            " spawn the trap.\n\nr0: position\nr1: trap ID\nr2: team (see struct"
+            " trap::team)\nr3: visibility flag\nreturn: true if a trap was spawned"
+            " succesfully"
+        ),
+    )
+
+    TrySpawnTrapperTrap = Symbol(
+        [0x11B94],
+        [0x22EDDD4],
+        None,
+        (
+            "If the flag for a trapper trap is set, handles spawning a trap based upon"
+            " the\ninformation inside the dungeon struct. Uses the entity for logging a"
+            " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
+            " true if a trap was spawned succesfully"
+        ),
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x1382C],
         [0x22EFA6C],
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -17013,14 +17119,25 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: target entity"
             " pointer\nr1: current_id\nreturn: ?"
         ),
     )
 
+    TryActivateTraceAndColorChange = Symbol(
+        [0x1D2B0],
+        [0x22F94F0],
+        None,
+        (
+            "Tries to activate the abilities trace and color change if possible. Called"
+            " after using\na move.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer\nr2: move pointer"
+        ),
+    )
+
     DefenderAbilityIsActive = Symbol(
         [0x1D48C, 0x257CC, 0x2E700, 0x35954, 0x46B24, 0x567CC],
         [0x22F96CC, 0x2301A0C, 0x230A940, 0x2311B94, 0x2322D64, 0x2332A0C],
         None,
         (
             "Checks if a defender has an active ability that isn't disabled by an"
             " attacker's Mold Breaker.\n\nThere are two versions of this function,"
@@ -17058,14 +17175,25 @@
         None,
         (
             "Checks if an entity is a monster (entity type 1).\n\nr0: entity"
             " pointer\nreturn: bool"
         ),
     )
 
+    TryActivateConversion2 = Symbol(
+        [0x1D504],
+        [0x22F9744],
+        None,
+        (
+            "Checks for the conversion2 status and applies the type change if"
+            " applicable. Called\nafter using a move.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr2: move pointer"
+        ),
+    )
+
     TryActivateTruant = Symbol(
         [0x1D5B0],
         [0x22F97F0],
         None,
         (
             "Checks if an entity has the ability Truant, and if so tries to apply the"
             " pause status to it.\n\nr0: pointer to entity"
@@ -18359,14 +18487,24 @@
             " spawn cooldown, it will try to spawn an enemy if the number of enemies is"
             " below the spawn cap.\n\nIf the spawn counter is greater than 900, it will"
             " instead perform the special spawn caused by the ability Illuminate.\n\nNo"
             " params."
         ),
     )
 
+    TryNonLeaderItemPickUp = Symbol(
+        [0x32F24],
+        [0x230F164],
+        None,
+        (
+            "Similar to TryLeaderItemPickUp, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: entity pointer"
+        ),
+    )
+
     AuraBowIsActive = Symbol(
         [0x33488],
         [0x230F6C8],
         None,
         (
             "Checks if a monster is holding an aura bow that isn't disabled by"
             " Klutz.\n\nr0: entity pointer\nreturn: bool"
@@ -19043,14 +19181,25 @@
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    MirrorMoveIsActive = Symbol(
+        [0x3D508],
+        [0x2319748],
+        None,
+        (
+            "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
+            " the effects is a status, 2 if it comes from an exclusive item, 0"
+            " otherwise.\n\nr0: pointer to entity\nreturn: int"
+        ),
+    )
+
     Conversion2IsActive = Symbol(
         [0x3D5D4],
         [0x2319814],
         None,
         (
             "Checks if the monster is under the effect of Conversion 2 (its type was"
             " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
@@ -19231,14 +19380,36 @@
             " item is sticky, or if the monster is under the STATUS_MUZZLED status and"
             " the item is edible.\nAlso prints failure messages if required.\n\nr0:"
             " Monster entity pointer\nr1: Item pointer\nreturn: True if the monster can"
             " use the item, false otherwise"
         ),
     )
 
+    ApplyGrimyFoodEffect = Symbol(
+        [0x412F4],
+        [0x231D534],
+        None,
+        (
+            "Randomly inflicts poison, shadow hold, burn, paralysis, or an offensive"
+            " stat debuff\nto the target. If the survivalist iq skill or gluttony"
+            " ability is active, the target\nhas a 50% chance not to be"
+            " affected.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyMixElixirEffect = Symbol(
+        [0x41440],
+        [0x231D680],
+        None,
+        (
+            "If the target monster is a Linoone, restores all the PP of all the"
+            " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         [0x42750],
         [0x231E990],
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -19328,14 +19499,39 @@
         (
             "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
             " target entity pointer\nr2: warp type\nr3: position (if warp type is"
             " position-based)"
         ),
     )
 
+    TryActivateNondamagingDefenderAbility = Symbol(
+        [0x45838],
+        [0x2321A78],
+        None,
+        (
+            "Applies the effects of a defender's ability on an attacker. After a move"
+            " is used,\nthis function is called to see if any of the bitflags for an"
+            " ability were set and\napplies the corresponding effect. (The way leech"
+            " seed removes certain statuses is\nalso handled here.)\n\nr0: entity"
+            " pointer"
+        ),
+    )
+
+    TryActivateNondamagingDefenderExclusiveItem = Symbol(
+        [0x45AB0],
+        [0x2321CF0],
+        None,
+        (
+            "Applies the effects of a defender's item on an attacker. After a move is"
+            " used,\nthis function is called to see if any of the bitflags for an item"
+            " were set and\napplies the corresponding effect.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer"
+        ),
+    )
+
     GetMoveRangeDistance = Symbol(
         [0x46064],
         [0x23222A4],
         None,
         (
             "Returns the maximum reach distance of a move, based on its AI range"
             " value.\n\nIf the move doesn't have an AI range value of RANGE_FRONT_10,"
@@ -19496,14 +19692,26 @@
         None,
         (
             "Gets the lower 2 bytes of a 4-byte number and interprets it as a signed"
             " short.\n\nr0: 4-byte number x\nreturn: (short) x"
         ),
     )
 
+    PlayMoveAnimation = Symbol(
+        [0x49474],
+        [0x23256B4],
+        None,
+        (
+            "Handles the process of getting and playing all the animations for a move."
+            " Waits\nuntil the animation has no more frames before returning.\n\nr0:"
+            " Pointer to the entity that used the move\nr1: Pointer to the entity that"
+            " is the target\nr2: Move pointer\nr3: position"
+        ),
+    )
+
     GetMoveAnimationId = Symbol(
         [0x498D0],
         [0x2325B10],
         None,
         (
             "Returns the move animation ID that should be played for a move.\nIt"
             " contains a check for weather ball. After that, if the parameter"
@@ -19659,14 +19867,27 @@
         (
             "Activates the Mud Sport or Water Sport condition on the dungeon floor for"
             " some number of turns.\n\nr0: water sport flag (false for Mud Sport, true"
             " for Water Sport)"
         ),
     )
 
+    TryActivateWeather = Symbol(
+        [0x59284],
+        [0x23354C4],
+        None,
+        (
+            "Tries to change the weather based upon the information for each weather"
+            " type in the\ndungeon struct. Returns whether the weather was succesfully"
+            " changed or not.\n\nr0: bool to not play the weather change"
+            " animation?\nr1: bool to force weather change? Like play the animation and"
+            " text for the weather?\nreturn: True if the weather changed"
+        ),
+    )
+
     DigitCount = Symbol(
         [0x59430],
         [0x2335670],
         None,
         (
             "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
             " negative, it is cast to a uint16_t before counting digits.\n\nr0:"
@@ -20860,14 +21081,25 @@
         None,
         (
             "Wrapper around GenerateItem with quantity set to 0 and stickiness type set"
             " to SPAWN_STICKY_NEVER.\n\nr0: pointer to item to initialize\nr1: item ID"
         ),
     )
 
+    TryLeaderItemPickUp = Symbol(
+        [0x68E18],
+        [0x2345058],
+        None,
+        (
+            "Checks the tile at the specified position and determines if the leader"
+            " should pick up an item.\n\nr0: position\nr1: flag for whether or not a"
+            " message should be logged upon the leader failing to obtain the item"
+        ),
+    )
+
     SpawnItem = Symbol(
         [0x692F8],
         [0x2345538],
         None,
         (
             "Spawns an item on the floor. Fails if there are more than 64 items already"
             " on the floor.\n\nThis calls SpawnItemEntity, fills in the item info"
@@ -22338,14 +22570,45 @@
             " is only used for the cardinal directions. The elements at odd indexes are"
             " unused and unconditionally set to 0.\n\nThis array is used by the dungeon"
             " generation algorithm when generating room imperfections. See"
             " GenerateRoomImperfections."
         ),
     )
 
+    GUMMI_LIKE_STRING_IDS = Symbol(
+        [0x77090],
+        [0x23532D0],
+        0x8,
+        (
+            "List that holds the message IDs for how much a monster liked a gummi in"
+            " decreasing order."
+        ),
+    )
+
+    GUMMI_IQ_STRING_IDS = Symbol(
+        [0x77090],
+        [0x23532D0],
+        0xA,
+        (
+            "List that holds the message IDs for how much a monster's IQ was raised by"
+            " in decreasing order."
+        ),
+    )
+
+    DAMAGE_STRING_IDS = Symbol(
+        [0x770F0],
+        [0x2353330],
+        0x36,
+        (
+            "List that matches the damage_message ID to their corresponding message ID."
+            " The null entry at 0xE in the middle is for hunger. The last entry is"
+            " null."
+        ),
+    )
+
     DUNGEON_PTR = Symbol(
         [0x772F8],
         [0x2353538],
         0x4,
         (
             "[Runtime] Pointer to the dungeon struct in dungeon mode.\n\nThis is a"
             " 'working copy' of DUNGEON_PTR_MASTER. The main dungeon engine uses this"
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -11817,14 +11817,20 @@
         None,
         None,
         "The chance of Steel Wing boosting defense, as a percentage (20%).",
     )
 
     GOLD_THORN_POWER = Symbol(None, None, None, "Attack power for Golden Thorns.")
 
+    BURN_DAMAGE = Symbol(None, None, None, "Damage dealt by the burn status condition.")
+
+    POISON_DAMAGE = Symbol(
+        None, None, None, "Damage dealt by the poison status condition."
+    )
+
     SPAWN_COOLDOWN = Symbol(
         None,
         None,
         None,
         "The number of turns between enemy spawns under normal conditions.",
     )
 
@@ -11988,14 +11994,28 @@
         ),
     )
 
     SONICBOOM_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by SonicBoom (20)."
     )
 
+    RAIN_ABILITY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is rain for the"
+            " abilities rain dish and dry skin."
+        ),
+    )
+
+    LEECH_SEED_HP_DRAIN = Symbol(
+        None, None, None, "The amount of health drained by leech seed status."
+    )
+
     EXCLUSIVE_ITEM_EXP_BOOST = Symbol(
         None,
         None,
         None,
         "The percentage increase in experience from exp-boosting exclusive items.",
     )
 
@@ -12069,14 +12089,24 @@
 
     STICK_POWER = Symbol(None, None, None, "Attack power for Sticks.")
 
     BUBBLE_LOWER_SPEED_CHANCE = Symbol(
         None, None, None, "The chance of Bubble lowering speed, as a percentage (10%)."
     )
 
+    ICE_BODY_BONUS_REGEN = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The passive bonus health regen given when the weather is hail for the"
+            " ability ice body."
+        ),
+    )
+
     POWDER_SNOW_FREEZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Powder Snow (and others, see DoMoveDamageFreeze15) freezing,"
             " as a percentage (15%)."
@@ -12103,14 +12133,24 @@
         ),
     )
 
     POISON_FANG_POISON_CHANCE = Symbol(
         None, None, None, "The chance of Poison Fang poisoning, as a percentage (30%)."
     )
 
+    WEATHER_MOVE_TURN_COUNT = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The number of turns the moves rain dance, hail, sandstorm, sunny day and"
+            " defog change the weather for. (3000)"
+        ),
+    )
+
     THUNDER_PARALYZE_CHANCE = Symbol(
         None,
         None,
         None,
         (
             "The chance of Thunder (and others, see DoMoveDamageParalyze20) paralyzing,"
             " as a percentage (20%)"
@@ -12229,14 +12269,18 @@
         ),
     )
 
     POISON_DAMAGE_COOLDOWN = Symbol(
         None, None, None, "The number of turns between passive poison damage."
     )
 
+    LEECH_SEED_DAMAGE_COOLDOWN = Symbol(
+        None, None, None, "The number of turns between leech seed health drain."
+    )
+
     GEO_PEBBLE_DAMAGE = Symbol(None, None, None, "Damage dealt by Geo Pebbles.")
 
     GRAVELEROCK_DAMAGE = Symbol(None, None, None, "Damage dealt by Gravelerocks.")
 
     RARE_FOSSIL_DAMAGE = Symbol(None, None, None, "Damage dealt by Rare Fossils.")
 
     GINSENG_CHANCE_3 = Symbol(
@@ -12257,14 +12301,18 @@
         None, None, None, "The permanent defense boost from ingesting an Iron."
     )
 
     CALCIUM_STAT_BOOST = Symbol(
         None, None, None, "The permanent special attack boost from ingesting a Calcium."
     )
 
+    WISH_BONUS_REGEN = Symbol(
+        None, None, None, "The passive bonus regen given by the wish status condition."
+    )
+
     DRAGON_RAGE_FIXED_DAMAGE = Symbol(
         None, None, None, "The amount of fixed damage dealt by Dragon Rage (30)."
     )
 
     CORSOLA_TWIG_POWER = Symbol(None, None, None, "Attack power for Corsola Twigs.")
 
     CACNEA_SPIKE_POWER = Symbol(None, None, None, "Attack power for Cacnea Spikes.")
@@ -12800,14 +12848,25 @@
         (
             "Maps each weather type (by index, see enum weather_id) to the"
             " corresponding Castform type and form.\n\ntype: struct"
             " castform_weather_attributes[8]"
         ),
     )
 
+    BAD_POISON_DAMAGE_TABLE = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Table for how much damage each tick of badly poisoned should deal. The"
+            " table is filled with 0x0006, but could use different values for each"
+            " entry."
+        ),
+    )
+
     TYPE_MATCHUP_COMBINATOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "Table of type matchup combinations.\n\nEach row corresponds to a single"
             " type matchup that results from combining two individual type matchups"
@@ -16247,14 +16306,53 @@
         (
             "A convenience wrapper around SpawnTrap and BindTrapToTile. Always passes 0"
             " for the team parameter (making it an enemy trap).\n\nr0: trap ID\nr1: x"
             " position\nr2: y position\nr3: flags\nstack[0]: visibility flag"
         ),
     )
 
+    PrepareTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Saves the relevant information in the dungeon struct to later place a trap"
+            " at the\nlocation of the entity. (Only called with trap ID 0x19"
+            " (TRAP_NONE), but could be used \nwith others).\n\nr0: entity pointer\nr1:"
+            " trap ID\nr2: team (see struct trap::team)"
+        ),
+    )
+
+    TrySpawnTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the a trap can be placed on the tile. If the trap ID is >="
+            " TRAP_NONE (the\nlast value for a trap), randomly select another trap"
+            " (except for wonder tile). After\n30 failed attempts to select a"
+            " non-wonder tile trap ID, default to chestnut trap.\nIf the checks pass,"
+            " spawn the trap.\n\nr0: position\nr1: trap ID\nr2: team (see struct"
+            " trap::team)\nr3: visibility flag\nreturn: true if a trap was spawned"
+            " succesfully"
+        ),
+    )
+
+    TrySpawnTrapperTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the flag for a trapper trap is set, handles spawning a trap based upon"
+            " the\ninformation inside the dungeon struct. Uses the entity for logging a"
+            " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
+            " true if a trap was spawned succesfully"
+        ),
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16490,14 +16588,25 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: target entity"
             " pointer\nr1: current_id\nreturn: ?"
         ),
     )
 
+    TryActivateTraceAndColorChange = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to activate the abilities trace and color change if possible. Called"
+            " after using\na move.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer\nr2: move pointer"
+        ),
+    )
+
     DefenderAbilityIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a defender has an active ability that isn't disabled by an"
             " attacker's Mold Breaker.\n\nThere are two versions of this function,"
@@ -16515,14 +16624,25 @@
         None,
         (
             "Checks if an entity is a monster (entity type 1).\n\nr0: entity"
             " pointer\nreturn: bool"
         ),
     )
 
+    TryActivateConversion2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks for the conversion2 status and applies the type change if"
+            " applicable. Called\nafter using a move.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr2: move pointer"
+        ),
+    )
+
     TryActivateTruant = Symbol(
         None,
         None,
         None,
         (
             "Checks if an entity has the ability Truant, and if so tries to apply the"
             " pause status to it.\n\nr0: pointer to entity"
@@ -17790,14 +17910,24 @@
             " spawn cooldown, it will try to spawn an enemy if the number of enemies is"
             " below the spawn cap.\n\nIf the spawn counter is greater than 900, it will"
             " instead perform the special spawn caused by the ability Illuminate.\n\nNo"
             " params."
         ),
     )
 
+    TryNonLeaderItemPickUp = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to TryLeaderItemPickUp, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: entity pointer"
+        ),
+    )
+
     AuraBowIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is holding an aura bow that isn't disabled by"
             " Klutz.\n\nr0: entity pointer\nreturn: bool"
@@ -18474,14 +18604,25 @@
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    MirrorMoveIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
+            " the effects is a status, 2 if it comes from an exclusive item, 0"
+            " otherwise.\n\nr0: pointer to entity\nreturn: int"
+        ),
+    )
+
     Conversion2IsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Conversion 2 (its type was"
             " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
@@ -18662,14 +18803,36 @@
             " item is sticky, or if the monster is under the STATUS_MUZZLED status and"
             " the item is edible.\nAlso prints failure messages if required.\n\nr0:"
             " Monster entity pointer\nr1: Item pointer\nreturn: True if the monster can"
             " use the item, false otherwise"
         ),
     )
 
+    ApplyGrimyFoodEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly inflicts poison, shadow hold, burn, paralysis, or an offensive"
+            " stat debuff\nto the target. If the survivalist iq skill or gluttony"
+            " ability is active, the target\nhas a 50% chance not to be"
+            " affected.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyMixElixirEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a Linoone, restores all the PP of all the"
+            " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -18759,14 +18922,39 @@
         (
             "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
             " target entity pointer\nr2: warp type\nr3: position (if warp type is"
             " position-based)"
         ),
     )
 
+    TryActivateNondamagingDefenderAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's ability on an attacker. After a move"
+            " is used,\nthis function is called to see if any of the bitflags for an"
+            " ability were set and\napplies the corresponding effect. (The way leech"
+            " seed removes certain statuses is\nalso handled here.)\n\nr0: entity"
+            " pointer"
+        ),
+    )
+
+    TryActivateNondamagingDefenderExclusiveItem = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the effects of a defender's item on an attacker. After a move is"
+            " used,\nthis function is called to see if any of the bitflags for an item"
+            " were set and\napplies the corresponding effect.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer"
+        ),
+    )
+
     GetMoveRangeDistance = Symbol(
         None,
         None,
         None,
         (
             "Returns the maximum reach distance of a move, based on its AI range"
             " value.\n\nIf the move doesn't have an AI range value of RANGE_FRONT_10,"
@@ -18927,14 +19115,26 @@
         None,
         (
             "Gets the lower 2 bytes of a 4-byte number and interprets it as a signed"
             " short.\n\nr0: 4-byte number x\nreturn: (short) x"
         ),
     )
 
+    PlayMoveAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Handles the process of getting and playing all the animations for a move."
+            " Waits\nuntil the animation has no more frames before returning.\n\nr0:"
+            " Pointer to the entity that used the move\nr1: Pointer to the entity that"
+            " is the target\nr2: Move pointer\nr3: position"
+        ),
+    )
+
     GetMoveAnimationId = Symbol(
         None,
         None,
         None,
         (
             "Returns the move animation ID that should be played for a move.\nIt"
             " contains a check for weather ball. After that, if the parameter"
@@ -19090,14 +19290,27 @@
         (
             "Activates the Mud Sport or Water Sport condition on the dungeon floor for"
             " some number of turns.\n\nr0: water sport flag (false for Mud Sport, true"
             " for Water Sport)"
         ),
     )
 
+    TryActivateWeather = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to change the weather based upon the information for each weather"
+            " type in the\ndungeon struct. Returns whether the weather was succesfully"
+            " changed or not.\n\nr0: bool to not play the weather change"
+            " animation?\nr1: bool to force weather change? Like play the animation and"
+            " text for the weather?\nreturn: True if the weather changed"
+        ),
+    )
+
     DigitCount = Symbol(
         None,
         None,
         None,
         (
             "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
             " negative, it is cast to a uint16_t before counting digits.\n\nr0:"
@@ -20276,14 +20489,25 @@
         None,
         (
             "Wrapper around GenerateItem with quantity set to 0 and stickiness type set"
             " to SPAWN_STICKY_NEVER.\n\nr0: pointer to item to initialize\nr1: item ID"
         ),
     )
 
+    TryLeaderItemPickUp = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile at the specified position and determines if the leader"
+            " should pick up an item.\n\nr0: position\nr1: flag for whether or not a"
+            " message should be logged upon the leader failing to obtain the item"
+        ),
+    )
+
     SpawnItem = Symbol(
         None,
         None,
         None,
         (
             "Spawns an item on the floor. Fails if there are more than 64 items already"
             " on the floor.\n\nThis calls SpawnItemEntity, fills in the item info"
@@ -21634,14 +21858,45 @@
             " is only used for the cardinal directions. The elements at odd indexes are"
             " unused and unconditionally set to 0.\n\nThis array is used by the dungeon"
             " generation algorithm when generating room imperfections. See"
             " GenerateRoomImperfections."
         ),
     )
 
+    GUMMI_LIKE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster liked a gummi in"
+            " decreasing order."
+        ),
+    )
+
+    GUMMI_IQ_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that holds the message IDs for how much a monster's IQ was raised by"
+            " in decreasing order."
+        ),
+    )
+
+    DAMAGE_STRING_IDS = Symbol(
+        None,
+        None,
+        None,
+        (
+            "List that matches the damage_message ID to their corresponding message ID."
+            " The null entry at 0xE in the middle is for hunger. The last entry is"
+            " null."
+        ),
+    )
+
     DUNGEON_PTR = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Pointer to the dungeon struct in dungeon mode.\n\nThis is a"
             " 'working copy' of DUNGEON_PTR_MASTER. The main dungeon engine uses this"
```

## pmdsky_debug_py/protocol.py

```diff
@@ -6506,14 +6506,24 @@
     ]
 
     GOLD_THORN_POWER: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    BURN_DAMAGE: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    POISON_DAMAGE: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     SPAWN_COOLDOWN: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     MIST_BALL_LOWER_SPECIAL_ATTACK_CHANCE: Symbol[
         Optional[List[int]],
@@ -6621,14 +6631,24 @@
     ]
 
     SONICBOOM_FIXED_DAMAGE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    RAIN_ABILITY_BONUS_REGEN: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    LEECH_SEED_HP_DRAIN: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     EXCLUSIVE_ITEM_EXP_BOOST: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     AFTERMATH_CHANCE: Symbol[
         Optional[List[int]],
@@ -6691,14 +6711,19 @@
     ]
 
     BUBBLE_LOWER_SPEED_CHANCE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    ICE_BODY_BONUS_REGEN: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     POWDER_SNOW_FREEZE_CHANCE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     POISON_STING_POISON_CHANCE: Symbol[
         Optional[List[int]],
@@ -6711,14 +6736,19 @@
     ]
 
     POISON_FANG_POISON_CHANCE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    WEATHER_MOVE_TURN_COUNT: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     THUNDER_PARALYZE_CHANCE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     THUNDERBOLT_PARALYZE_CHANCE: Symbol[
         Optional[List[int]],
@@ -6786,14 +6816,19 @@
     ]
 
     POISON_DAMAGE_COOLDOWN: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    LEECH_SEED_DAMAGE_COOLDOWN: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     GEO_PEBBLE_DAMAGE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     GRAVELEROCK_DAMAGE: Symbol[
         Optional[List[int]],
@@ -6821,14 +6856,19 @@
     ]
 
     CALCIUM_STAT_BOOST: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    WISH_BONUS_REGEN: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     DRAGON_RAGE_FIXED_DAMAGE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     CORSOLA_TWIG_POWER: Symbol[
         Optional[List[int]],
@@ -7106,14 +7146,19 @@
     ]
 
     CASTFORM_WEATHER_ATTRIBUTE_TABLE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    BAD_POISON_DAMAGE_TABLE: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     TYPE_MATCHUP_COMBINATOR_TABLE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     OFFENSIVE_STAT_STAGE_MULTIPLIERS: Symbol[
         Optional[List[int]],
@@ -9790,14 +9835,29 @@
     ]
 
     SpawnEnemyTrapAtPos: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    PrepareTrapperTrap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TrySpawnTrap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TrySpawnTrapperTrap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DebugRecruitingEnabled: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsSecretBazaarNpcBehavior: Symbol[
         Optional[List[int]],
@@ -9910,24 +9970,34 @@
     ]
 
     GetMonsterApparentId: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryActivateTraceAndColorChange: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DefenderAbilityIsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsMonster: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryActivateConversion2: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryActivateTruant: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryPointCameraToMonster: Symbol[
         Optional[List[int]],
@@ -10440,14 +10510,19 @@
     ]
 
     TrySpawnMonsterAndTickSpawnCounter: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryNonLeaderItemPickUp: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     AuraBowIsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ExclusiveItemOffenseBoost: Symbol[
         Optional[List[int]],
@@ -10740,14 +10815,19 @@
     ]
 
     HasConditionalGroundImmunity: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    MirrorMoveIsActive: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     Conversion2IsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     AiConsiderMove: Symbol[
         Optional[List[int]],
@@ -10815,14 +10895,24 @@
     ]
 
     CanMonsterUseItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ApplyGrimyFoodEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyMixElixirEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ShouldTryEatItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetMaxPpWrapper: Symbol[
         Optional[List[int]],
@@ -10860,14 +10950,24 @@
     ]
 
     TryWarp: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryActivateNondamagingDefenderAbility: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryActivateNondamagingDefenderExclusiveItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetMoveRangeDistance: Symbol[
         Optional[List[int]],
         None,
     ]
 
     MoveHitCheck: Symbol[
         Optional[List[int]],
@@ -10925,14 +11025,19 @@
     ]
 
     LowerSshort: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    PlayMoveAnimation: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetMoveAnimationId: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ShouldMovePlayAlternativeAnimation: Symbol[
         Optional[List[int]],
@@ -10990,14 +11095,19 @@
     ]
 
     ActivateSportCondition: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryActivateWeather: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DigitCount: Symbol[
         Optional[List[int]],
         None,
     ]
 
     LoadTextureUi: Symbol[
         Optional[List[int]],
@@ -11500,14 +11610,19 @@
     ]
 
     GenerateCleanItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryLeaderItemPickUp: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SpawnItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SpawnEnemyItemDropWrapper: Symbol[
         Optional[List[int]],
@@ -12197,14 +12312,29 @@
     ]
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    GUMMI_LIKE_STRING_IDS: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    GUMMI_IQ_STRING_IDS: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    DAMAGE_STRING_IDS: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     DUNGEON_PTR: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     DUNGEON_PTR_MASTER: Symbol[
         Optional[List[int]],
```

## Comparing `pmdsky_debug_py-5.1.8.dist-info/METADATA` & `pmdsky_debug_py-5.1.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 5.1.8
+Version: 5.1.9
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `pmdsky_debug_py-5.1.8.dist-info/RECORD` & `pmdsky_debug_py-5.1.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pmdsky_debug_py/__init__.py,sha256=xvXjdxEqeoQaaS6ssZYVI9jARzv5M4q6FNwA3Z6fOw4,1831
-pmdsky_debug_py/_release.py,sha256=pgqHIl7_d-eyAN83PFsd2fsum5yGnA8KA_c0vclxj_I,30
-pmdsky_debug_py/eu.py,sha256=BvqMoeBwfCdIv4E2XxaAeWb_ZkNaR87_FUqByV4nstU,712779
-pmdsky_debug_py/eu_itcm.py,sha256=m-wDusWIwldVjPsIa7rP1k7rPn8u-bRDzvsQSfFf3U8,680684
-pmdsky_debug_py/jp.py,sha256=_Daiyf-xOTTFl3ETCwY50AV4vrZ2ljpZwPN2MBBkHBs,701749
-pmdsky_debug_py/jp_itcm.py,sha256=lgJgdOeLv5o2CeXC_mZiSouZOXNb07KvR8fVDmjeQ9o,680684
-pmdsky_debug_py/na.py,sha256=iqBP3871Ibzk3KjOAtgTzsY59SsO94vKOgp5O7AG-MI,718907
-pmdsky_debug_py/na_itcm.py,sha256=KqitEPvDBjarv9Dj-Hm-xrBxWjad13sRkAFkSJNlGB4,680695
-pmdsky_debug_py/protocol.py,sha256=YeFJPK2tMYyLqAZDAOcQJChU3Z6gCAN9Z9ACnDBOz1g,227398
+pmdsky_debug_py/_release.py,sha256=RRvJyKve18mHezvdHNJgqVhVKq4QDEzCKFtOEQQQTkQ,30
+pmdsky_debug_py/eu.py,sha256=F2VBVDDFNoPeue5HBZtLTohEQWKWg1uikkwmaB2CVVU,720789
+pmdsky_debug_py/eu_itcm.py,sha256=zU3uXb5oQtDk_ixamX0prakF9_wNAdGieQHlyeQGjmk,688659
+pmdsky_debug_py/jp.py,sha256=Ea76A1rIJ0B0dNSZWL5aGk-ROLPB6LGES6-1dSv_CSk,709748
+pmdsky_debug_py/jp_itcm.py,sha256=dNT3uroNQ4voG-ukv7XXfnW9DLg7Qzlxkn7uI8TEcIk,688659
+pmdsky_debug_py/na.py,sha256=RHe_4CH5E8Hi7TOH1xXNrzwbCMOFzogB1CnuKFmLe3s,727240
+pmdsky_debug_py/na_itcm.py,sha256=X_0NnKVOz0dZKTTDszepvDpiJV0XacpmvAfPf1vpDKo,688670
+pmdsky_debug_py/protocol.py,sha256=gQYpA5oJdojDGnoEfvc-F0Kt6ePHVDWrSNvRQf9eCE8,229717
 pmdsky_debug_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pmdsky_debug_py-5.1.8.dist-info/METADATA,sha256=Nj-b7C9XLNqXMerNxFeLZAj5A7lb2H8RBtJPZu-Wyvc,1320
-pmdsky_debug_py-5.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pmdsky_debug_py-5.1.8.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
-pmdsky_debug_py-5.1.8.dist-info/RECORD,,
+pmdsky_debug_py-5.1.9.dist-info/METADATA,sha256=w2920XQs4Eq8v7oImTw5yYEvUV8vHtBcGr7fe7sUkdQ,1320
+pmdsky_debug_py-5.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pmdsky_debug_py-5.1.9.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
+pmdsky_debug_py-5.1.9.dist-info/RECORD,,
```

