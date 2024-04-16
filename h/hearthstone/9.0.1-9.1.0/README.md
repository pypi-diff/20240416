# Comparing `tmp/hearthstone-9.0.1.tar.gz` & `tmp/hearthstone-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-9.0.1.tar", last modified: Fri Apr 12 10:05:53 2024, max compression
+gzip compressed data, was "hearthstone-9.1.0.tar", last modified: Tue Apr 16 15:05:14 2024, max compression
```

## Comparing `hearthstone-9.0.1.tar` & `hearthstone-9.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:05:53.316491 hearthstone-9.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 10:05:49.000000 hearthstone-9.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 10:05:53.316491 hearthstone-9.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-12 10:05:49.000000 hearthstone-9.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:05:53.312491 hearthstone-9.0.1/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    60212 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:05:53.316491 hearthstone-9.0.1/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-12 10:05:49.000000 hearthstone-9.0.1/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:05:53.312491 hearthstone-9.0.1/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 10:05:53.000000 hearthstone-9.0.1/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 10:05:53.000000 hearthstone-9.0.1/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:05:53.000000 hearthstone-9.0.1/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 10:05:53.000000 hearthstone-9.0.1/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 10:05:53.000000 hearthstone-9.0.1/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:05:53.000000 hearthstone-9.0.1/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-12 10:05:53.316491 hearthstone-9.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-12 10:05:49.000000 hearthstone-9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 15:05:08.000000 hearthstone-9.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-16 15:05:14.468963 hearthstone-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-16 15:05:08.000000 hearthstone-9.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61527 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 15:05:08.000000 hearthstone-9.1.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:05:14.468963 hearthstone-9.1.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:05:14.000000 hearthstone-9.1.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-16 15:05:14.468963 hearthstone-9.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-16 15:05:08.000000 hearthstone-9.1.0/setup.py
```

### Comparing `hearthstone-9.0.1/LICENSE` & `hearthstone-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/PKG-INFO` & `hearthstone-9.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.0.1
+Version: 9.1.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-9.0.1/README.md` & `hearthstone-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/bountyxml.py` & `hearthstone-9.1.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/cardxml.py` & `hearthstone-9.1.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/dbf.py` & `hearthstone-9.1.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/deckstrings.py` & `hearthstone-9.1.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/entities.py` & `hearthstone-9.1.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/enums.py` & `hearthstone-9.1.0/hearthstone/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,15 +155,14 @@
 	AFFECTED_BY_SPELL_POWER = 370
 	EXTRA_MINION_DEATHRATTLES_BASE = 371
 	START_WITH_1_HEALTH = 372
 	IMMUNE_WHILE_ATTACKING = 373
 	MULTIPLY_HERO_DAMAGE = 374
 	MULTIPLY_BUFF_VALUE = 375
 	CUSTOM_KEYWORD_EFFECT = 376
-	TOPDECK = 377
 	CANT_BE_TARGETED_BY_BATTLECRIES = 379
 	HERO_POWER = 380
 	DEATHRATTLE_RETURN_ZONE = 382
 	STEADY_SHOT_CAN_TARGET = 383
 	DISPLAYED_CREATOR = 385
 	POWERED_UP = 386
 	SPARE_PART = 388
@@ -463,14 +462,15 @@
 	BATTLEGROUNDS_PREMIUM_EMOTES = 1463
 	MOVE_MINION_HOVER_TARGET_SLOT = 1464
 	BACON_COIN_ON_ENEMY_MINIONS = 1467
 	BACON_TRIPLED_BASE_MINION_ID = 1471
 	ALWAYS_USE_FAST_ACTOR_TRIGGERS = 1473
 	BACON_HERO_CAN_BE_DRAFTED = 1491
 	TRANSIENT_ENTITY = 1493
+	BACON_MAX_PLAYER_TECH_LEVEL = 1494
 	DISABLE_NONHERO_GOLDEN_ANIMATIONS = 1514
 	WATERMARK_OVERRIDE_CARD_SET = 1517
 	DORMANT = 1518
 	DORMANT_AWAKEN_CONDITION_ENCHANT = 1519
 	SUPPRESS_SUMMON_VO_FOR_PLAYER = 1521
 	CORRUPT = 1524
 	ALLOW_GAME_SPEEDUP = 1526
@@ -683,14 +683,15 @@
 	LETTUCE_ELVES = 2322
 	OBJECTIVE_AURA = 2329
 	DREDGE = 2332
 	CURRENT_HEALING_POWER = 2333
 	EARLY_CONCEDE_POPUP_AVAILABLE = 2340
 	BACON_PLAYER_NUM_HERO_BUDDIES_GAINED = 2346
 	BATTLEGROUNDS_FAVORITE_FINISHER = 2348
+	DAMAGE_DEALT_TO_HERO_LAST_TURN = 2349
 	LOCATION_ACTION_COST = 2352
 	LOCATION_ACTION_COOLDOWN = 2353
 	WHELP = 2355
 	BACON_SPELLCRAFT_ID = 2359
 	BACON_HERO_BUDDY_PROGRESS = 2364
 	REVIVE = 2369
 	BACON_HEROPOWER_BASE_HERO_ID = 2376
@@ -797,71 +798,92 @@
 	TAG_SCRIPT_DATA_NUM_6 = 2921
 	DECK_SWAP_ACTIVE = 2929
 	MAX_SIDEBOARD_CARDS = 2931
 	BONUS_EFFECTS = 2934
 	BACON_USE_COIN_BASED_BUDDY_METER = 2935
 	BACON_BUY_BUDDY = 2937
 	BACON_BUY_BUDDY_2 = 2938
+	BACON_DUO_TEAMMATE_PLAYER_ID = 2939
 	BACON_SHOW_HEROPOWER_BUDDY_AS_EVOLVING_BIG_CARD = 2943
 	HIDDEN_CHOICE_OVERRIDE = 2946
+	BACON_DUO_PLAYER_FIGHTS_FIRST_NEXT_COMBAT = 2975
+	NEXT_OPPONENT_TEAMMATE_PLAYER_ID = 2988
+	BACON_CURRENT_COMBAT_PLAYER_ID = 2989
 	FORGED = 3011
 	BUILDING_UP = 3016
 	BACON_PAIR_CANDIDATE = 3031
 	CTHUN_TAUNT_BUFF = 3034
 	BACON_TRIGGER_UPBEAT = 3046
 	BACON_TRIGGER_XY = 3047
+	BACON_COMBAT_PHASE_HERO = 3048
 	FAN_LINK = 3052
 	CTHUN_HEALTH_BUFF = 3053
 	CTHUN_ATTACK_BUFF = 3054
 	FORGE_REVEALED = 3070
 	FORGES_INTO = 3074
 	FX_DATANUM_2 = 3077
 	RITUALIST_MINION = 3078
+	SUPPRES_ALL_SOUNDS_FOR_ENTITY = 3093
+	BACON_DUO_TEAM_ID = 3095
 	FX_DATANUM_3 = 3109
 	ALLOW_MOVE_BACON_SPELL = 3111
 	EXCAVATE = 3114
 	SUMMONED_WHEN_DRAWN = 3128
 	IS_ALTERNATE_HEROPOWER = 3130
 	TITAN_ABILITY_USED_1 = 3140
 	TITAN_ABILITY_USED_2 = 3141
 	TITAN_ABILITY_USED_3 = 3142
+	BACON_DUO_TRIPLE_CANDIDATE_TEAMMATE = 3145
+	BACON_DUO_PAIR_CANDIDATE_TEAMMATE = 3146
+	BACON_DUO_PASSABLE = 3178
 	ANOMALY1 = 3182
 	ANOMALY2 = 3183
+	IS_USING_PASS_OPTION = 3185
 	TUTORIAL_TARGET_OPPONENT_ANIM = 3192
 	TUTORIAL_TARGET_MINION_ANIM = 3193
 	TUTORIAL_PLAY_MINION_ANIM = 3195
 	TUTORIAL_HERO_POWER_TARGET_MINION_ANIM = 3196
 	TUTORIAL_HERO_POWER_TARGET_OPPONENT_ANIM = 3197
 	SUPPRESS_EVIL_TWIN_MUSTACHE_SOUND = 3198
 	HERO_DOESNT_MOVE_ON_ATTACK = 3211
 	CURRENT_EXCAVATE_TIER = 3249
+	BACON_CONSUME_TOOLTIP = 3254
 	ALONE_RANGER = 3258
 	CUTSCENE_CARD_TYPE = 3265
 	MINIATURIZE = 3318
 	MINI = 3319
+	BACON_PASS_TOOLTIP = 3321
 	MAX_EXCAVATE_TIER = 3326
 	PALADIN_AURA = 3374
 	ZILLIAX_CUSTOMIZABLE_COSMETICMODULE = 3376
 	ZILLIAX_CUSTOMIZABLE_FUNCTIONALMODULE = 3377
+	BACON_COMBAT_DAMAGE_CAP_ENABLED = 3403
 	SIDEBOARD_TYPE = 3427
 	CREATED_BY_TWINSPELL = 3432
 	CREATED_BY_MINIATURIZE = 3433
 	SUPPRESS_HERO_STANDARD_SUMMON_FX = 3438
 	ZILLIAX_CUSTOMIZABLE_LINKED_COSMETICMOUDLE = 3450
 	MIN_SIDEBOARD_CARDS = 3459
 	FORGETFUL_ATTACK_VISUAL = 3460
 	SHUDDERWOCKHIGHLIGHTHINT = 3463
+	HERO_FRAME_TYPE = 3495
 	NUM_TURNS_LAST_AFFECTED_BY = 3464
 	EXTRA_TURNS_SPELL_OVERRIDE = 3465
 	ZILLIAX_CUSTOMIZABLE_LINKED_FUNCTIONALMOUDLE = 3470
 	HIDE_HEALTH_NUMBER = 3471
 	HIDE_ATTACK_NUMBER = 3472
 	ZILLIAX_CUSTOMIZABLE_SAVED_VERSION = 3477
+	DUOS_QUEUED_NOT_ON_TEAM = 3478
+	PLAYER_ABANDONED_BY_TEAMMATE = 3480
 	SUPPRESS_MILL_ANIMATION = 3481
 	IGNORE_SUPPRESS_MILL_ANIMATION = 3482
+	BACON_TEAMMATE_BONUS_MINION_DAMAGE_LAST_COMBAT = 3492
+	BACON_DUOS_PUNISH_LEAVERS = 3494
+	BACON_TRIPLED_BASE_MINION_ID2 = 3499
+	BACON_TRIPLED_BASE_MINION_ID3 = 3500
 
 	InvisibleDeathrattle = 335
 	ImmuneToSpellpower = 349
 	AttackVisualType = 251
 	DevState = 268
 	GrantCharge = 355
 	HealTarget = 361
@@ -988,14 +1010,15 @@
 	EXTRA_OVERLOAD_SPELL_CASTS_BASE = 1272
 	EXTRA_SPELL_CASTS_ADDITIONAL = 1348
 	BACON_MINION_IS_LEVEL_TWO = 1421
 	PIECE_OF_CTHUN = 1477
 	AVFACTION = 2323
 	AVRANK = 2324
 	MERCS_DISCOVER = 2665
+	TOPDECK = 377
 
 	# Missing/guessed, only present in logs
 	WEAPON = 334
 	DISCARD_CARDS = 890
 	BATTLEGROUNDS_HERO_ARMOR_TIER = 1723
 	BATTLEGROUNDS_DARKMOON_PRIZE_TURN = 1735
 
@@ -1539,14 +1562,18 @@
 	BGT_RANKED_CLASSIC = 58
 	BGT_CASUAL_CLASSIC = 59
 	BGT_MERCENARIES_PVE_COOP = 60
 	BGT_MERCENARIES_FRIENDLY = 61
 	BGT_BATTLEGROUNDS_PLAYER_VS_AI = 62,
 	BGT_RANKED_TWIST = 63,
 	BGT_CASUAL_TWIST = 64,
+	BGT_BATTLEGROUNDS_DUO = 65
+	BGT_BATTLEGROUNDS_DUO_VS_AI = 66
+	BGT_BATTLEGROUNDS_DUO_FRIENDLY = 67
+	BGT_CASUAL_STANDARD_APPRENTICE = 68
 	# BGT_LAST = 65
 
 	BGT_NEWBIE = BGT_CASUAL_STANDARD_NEWBIE
 	BGT_CASUAL_STANDARD = BGT_CASUAL_STANDARD_NORMAL
 
 	BGT_RESERVED_18_22 = BGT_MERCENARIES_PVP
 	BGT_RESERVED_18_23 = BGT_MERCENARIES_PVE
@@ -1620,16 +1647,19 @@
 	GT_PVPDR = 29
 	GT_MERCENARIES_PVP = 30
 	GT_MERCENARIES_PVE = 31
 	GT_MERCENARIES_PVE_COOP = 32
 	GT_MERCENARIES_AI_VS_AI = 33
 	GT_MERCENARIES_FRIENDLY = 34
 	GT_BATTLEGROUNDS_AI_VS_AI = 35
-
-	# GT_LAST = 35
+	GT_BATTLEGROUNDS_PLAYER_VS_AI = 36
+	GT_BATTLEGROUNDS_DUO = 37
+	GT_BATTLEGROUNDS_DUO_VS_AI = 38
+	GT_BATTLEGROUNDS_DUO_FRIENDLY = 39
+	GT_BATTLEGROUNDS_DUO_AI_VS_AI = 4
 
 	# Renamed
 	GT_TEST = GT_TEST_AI_VS_AI
 
 	# Removed
 	# GT_TOURNAMENT = 23
 	# GT_RESERVED_18_22 = 26
@@ -1677,15 +1707,17 @@
 			GameType.GT_BATTLEGROUNDS_FRIENDLY: BnetGameType.BGT_BATTLEGROUNDS_FRIENDLY,
 			GameType.GT_PVPDR_PAID: BnetGameType.BGT_PVPDR_PAID,
 			GameType.GT_PVPDR: BnetGameType.BGT_PVPDR,
 			GameType.GT_MERCENARIES_PVP: BnetGameType.BGT_MERCENARIES_PVP,
 			GameType.GT_MERCENARIES_PVE: BnetGameType.BGT_MERCENARIES_PVE,
 			GameType.GT_MERCENARIES_PVE_COOP: BnetGameType.BGT_MERCENARIES_PVE_COOP,
 			GameType.GT_MERCENARIES_FRIENDLY: BnetGameType.BGT_MERCENARIES_FRIENDLY,
-			# GameType.GT_LAST: BnetGameType.BGT_LAST,
+			GameType.GT_BATTLEGROUNDS_DUO: BnetGameType.BGT_BATTLEGROUNDS_DUO,
+			GameType.GT_BATTLEGROUNDS_DUO_VS_AI: BnetGameType.BGT_BATTLEGROUNDS_DUO_VS_AI,
+			GameType.GT_BATTLEGROUNDS_DUO_FRIENDLY: BnetGameType.BGT_BATTLEGROUNDS_DUO_FRIENDLY,
 		}[self]
 
 	@property
 	def is_fireside(self):
 		return self.name.startswith("GT_FSG_")
 
 	@property
```

### Comparing `hearthstone-9.0.1/hearthstone/mercenaryxml.py` & `hearthstone-9.1.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/stringsfile.py` & `hearthstone-9.1.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/utils/__init__.py` & `hearthstone-9.1.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone/xmlutils.py` & `hearthstone-9.1.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/hearthstone.egg-info/PKG-INFO` & `hearthstone-9.1.0/hearthstone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.0.1
+Version: 9.1.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-9.0.1/hearthstone.egg-info/SOURCES.txt` & `hearthstone-9.1.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-9.0.1/setup.cfg` & `hearthstone-9.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 9.0.1
+version = 9.1.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

