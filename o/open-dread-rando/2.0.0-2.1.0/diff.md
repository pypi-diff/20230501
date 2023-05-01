# Comparing `tmp/open-dread-rando-2.0.0.tar.gz` & `tmp/open-dread-rando-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-dread-rando-2.0.0.tar", last modified: Fri Apr 28 11:56:53 2023, max compression
+gzip compressed data, was "open-dread-rando-2.1.0.tar", last modified: Mon May  1 09:08:38 2023, max compression
```

## Comparing `open-dread-rando-2.0.0.tar` & `open-dread-rando-2.1.0.tar`

### file list

```diff
@@ -1,190 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.294380 open-dread-rando-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.278379 open-dread-rando-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/.github/workflows/patch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.278379 open-dread-rando-2.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-28 11:56:53.294380 open-dread-rando-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.282379 open-dread-rando-2.0.0/open_dread_rando/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.282379 open-dread-rando-2.0.0/open_dread_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/custom_door_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/door_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/dread_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/elevator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/environmental_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/environmental_damage_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/exefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.282379 open-dread-rando-2.0.0/open_dread_rando/files/
--rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/custom_scenario.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.282379 open-dread-rando-2.0.0/open_dread_rando/files/dread_depackager/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/dread_depackager/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/dread_depackager/main.npdm
--rw-r--r--   0 runner    (1001) docker     (123)   190028 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/dread_depackager/subsdk9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.282379 open-dread-rando-2.0.0/open_dread_rando/files/exefs_patches/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/exefs_patches/debug_input.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s010_cave.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s020_magma.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s030_baselab.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s040_aqua.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s050_forest.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s060_quarantine.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s070_basesanc.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s080_shipyard.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/levels/s090_skybase.lc.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/bit.lua
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/data_structures.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/death_counter.lua
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/input_handling.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/msemenu_mainmenu.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/randomizer_powerup.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.270378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.286380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.274378 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/system/minimap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.290380 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/system/minimap/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   423525 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/lua_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/model_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/output_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/patcher_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/pickup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/static_fixes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.294380 open-dread-rando-2.0.0/open_dread_rando/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/boss_powerup_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/custom_core_x.lua
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/randomizer_progressive_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/template_doorshield_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/templates/template_shieldenergy_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/tilegroup_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/open_dread_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.282379 open-dread-rando-2.0.0/open_dread_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:56:43.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 11:56:53.000000 open-dread-rando-2.0.0/open_dread_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-28 11:56:53.294380 open-dread-rando-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.294380 open-dread-rando-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:56:53.294380 open-dread-rando-2.0.0/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)   145222 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/tests/test_lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 11:56:30.000000 open-dread-rando-2.0.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.730997 open-dread-rando-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/.github/workflows/patch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.730997 open-dread-rando-2.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.734997 open-dread-rando-2.1.0/open_dread_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.734997 open-dread-rando-2.1.0/open_dread_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/custom_door_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/door_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/dread_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/elevator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/environmental_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/environmental_damage_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/exefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.734997 open-dread-rando-2.1.0/open_dread_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/custom_scenario.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.734997 open-dread-rando-2.1.0/open_dread_rando/files/dread_depackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/dread_depackager/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/dread_depackager/main.npdm
+-rw-r--r--   0 runner    (1001) docker     (123)   190028 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/dread_depackager/subsdk9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.734997 open-dread-rando-2.1.0/open_dread_rando/files/exefs_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/exefs_patches/debug_input.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s010_cave.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s020_magma.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s030_baselab.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s040_aqua.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s050_forest.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s060_quarantine.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s070_basesanc.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s080_shipyard.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/levels/s090_skybase.lc.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/bit.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/data_structures.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/death_counter.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/input_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/msemenu_mainmenu.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/randomizer_powerup.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.738997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.722997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.742997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.726997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/system/minimap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/system/minimap/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   423525 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/lua_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/patcher_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/static_fixes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/open_dread_rando/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/boss_powerup_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/custom_core_x.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/randomizer_progressive_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/template_doorshield_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/templates/template_shieldenergy_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/tilegroup_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/open_dread_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.734997 open-dread-rando-2.1.0/open_dread_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:08:29.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 09:08:38.000000 open-dread-rando-2.1.0/open_dread_rando.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-01 09:08:38.750997 open-dread-rando-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:08:38.746997 open-dread-rando-2.1.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/tests/test_files/randomizer_progressive_expected.lua
+-rw-r--r--   0 runner    (1001) docker     (123)   153802 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/tests/test_lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-01 09:08:11.000000 open-dread-rando-2.1.0/tests/test_schema.py
```

### Comparing `open-dread-rando-2.0.0/.github/dependabot.yml` & `open-dread-rando-2.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/.github/workflows/patch.yml` & `open-dread-rando-2.1.0/.github/workflows/patch.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/.github/workflows/python.yml` & `open-dread-rando-2.1.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/.gitignore` & `open-dread-rando-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/LICENSE` & `open-dread-rando-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/PKG-INFO` & `open-dread-rando-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.0.0
+Version: 2.1.0
 Summary: An open source randomizer patcher for Metroid Dread.
 Home-page: https://github.com/randovania/open-dread-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `open-dread-rando-2.0.0/README.md` & `open-dread-rando-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/cli.py` & `open-dread-rando-2.1.0/open_dread_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/cosmetic_patches.py` & `open-dread-rando-2.1.0/open_dread_rando/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/custom_door_types.py` & `open-dread-rando-2.1.0/open_dread_rando/custom_door_types.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/door_patcher.py` & `open-dread-rando-2.1.0/open_dread_rando/door_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/dread_patcher.py` & `open-dread-rando-2.1.0/open_dread_rando/dread_patcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,24 +100,24 @@
 
     replacement.update(configuration.get("game_patches", {}))
 
     return lua_util.replace_lua_template("custom_init.lua", replacement)
 
 def create_collision_camera_table(editor: PatcherEditor, configuration: dict):
     py_dict: dict = configuration["cosmetic_patches"]["lua"]["camera_names_dict"]
-    
+
     file = lua_util.replace_lua_template("cc_to_room_name.lua", { "room_dict" : py_dict}, True).encode("ascii")
     editor.add_new_asset("system/scripts/cc_to_room_name.lc", file, ["packs/system/system.pkg"])
 
 def patch_pickups(editor: PatcherEditor, lua_scripts: LuaEditor, pickups_config: list[dict], configuration: dict):
     # add to the TOC
     editor.add_new_asset("actors/items/randomizer_powerup/scripts/randomizer_powerup.lc", b'', [])
 
     for i, pickup in enumerate(pickups_config):
-        LOG.debug("Writing pickup %d: %s", i, pickup["resources"][0]["item_id"])
+        LOG.debug("Writing pickup %d: %s", i, pickup["resources"][0][0]["item_id"])
         try:
             pickup_object_for(lua_scripts, pickup, i, configuration).patch(editor)
         except NotImplementedError as e:
             LOG.warning(e)
 
 
 def patch_doors(editor: PatcherEditor, doors_config: list[dict]):
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando/elevator.py` & `open-dread-rando-2.1.0/open_dread_rando/elevator.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/environmental_damage.py` & `open-dread-rando-2.1.0/open_dread_rando/environmental_damage.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/environmental_damage_sources.py` & `open-dread-rando-2.1.0/open_dread_rando/environmental_damage_sources.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/exefs.py` & `open-dread-rando-2.1.0/open_dread_rando/exefs.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/custom_scenario.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/custom_scenario.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/dread_depackager/main.npdm` & `open-dread-rando-2.1.0/open_dread_rando/files/dread_depackager/main.npdm`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/dread_depackager/subsdk9` & `open-dread-rando-2.1.0/open_dread_rando/files/dread_depackager/subsdk9`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/exefs_patches/debug_input.s` & `open-dread-rando-2.1.0/open_dread_rando/files/exefs_patches/debug_input.s`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s010_cave.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s010_cave.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s020_magma.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s020_magma.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s030_baselab.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s030_baselab.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s040_aqua.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s040_aqua.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s050_forest.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s050_forest.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s060_quarantine.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s060_quarantine.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s070_basesanc.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s070_basesanc.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s080_shipyard.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s080_shipyard.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/levels/s090_skybase.lc.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/levels/s090_skybase.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/bit.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/bit.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/data_structures.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/data_structures.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/death_counter.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/death_counter.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/guilib.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/guilib.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/input_handling.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/input_handling.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/lua_libraries/room_names.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/lua_libraries/room_names.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/msemenu_mainmenu.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/msemenu_mainmenu.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/randomizer_powerup.lua` & `open-dread-rando-2.1.0/open_dread_rando/files/randomizer_powerup.lua`

 * *Files 5% similar despite different names*

```diff
@@ -39,31 +39,35 @@
 function RandomizerPowerup.MarkLocationCollected(locationIdentifier)
     local playerSection = Game.GetPlayerBlackboardSectionName()
     local propName = RandomizerPowerup.PropertyForLocation(locationIdentifier)
     Game.LogWarn(0, propName)
     Blackboard.SetProp(playerSection, propName, "b", true)
 end
 
-function RandomizerPowerup.OnPickedUp(actor, progression)
+function RandomizerPowerup.OnPickedUp(actor, resources)
     RandomizerPowerup.Self = actor
     local name = "Boss"
     if actor ~= nil then
         name = actor.sName
         RandomizerPowerup.MarkLocationCollected(string.format("%s_%s", Scenario.CurrentScenarioID, name))
     end
 
     Game.LogWarn(0, "Collected pickup: " .. name)
-    local granted = RandomizerPowerup.ProgressivePickup(actor, progression)
+    local granted = RandomizerPowerup.HandlePickupResources(resources)
+
     -- RandomizerPowerup.ChangeSuit()
-    RandomizerPowerup.IncreaseEnergy(granted)
-    RandomizerPowerup.IncreaseAmmo(granted)
 
-    RandomizerPowerup.CheckArtifacts(granted)
-    RandomizerPowerup.ApplyTunableChanges()
+    for _, resource in ipairs(granted) do
+        RandomizerPowerup.IncreaseEnergy(resource)
+        RandomizerPowerup.IncreaseAmmo(resource)
+
+        RandomizerPowerup.CheckArtifacts(resource)
+    end
 
+    RandomizerPowerup.ApplyTunableChanges()
     Scenario.UpdateProgressiveItemModels()
     RL.UpdateRDVClient(false)
     return granted
 end
 
 function RandomizerPowerup.DisableInput()
     -- items with unique inputs (Speed Booster, Phantom Cloak) require disabling and re-enabling inputs to work properly
@@ -76,38 +80,56 @@
 function RandomizerPowerup.RecoverInput()
     local oPlayer = Game.GetPlayer()
     if oPlayer ~= nil then
         oPlayer.INPUT:IgnoreInput(false, false, "PickupObtained")
     end
 end
 
-function RandomizerPowerup.ProgressivePickup(actor, progression)
+function RandomizerPowerup.HandlePickupResources(progression)
     progression = progression or {}
-    local loop = false
+
+    local alwaysGrant = false
 
     if #progression == 0 then
-        return nil
+        return {}
     elseif #progression == 1 then
-        loop = true
+        alwaysGrant = true
     end
 
-    local data = "Progression: "
-    for _, resource in ipairs(progression) do
-        data = data .. resource.item_id .. " (" .. resource.quantity .. ") / "
+    Game.LogWarn(0, "Resources:")
+    for _, resource_list in ipairs(progression) do
+        local data = "  - "
+        for _, resource in ipairs(resource_list) do
+            data = data .. resource.item_id .. " (" .. resource.quantity .. ") / "
+        end
+        Game.LogWarn(0, data)
     end
-    Game.LogWarn(0, data)
 
-    for _, resource in ipairs(progression) do
-        local current = RandomizerPowerup.GetItemAmount(resource.item_id)
-        if loop or current < resource.quantity then
-            Game.LogWarn(0, "Granting " .. resource.quantity .. " " .. resource.item_id)
-            RandomizerPowerup.IncreaseItemAmount(resource.item_id, resource.quantity)
-            return resource
+    -- For each progression stage, if the player does not have the FIRST item in that stage, the whole stage is granted
+    for _, resource_list in ipairs(progression) do
+        -- Check if we need to grant anything from this progression stage
+
+        if #resource_list > 0 then
+            local current = RandomizerPowerup.GetItemAmount(resource_list[1].item_id)
+            local shouldGrant = alwaysGrant or current < resource_list[1].quantity
+
+            if shouldGrant then
+                for _, resource in ipairs(resource_list) do
+                    Game.LogWarn(0, "Granting " .. resource.quantity .. " " .. resource.item_id)
+                    RandomizerPowerup.IncreaseItemAmount(resource.item_id, resource.quantity)
+                end
+
+                return resource_list
+            end
         end
+
+        -- Otherwise, loop to next progression stage (or fall out of loop)
     end
+
+    return {} -- nothing granted after final stage of progression is reached
 end
 
 function RandomizerPowerup.ChangeSuit()
     -- ordered by priority
     local suits = {
         {item = "ITEM_HYPER_SUIT", model = "Hyper"},
         {item = "ITEM_GRAVITY_SUIT", model = "Gravity"},
@@ -136,21 +158,21 @@
     Game.LogWarn(0, "Updating suit to " .. model)
     model_updater.sModelAlias = model
 end
 
 MAX_ENERGY = 1499
 function RandomizerPowerup.IncreaseEnergy(resource)
     -- No resource, quit
-    if resource == nil then return end
+    if not resource then return end
+
     local item_id = resource.item_id
 
     -- Not etank or epart, quit
     if item_id ~= "ITEM_ENERGY_TANKS" and item_id ~= "ITEM_LIFE_SHARDS" then return end
 
-
     local energy = Init.fEnergyPerTank
 
     if item_id == "ITEM_LIFE_SHARDS" then
         if Init.bImmediateEnergyParts then
             energy = Init.fEnergyPerPart
         elseif (RandomizerPowerup.GetItemAmount(item_id) % 4) ~= 0 then
             -- only change energy every 4 parts if not immediate!
@@ -174,35 +196,36 @@
 
     local life = Game.GetPlayer().LIFE
     life.fMaxLife = new_max
     life.fCurrentLife = new_current
 end
 
 function RandomizerPowerup.IncreaseAmmo(resource)
-    if resource == nil then return end
+    if not resource then return end
+
     local current_id = nil
 
     if resource.item_id == "ITEM_WEAPON_POWER_BOMB_MAX" then
         current_id = "ITEM_WEAPON_POWER_BOMB_CURRENT"
     elseif resource.item_id == "ITEM_WEAPON_MISSILE_MAX" then
         current_id = "ITEM_WEAPON_MISSILE_CURRENT"
     end
 
     if current_id == nil then return end
 
     RandomizerPowerup.IncreaseItemAmount(current_id, resource.quantity, resource.item_id)
 end
 
 function RandomizerPowerup.CheckArtifacts(resource)
-    if resource == nil then return end
+    if not resource then return end
     if Init.iNumRequiredArtifacts == 0 then return end
     if RandomizerPowerup.HasItem("ITEM_METROIDNIZATION") then return end
 
     if resource.item_id:find("ITEM_RANDO_ARTIFACT", 1, true) then
-        GUI.AddEmmyMissionLogEntry("#MLOG_"..resource.item_id)
+        GUI.AddEmmyMissionLogEntry("#MLOG_" .. resource.item_id)
     end
 
     -- check for all artifact items, which are numbered. if all are collected, grant metroidnization
     for i=1, Init.iNumRequiredArtifacts do
         if RandomizerPowerup.GetItemAmount("ITEM_RANDO_ARTIFACT_"..i) == 0 then return end
     end
 
@@ -238,27 +261,40 @@
 
         Game.LogWarn(0, "Calling tunable handler for " .. item .. " = " .. totalQuantity)
 
         handler(totalQuantity)
     end
 end
 
--- Main PBs (always) + PB expansions (if required mains are disabled)
+-- Main PBs
 RandomizerPowerBomb = {}
 setmetatable(RandomizerPowerBomb, {__index = RandomizerPowerup})
 function RandomizerPowerBomb.OnPickedUp(actor, progression)
-    progression = progression or {{item_id = "ITEM_WEAPON_POWER_BOMB_MAX", quantity = 0}}
-    if actor ~= nil then
-        -- actor pickups grant the quantity directly; bosses do not
-        progression[1].quantity = 0
-    end
-    local granted = RandomizerPowerup.OnPickedUp(actor, progression)
-    if granted ~= nil and granted.item_id == "ITEM_WEAPON_POWER_BOMB_MAX" then
-        RandomizerPowerup.SetItemAmount("ITEM_WEAPON_POWER_BOMB", 1)
+    progression = progression or {{{ item_id = "ITEM_WEAPON_POWER_BOMB_MAX", quantity = 0 }}}
+    RandomizerPowerup.OnPickedUp(actor, progression)
+end
+
+-- Flash Shift
+RandomizerFlashShift = {}
+setmetatable(RandomizerFlashShift, {__index = RandomizerPowerup})
+function RandomizerFlashShift.OnPickedUp(actor, progression)
+    progression = progression or {{{item_id = "ITEM_UPGRADE_FLASH_SHIFT_CHAIN", quantity = 0}}}
+
+    local hasFlashShift = RandomizerPowerup.HasItem("ITEM_GHOST_AURA")
+
+    for _, resource_list in ipairs(progression) do
+        for _, resource in ipairs(resource_list) do
+            if resource.item_id == "ITEM_UPGRADE_FLASH_SHIFT_CHAIN" and hasFlashShift then
+                -- Subsequent Flash Shift main items do not grant additional chains
+                resource.quantity = 0
+            end
+        end
     end
+
+    RandomizerPowerup.OnPickedUp(actor, progression)
 end
 
 function RandomizerPowerup.ToggleInputsOnPickedUp(actor, progression, item, SFs)
     SFs = SFs or {}
     local has_item_already = RandomizerPowerup.HasItem(item)
     RandomizerPowerup.OnPickedUp(actor, progression)
     if not has_item_already then
@@ -299,11 +335,15 @@
         actor, progression, "ITEM_MULTILOCKON"
     )
 end
 
 RandomizerEnergyPart = {}
 setmetatable(RandomizerEnergyPart, {__index = RandomizerPowerup})
 function RandomizerEnergyPart.OnPickedUp(actor, progression)
+    Game.LogWarn(0, "RandomizerEnergyPart " .. type(progression))
+    progression = progression or {{{ item_id = "ITEM_LIFE_SHARDS", quantity = 1 }}}
     if Init.bImmediateEnergyParts or not actor then
-        RandomizerPowerup.IncreaseEnergy({item_id = "ITEM_LIFE_SHARDS"})
+        for _, resource in ipairs(progression[1]) do
+            RandomizerPowerup.IncreaseEnergy(resource)
+        end
     end
 end
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex` & `open-dread-rando-2.1.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/files/schema.json` & `open-dread-rando-2.1.0/open_dread_rando/files/schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910690419107457%*

 * *Differences: {"'$defs'": "{'item': OrderedDict([('type', 'object'), ('properties', OrderedDict([('item_id', "*

 * *            "OrderedDict([('$ref', '#/$defs/item_id')])), ('quantity', OrderedDict([('type', "*

 * *            "'number')]))])), ('required', ['item_id', 'quantity']), ('additionalProperties', "*

 * *            'False)])}',*

 * * "'properties'": "{'pickups': {'items': {'properties': {'resources': {'items': {'type': 'array', "*

 * *                 "'items': OrderedDict([('$ref', '#/$defs/item')]), 'minItems': 1, 'description': "*

 * * […]*

```diff
@@ -43,14 +43,30 @@
                 },
                 {
                     "type": "null"
                 }
             ],
             "default": null
         },
+        "item": {
+            "additionalProperties": false,
+            "properties": {
+                "item_id": {
+                    "$ref": "#/$defs/item_id"
+                },
+                "quantity": {
+                    "type": "number"
+                }
+            },
+            "required": [
+                "item_id",
+                "quantity"
+            ],
+            "type": "object"
+        },
         "item_id": {
             "enum": [
                 "ITEM_NONE",
                 "ITEM_WEAPON_WIDE_BEAM",
                 "ITEM_WEAPON_PLASMA_BEAM",
                 "ITEM_WEAPON_WAVE_BEAM",
                 "ITEM_WEAPON_HYPER_BEAM",
@@ -511,30 +527,58 @@
                             "corex",
                             "corpius",
                             "cutscene"
                         ],
                         "type": "string"
                     },
                     "resources": {
+                        "description": "An array of arrays representing progressive item stages and resource gains for each stage.",
+                        "examples": [
+                            [
+                                [
+                                    {
+                                        "item_id": "ITEM_WEAPON_WIDE_BEAM",
+                                        "quantity": 1
+                                    }
+                                ],
+                                [
+                                    {
+                                        "item_id": "ITEM_WEAPON_PLASMA_BEAM",
+                                        "quantity": 1
+                                    }
+                                ],
+                                [
+                                    {
+                                        "item_id": "ITEM_WEAPON_WAVE_BEAM",
+                                        "quantity": 1
+                                    }
+                                ]
+                            ],
+                            [
+                                [
+                                    {
+                                        "item_id": "ITEM_WEAPON_POWER_BOMB",
+                                        "quantity": 1
+                                    },
+                                    {
+                                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                                        "quantity": 2
+                                    }
+                                ]
+                            ]
+                        ],
                         "items": {
-                            "additionalProperties": false,
-                            "properties": {
-                                "item_id": {
-                                    "$ref": "#/$defs/item_id"
-                                },
-                                "quantity": {
-                                    "type": "number"
-                                }
+                            "description": "An array of all resources that will be gained from a particular stage of progression.",
+                            "items": {
+                                "$ref": "#/$defs/item"
                             },
-                            "required": [
-                                "item_id",
-                                "quantity"
-                            ],
-                            "type": "object"
+                            "minItems": 1,
+                            "type": "array"
                         },
+                        "minItems": 1,
                         "type": "array"
                     }
                 },
                 "required": [
                     "pickup_type",
                     "caption",
                     "resources"
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando/game_patches.py` & `open-dread-rando-2.1.0/open_dread_rando/game_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/lua_editor.py` & `open-dread-rando-2.1.0/open_dread_rando/lua_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 SPECIFIC_CLASSES = {
     "ITEM_WEAPON_POWER_BOMB": "RandomizerPowerBomb",
     "ITEM_OPTIC_CAMOUFLAGE": "RandomizerPhantomCloak",
     "ITEM_SPEED_BOOSTER": "RandomizerSpeedBooster",
     "ITEM_MULTILOCKON": "RandomizerStormMissile",
     "ITEM_LIFE_SHARDS": "RandomizerEnergyPart",
+    "ITEM_GHOST_AURA": "RandomizerFlashShift",
 }
 
 
 class LuaEditor:
     def __init__(self):
         self._progressive_classes = {}
         self._powerup_script = _read_powerup_lua()
@@ -40,41 +41,46 @@
         }
 
     def get_parent_for(self, item_id) -> str:
         return SPECIFIC_CLASSES.get(item_id, "RandomizerPowerup")
 
     def get_script_class(self, pickup: dict, boss: bool = False, actordef_name: str = "") -> str:
         pickup_resources = pickup["resources"]
-        parent = self.get_parent_for(pickup_resources[0]["item_id"])
-        if not boss and len(pickup_resources) == 1:
+        parent = self.get_parent_for(pickup_resources[0][0]["item_id"])
+
+        if not boss and len(pickup_resources) == 1 and len(pickup_resources[0]) == 1:
+            # Single-item pickup; don't include progressive template
             return parent
 
         if actordef_name and len(pickup["model"]) > 1:
             self.add_progressive_models(pickup, actordef_name)
 
         hashable_progression = "_".join([
-            f'{res["item_id"]}_{res["quantity"]}'
+            f'{res[0]["item_id"]}_{res[0]["quantity"]}'
             for res in pickup_resources
         ]).replace("-", "MINUS")
 
         if hashable_progression in self._progressive_classes.keys():
             return self._progressive_classes[hashable_progression]
 
         class_name = f"RandomizerProgressive{hashable_progression}"
 
         resources = [
-            {
-                "item_id": lua_util.wrap_string(res["item_id"]),
-                "quantity": res["quantity"]
-            }
-            for res in pickup_resources
+            [
+                {
+                    "item_id": lua_util.wrap_string(res["item_id"]),
+                    "quantity": res["quantity"]
+                }
+                for res in resource_list
+            ]
+            for resource_list in pickup_resources
         ]
         replacement = {
             "name": class_name,
-            "progression": resources,
+            "resources": resources,
             "parent": parent,
         }
         self.add_progressive_class(replacement)
 
         self._progressive_classes[hashable_progression] = class_name
         return class_name
 
@@ -85,16 +91,16 @@
     def add_progressive_models(self, pickup: dict, actordef_name: str):
         progressive_models = [
             {
                 "item": lua_util.wrap_string(resource["item_id"]),
                 "alias": lua_util.wrap_string(model_name),
             }
             for resource, model_name in itertools.chain(
-                zip(pickup["resources"], pickup["model"][1:]),
-                [(pickup["resources"][-1], pickup["model"][-1])],
+                zip([r[0] for r in pickup["resources"]], pickup["model"][1:]),
+                [(pickup["resources"][-1][0], pickup["model"][-1])],
             )
         ]
         progressive_models.reverse()
 
         replacement = {
             "actordef_name": actordef_name,
             "progressive_models": progressive_models,
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando/lua_util.py` & `open-dread-rando-2.1.0/open_dread_rando/lua_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import re
 from pathlib import Path
+from typing import Any
 
 from mercury_engine_data_structures.file_tree_editor import FileTreeEditor
 
 
 def _templates() -> Path:
     return Path(__file__).parent.joinpath("templates")
 
 
 def _files() -> Path:
     return Path(__file__).parent.joinpath("files")
 
 
-def replace_lua_template(file: str, replacement: dict[str, str], wrap_strings: bool = False) -> str:
+def replace_lua_template(file: str, replacement: dict[str, Any], wrap_strings: bool = False) -> str:
     code = _templates().joinpath(file).read_text()
     for key, content in replacement.items():
+        # Replace `TEMPLATE("key")`-style replacements
         code = code.replace(f'TEMPLATE("{key}")', lua_convert(content, wrap_strings))
+        # Replace `T__key__T`-style replacements
+        code = code.replace(f'T__{key}__T', lua_convert(content, wrap_strings))
 
     unknown_templates = re.findall(r'TEMPLATE\("([^"]+)"\)', code)
+    unknown_templates.extend(re.findall(r'T__(\w+)__T', code))
 
     if unknown_templates:
         raise ValueError("The following templates were left unfulfilled: " + str(unknown_templates))
 
     return code
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando/map_icons.py` & `open-dread-rando-2.1.0/open_dread_rando/map_icons.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/model_data.py` & `open-dread-rando-2.1.0/open_dread_rando/model_data.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/objective.py` & `open-dread-rando-2.1.0/open_dread_rando/objective.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/output_config.py` & `open-dread-rando-2.1.0/open_dread_rando/output_config.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/patch_util.py` & `open-dread-rando-2.1.0/open_dread_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/patcher_editor.py` & `open-dread-rando-2.1.0/open_dread_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/pickup.py` & `open-dread-rando-2.1.0/open_dread_rando/pickup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 EXPANSION_ITEM_IDS = {
     "ITEM_ENERGY_TANKS",
     "ITEM_LIFE_SHARDS",
     "ITEM_WEAPON_MISSILE_MAX",
     "ITEM_WEAPON_POWER_BOMB_MAX",
     "ITEM_WEAPON_POWER_BOMB",
+    "ITEM_UPGRADE_FLASH_SHIFT_CHAIN",
 
     # For multiworld
     "ITEM_NONE",
 }
 
-
 @functools.cache
 def _read_template_powerup():
     with Path(__file__).parent.joinpath("templates", "template_powerup_bmsad.json").open() as f:
         return json.load(f)
 
 
 class PickupType(Enum):
@@ -52,16 +52,16 @@
 
 class ActorPickup(BasePickup):
     def patch_single_item_pickup(self, bmsad: dict) -> dict:
         pickable: dict = bmsad["property"]["components"]["PICKABLE"]
         script: dict = bmsad["property"]["components"]["SCRIPT"]
 
         set_custom_params: dict = pickable["functions"][0]["params"]
-        item_id: str = self.pickup["resources"][0]["item_id"]
-        quantity: float = self.pickup["resources"][0]["quantity"]
+        item_id: str = self.pickup["resources"][0][0]["item_id"]
+        quantity: float = self.pickup["resources"][0][0]["quantity"]
 
         if item_id == "ITEM_ENERGY_TANKS":
             quantity *= self.configuration["energy_per_tank"]
             set_custom_params["Param4"]["value"] = "Full"
             set_custom_params["Param5"]["value"] = "fCurrentLife"
             set_custom_params["Param6"]["value"] = "LIFE"
 
@@ -101,27 +101,20 @@
             set_custom_params["Param13"] = {
                 "type": "f",
                 "value": quantity,
             }
 
         script["functions"][0]["params"]["Param2"]["value"] = self.lua_editor.get_script_class(self.pickup)
 
-        if item_id == "ITEM_WEAPON_POWER_BOMB":
-            item_id = "ITEM_WEAPON_POWER_BOMB_MAX"
-
         set_custom_params["Param1"]["value"] = item_id
         set_custom_params["Param2"]["value"] = quantity
 
         return bmsad
 
-    def patch_progressive_pickup(self, bmsad: dict) -> dict:
-        item_ids = {resource["item_id"] for resource in self.pickup["resources"]}
-        if not EXPANSION_ITEM_IDS.isdisjoint(item_ids):
-            raise NotImplementedError("Progressive pickups cannot include expansions.")
-
+    def patch_multi_item_pickup(self, bmsad: dict) -> dict:
         pickable: dict = bmsad["property"]["components"]["PICKABLE"]
         script: dict = bmsad["property"]["components"]["SCRIPT"]
 
         set_custom_params: dict = pickable["functions"][0]["params"]
         set_custom_params["Param1"]["value"] = "ITEM_NONE"
 
         script["functions"][0]["params"]["Param2"]["value"] = self.lua_editor.get_script_class(self.pickup,
@@ -218,18 +211,18 @@
 
         # Update caption
         pickable = new_template["property"]["components"]["PICKABLE"]
         pickable["fields"]["fields"]["sOnPickCaption"] = self.pickup["caption"]
         pickable["fields"]["fields"]["sOnPickTankUnknownCaption"] = self.pickup["caption"]
 
         # Update given item
-        if len(self.pickup["resources"]) == 1:
+        if len(self.pickup["resources"]) == 1 and len(self.pickup["resources"][0]) == 1:
             new_template = self.patch_single_item_pickup(new_template)
         else:
-            new_template = self.patch_progressive_pickup(new_template)
+            new_template = self.patch_multi_item_pickup(new_template)
 
         new_path = f"actors/items/randomizer_powerup/charclasses/randomizer_powerup_{self.pickup_id}.bmsad"
         editor.add_new_asset(new_path, Bmsad(new_template, editor.target_game), in_pkgs=pkgs_for_level)
         actor.oActorDefLink = f"actordef:{new_path}"
 
         # Powerup is in plain sight (except for the part we're using the sphere model)
         actor.pComponents.pop("LIFE", None)
@@ -256,26 +249,21 @@
         return self.lua_editor.patch_actordef_pickup_script(
             editor,
             self.pickup,
             self.pickup["pickup_lua_callback"],
         )
 
     def _patch_actordef_pickup(self, editor: PatcherEditor, item_id_field: str) -> tuple[str, Bmsad]:
-        resources = self.pickup["resources"]
-        item_id: str = resources[0]["item_id"]
-
-        # if len(resources) > 1 or resources[0]["quantity"] > 1 or item_id in EXPANSION_ITEM_IDS:
-        item_id = "ITEM_NONE"
         self._patch_actordef_pickup_script_help(editor)
 
         bmsad_path: str = self.pickup["pickup_actordef"]
         actordef = editor.get_file(bmsad_path, Bmsad)
 
         ai_component = actordef.raw["property"]["components"]["AI"]
-        ai_component["fields"]["fields"][item_id_field] = item_id
+        ai_component["fields"]["fields"][item_id_field] = "ITEM_NONE"
 
         patch_text(editor, self.pickup["pickup_string_key"], self.pickup["caption"])
 
         return bmsad_path, actordef
 
     def patch(self, editor: PatcherEditor):
         raise NotImplementedError()
@@ -299,15 +287,15 @@
             self.pickup["pickup_lua_callback"],
         )
 
 
 class CorpiusPickup(ActorDefPickup):
     def patch(self, editor: PatcherEditor):
         bmsad_path, actordef = self._patch_actordef_pickup(editor, "sInventoryItemOnKilled")
-        if self.pickup["resources"][0]["item_id"] not in EXPANSION_ITEM_IDS:
+        if self.pickup["resources"][0][0]["item_id"] not in EXPANSION_ITEM_IDS:
             actordef.raw["property"]["components"]["AI"]["fields"]["fields"]["bGiveInventoryItemOnDead"] = True
 
         editor.replace_asset(bmsad_path, actordef)
 
 
 class CutscenePickup(BasePickup):
     def patch(self, editor: PatcherEditor):
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando/static_fixes.py` & `open-dread-rando-2.1.0/open_dread_rando/static_fixes.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/templates/custom_core_x.lua` & `open-dread-rando-2.1.0/open_dread_rando/templates/custom_core_x.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua` & `open-dread-rando-2.1.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/templates/custom_init.lua` & `open-dread-rando-2.1.0/open_dread_rando/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/templates/template_doorshield_bmsad.json` & `open-dread-rando-2.1.0/open_dread_rando/templates/template_doorshield_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/templates/template_powerup_bmsad.json` & `open-dread-rando-2.1.0/open_dread_rando/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/templates/template_shieldenergy_bmsad.json` & `open-dread-rando-2.1.0/open_dread_rando/templates/template_shieldenergy_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/text_patches.py` & `open-dread-rando-2.1.0/open_dread_rando/text_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/tilegroup_patcher.py` & `open-dread-rando-2.1.0/open_dread_rando/tilegroup_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando/validator_with_default.py` & `open-dread-rando-2.1.0/open_dread_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/open_dread_rando.egg-info/PKG-INFO` & `open-dread-rando-2.1.0/open_dread_rando.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.0.0
+Version: 2.1.0
 Summary: An open source randomizer patcher for Metroid Dread.
 Home-page: https://github.com/randovania/open-dread-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `open-dread-rando-2.0.0/open_dread_rando.egg-info/SOURCES.txt` & `open-dread-rando-2.1.0/open_dread_rando.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,8 +113,9 @@
 open_dread_rando/templates/progressive_model_template.lua
 open_dread_rando/templates/randomizer_progressive_template.lua
 open_dread_rando/templates/template_doorshield_bmsad.json
 open_dread_rando/templates/template_powerup_bmsad.json
 open_dread_rando/templates/template_shieldenergy_bmsad.json
 tests/test_lua_util.py
 tests/test_schema.py
+tests/test_files/randomizer_progressive_expected.lua
 tests/test_files/starter_preset_patcher.json
```

### Comparing `open-dread-rando-2.0.0/setup.cfg` & `open-dread-rando-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.0.0/tests/test_files/starter_preset_patcher.json` & `open-dread-rando-2.1.0/tests/test_files/starter_preset_patcher.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978956935123042%*

 * *Differences: {"'pickups'": "{0: {'resources': [[OrderedDict([('item_id', 'ITEM_MORPH_BALL'), ('quantity', "*

 * *              "1)])]]}, 1: {'resources': [[OrderedDict([('item_id', 'ITEM_WEAPON_MISSILE_MAX'), "*

 * *              "('quantity', 2)])]]}, 2: {'resources': [[OrderedDict([('item_id', "*

 * *              "'ITEM_MAGNET_GLOVE'), ('quantity', 1)])]]}, 3: {'resources': "*

 * *              "[[OrderedDict([('item_id', 'ITEM_WEAPON_MISSILE_MAX'), ('quantity', 10)])]]}, 4: "*

 * *              "{'resources': [[OrderedDict([('item_id', 'ITE […]*

```diff
@@ -1023,18 +1023,20 @@
             "pickup_actor": {
                 "actor": "ItemSphere_ChargeBeam",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_MORPH_BALL",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_MORPH_BALL",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1044,18 +1046,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank011",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Spider Magnet acquired.",
             "map_icon": {
                 "icon_id": "powerup_spidermagnet"
             },
@@ -1065,18 +1069,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank012",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_MAGNET_GLOVE",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_MAGNET_GLOVE",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -1086,18 +1092,20 @@
             "pickup_actor": {
                 "actor": "Item_EnergyTank001",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -1107,18 +1115,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank001",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1128,18 +1138,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank002",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1149,18 +1161,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Suit acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_SUIT"
             },
@@ -1171,22 +1185,26 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank003",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_VARIA_SUIT",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_GRAVITY_SUIT",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_VARIA_SUIT",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_GRAVITY_SUIT",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Charge Beam acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_CHARGE"
             },
@@ -1197,22 +1215,26 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank004",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_CHARGE_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_DIFFUSION_BEAM",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_CHARGE_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_DIFFUSION_BEAM",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Flash Shift acquired.",
             "map_icon": {
                 "icon_id": "powerup_ghostaura"
             },
@@ -1222,18 +1244,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank005",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_GHOST_AURA",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_GHOST_AURA",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -1243,18 +1267,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank006",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -1264,18 +1290,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank007",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -1285,18 +1313,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank003_1",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -1306,18 +1336,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank009",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1327,18 +1359,20 @@
             "pickup_actor": {
                 "actor": "item_energytank_000",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1348,18 +1382,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_000",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Beam acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_BEAM"
             },
@@ -1371,26 +1407,32 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_001",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_WIDE_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_PLASMA_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_WAVE_BEAM",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_WIDE_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_PLASMA_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_WAVE_BEAM",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -1400,18 +1442,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_001",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1421,18 +1465,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_000",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Bomb acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_BOMB"
             },
@@ -1443,22 +1489,26 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_BOMB",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_LINE_BOMB",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_BOMB",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_LINE_BOMB",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1468,18 +1518,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_003",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -1489,18 +1541,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_004",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Beam acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_BEAM"
             },
@@ -1512,26 +1566,32 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank010",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_WIDE_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_PLASMA_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_WAVE_BEAM",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_WIDE_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_PLASMA_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_WAVE_BEAM",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Missile acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_MISSILE",
                 "original_actor": {
@@ -1547,22 +1607,26 @@
             "pickup_actor": {
                 "actor": "IT_VARIA_GEN_001",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_SUPER_MISSILE",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_ICE_MISSILE",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_SUPER_MISSILE",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_ICE_MISSILE",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -1572,18 +1636,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_002",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank",
                 "original_actor": {
@@ -1598,18 +1664,20 @@
             "pickup_actor": {
                 "actor": "ItemSphere_GrappleBeam",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1619,18 +1687,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank014",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank",
                 "original_actor": {
@@ -1645,18 +1715,20 @@
             "pickup_actor": {
                 "actor": "ItemSphere_ScrewAttack",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1666,18 +1738,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank015",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1687,18 +1761,20 @@
             "pickup_actor": {
                 "actor": "Item_MissileTank016",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1708,18 +1784,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_001",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Charge Beam acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_CHARGE"
             },
@@ -1730,22 +1808,26 @@
             "pickup_actor": {
                 "actor": "item_missiletank_005",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_CHARGE_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_DIFFUSION_BEAM",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_CHARGE_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_DIFFUSION_BEAM",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1755,18 +1837,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_006",
                 "layer": "default",
                 "scenario": "s010_cave"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -1776,18 +1860,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_002",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Storm Missile acquired.",
             "map_icon": {
                 "icon_id": "powerup_stormmissile"
             },
@@ -1797,18 +1883,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_012",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_MULTILOCKON",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_MULTILOCKON",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank",
                 "original_actor": {
@@ -1823,18 +1911,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_diffusionbeam",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1844,18 +1934,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1865,18 +1957,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_008",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1886,18 +1980,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_001",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -1907,18 +2003,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_003",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -1928,18 +2026,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_004",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Spin acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_SPIN"
             },
@@ -1950,22 +2050,26 @@
             "pickup_actor": {
                 "actor": "item_missiletank_005",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_DOUBLE_JUMP",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_SPACE_JUMP",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_DOUBLE_JUMP",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_SPACE_JUMP",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -1975,18 +2079,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_001",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -1996,18 +2102,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_007",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2017,18 +2125,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_000",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -2038,18 +2148,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_009",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2059,18 +2171,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_010",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2080,18 +2194,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_011",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2101,18 +2217,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2122,18 +2240,20 @@
             "pickup_actor": {
                 "actor": "item_energytank_000",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Beam acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_BEAM"
             },
@@ -2145,26 +2265,32 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_000",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_WIDE_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_PLASMA_BEAM",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_WAVE_BEAM",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_WIDE_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_PLASMA_BEAM",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_WAVE_BEAM",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2174,18 +2300,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_001",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -2195,18 +2323,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_002",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -2216,18 +2346,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_006",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -2237,18 +2369,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s020_magma"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2258,18 +2392,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_004",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2279,18 +2415,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_002",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank",
                 "original_actor": {
@@ -2305,18 +2443,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_widebeam",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus",
                 "original_actor": {
@@ -2331,18 +2471,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_bomb",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Bomb acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_BOMB"
             },
@@ -2353,22 +2495,26 @@
             "pickup_actor": {
                 "actor": "item_missiletank",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_BOMB",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_LINE_BOMB",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_BOMB",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_LINE_BOMB",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -2378,18 +2524,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2399,18 +2547,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2420,18 +2570,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_003",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2441,18 +2593,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_000",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -2462,18 +2616,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_001",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2483,18 +2639,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_001",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2504,18 +2662,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_007",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Missile acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_MISSILE"
             },
@@ -2526,22 +2686,26 @@
             "pickup_actor": {
                 "actor": "item_missiletank_008",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_SUPER_MISSILE",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_WEAPON_ICE_MISSILE",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_SUPER_MISSILE",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_ICE_MISSILE",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2551,18 +2715,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_000",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2572,18 +2738,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_010",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2593,18 +2761,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_002",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -2614,18 +2784,20 @@
             "pickup_actor": {
                 "actor": "item_energytank",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2635,18 +2807,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_003",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2656,18 +2830,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_002",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Main Power Bomb acquired.",
             "map_icon": {
                 "icon_id": "powerup_powerbomb"
             },
@@ -2677,18 +2853,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_001",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -2698,18 +2876,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_005",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2719,18 +2899,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_006",
                 "layer": "default",
                 "scenario": "s030_baselab"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -2740,18 +2922,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -2761,18 +2945,20 @@
             "pickup_actor": {
                 "actor": "powerup_ghostaura",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank",
                 "original_actor": {
@@ -2787,18 +2973,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_gravitysuit",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2808,18 +2996,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Phantom Cloak acquired.",
             "map_icon": {
                 "icon_id": "powerup_opticcamo"
             },
@@ -2829,18 +3019,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_001",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_OPTIC_CAMOUFLAGE",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_OPTIC_CAMOUFLAGE",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2850,18 +3042,20 @@
             "pickup_actor": {
                 "actor": "item_energytank_000",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -2871,18 +3065,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_003",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2892,18 +3088,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_005",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2913,18 +3111,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2934,18 +3134,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_002",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -2955,18 +3157,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_002",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -2976,18 +3180,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Spin acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_SPIN"
             },
@@ -2998,22 +3204,26 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_001",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_DOUBLE_JUMP",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_SPACE_JUMP",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_DOUBLE_JUMP",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_SPACE_JUMP",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3023,18 +3233,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_000",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Grapple Beam acquired.",
             "map_icon": {
                 "icon_id": "powerup_grapplebeam"
             },
@@ -3044,18 +3256,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_000",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_GRAPPLE_BEAM",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_GRAPPLE_BEAM",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3065,18 +3279,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_006",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Nothing acquired.",
             "map_icon": {
                 "custom_icon": {
                     "label": "NOTHING"
@@ -3088,18 +3304,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_004",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_NONE",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_NONE",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3109,18 +3327,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_007",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -3130,18 +3350,20 @@
             "pickup_actor": {
                 "actor": "item_energytank",
                 "layer": "default",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -3151,18 +3373,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3172,18 +3396,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3193,18 +3419,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_005",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -3214,18 +3442,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_001",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank",
                 "original_actor": {
@@ -3240,18 +3470,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_supermissile",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3261,18 +3493,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_002",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3282,18 +3516,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_000",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3303,18 +3539,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_004",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank",
                 "original_actor": {
@@ -3329,18 +3567,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_doublejump",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3350,18 +3590,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_000",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -3371,18 +3613,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_006",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -3392,18 +3636,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_007",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3413,18 +3659,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_003",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3434,18 +3682,20 @@
             "pickup_actor": {
                 "actor": "item_energytank_000",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -3455,18 +3705,20 @@
             "pickup_actor": {
                 "actor": "powerup_sonar",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3476,18 +3728,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_009",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3497,18 +3751,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Progressive Suit acquired.",
             "map_icon": {
                 "icon_id": "PROGRESSIVE_SUIT"
             },
@@ -3519,22 +3775,26 @@
             "pickup_actor": {
                 "actor": "item_missiletank",
                 "layer": "default",
                 "scenario": "s050_forest"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_VARIA_SUIT",
-                    "quantity": 1
-                },
-                {
-                    "item_id": "ITEM_GRAVITY_SUIT",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_VARIA_SUIT",
+                        "quantity": 1
+                    }
+                ],
+                [
+                    {
+                        "item_id": "ITEM_GRAVITY_SUIT",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3544,18 +3804,20 @@
             "pickup_actor": {
                 "actor": "item_energytank_000",
                 "layer": "default",
                 "scenario": "s060_quarantine"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank",
                 "original_actor": {
@@ -3570,18 +3832,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_plasmabeam_000",
                 "layer": "default",
                 "scenario": "s060_quarantine"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3591,18 +3855,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s060_quarantine"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3612,18 +3878,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_002",
                 "layer": "default",
                 "scenario": "s060_quarantine"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3633,18 +3901,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s060_quarantine"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus",
                 "original_actor": {
@@ -3659,18 +3929,20 @@
             "pickup_actor": {
                 "actor": "itemsphere_spacejump",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3680,18 +3952,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_001",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Speed Booster acquired.",
             "map_icon": {
                 "icon_id": "powerup_speedbooster"
             },
@@ -3701,18 +3975,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_SPEED_BOOSTER",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_SPEED_BOOSTER",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Screw Attack acquired.",
             "map_icon": {
                 "icon_id": "powerup_screwattack"
             },
@@ -3722,18 +3998,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_004",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_SCREW_ATTACK",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_SCREW_ATTACK",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3743,18 +4021,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_002",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -3764,18 +4044,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_001",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3785,18 +4067,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_003",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3806,18 +4090,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_001",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "map_icon": {
                 "icon_id": "item_missiletankplus"
             },
@@ -3827,18 +4113,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3848,18 +4136,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_001",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "map_icon": {
                 "icon_id": "item_powerbombtank"
             },
@@ -3869,18 +4159,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_002",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -3890,18 +4182,20 @@
             "pickup_actor": {
                 "actor": "item_missiletankplus_000",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3911,18 +4205,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment_000",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3932,18 +4228,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_005",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -3953,18 +4251,20 @@
             "pickup_actor": {
                 "actor": "item_energyfragment",
                 "layer": "default",
                 "scenario": "s070_basesanc"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "map_icon": {
                 "icon_id": "item_energyfragment"
             },
@@ -3974,18 +4274,20 @@
             "pickup_actor": {
                 "actor": "item_missiletank_000",
                 "layer": "default",
                 "scenario": "s080_shipyard"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "map_icon": {
                 "icon_id": "item_missiletank"
             },
@@ -3995,18 +4297,20 @@
             "pickup_actor": {
                 "actor": "item_powerbombtank_000",
                 "layer": "default",
                 "scenario": "s080_shipyard"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Tank acquired.\nEnergy capacity increased by 100.",
             "map_icon": {
                 "icon_id": "item_energytank"
             },
@@ -4016,216 +4320,242 @@
             "pickup_actor": {
                 "actor": "item_missiletank",
                 "layer": "default",
                 "scenario": "s080_shipyard"
             },
             "pickup_type": "actor",
             "resources": [
-                {
-                    "item_id": "ITEM_ENERGY_TANKS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_ENERGY_TANKS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "pickup_actordef": "actors/characters/emmyshipyard/charclasses/emmyshipyard.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnEmmyShipyardAbilityObtained",
                 "scenario": "s080_shipyard"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_POWER_BOMB",
             "pickup_type": "emmi",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Metroid DNA 1 acquired.",
             "pickup_actordef": "actors/characters/scorpius/charclasses/scorpius.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnCorpiusDeath_CUSTOM",
                 "scenario": "s010_cave"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_OPTICAL_CAMO",
             "pickup_type": "corpius",
             "resources": [
-                {
-                    "item_id": "ITEM_RANDO_ARTIFACT_1",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_RANDO_ARTIFACT_1",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "pickup_actordef": "actors/characters/emmycave/charclasses/emmycave.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnEmmyCaveDead",
                 "scenario": "s010_cave"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_SPIDER_MAGNET",
             "pickup_type": "emmi",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnHydrogigaDead_CUSTOM",
                 "scenario": "s040_aqua"
             },
             "pickup_type": "cutscene",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile+ Tank acquired.\nMissile capacity increased by 10.",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnExperimentDeath_CUSTOM",
                 "scenario": "s020_magma"
             },
             "pickup_type": "cutscene",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 10
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 10
+                    }
+                ]
             ]
         },
         {
             "caption": "Power Bomb Tank acquired.\nPower Bomb capacity increased by 1.",
             "pickup_actordef": "actors/characters/core_x_superquetzoa/charclasses/core_x_superquetzoa.bmsad",
             "pickup_lua_callback": {
                 "args": 2,
                 "function": "escue",
                 "scenario": "s070_basesanc"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_MULTI_LOCK",
             "pickup_type": "corex",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_POWER_BOMB_MAX",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Metroid DNA 3 acquired.",
             "pickup_actordef": "actors/characters/emmysanc/charclasses/emmysanc.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnEmmySancDead",
                 "scenario": "s070_basesanc"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_WAVE_BEAM",
             "pickup_type": "emmi",
             "resources": [
-                {
-                    "item_id": "ITEM_RANDO_ARTIFACT_3",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_RANDO_ARTIFACT_3",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "pickup_actordef": "actors/characters/emmymagma/charclasses/emmymagma.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnEmmyMagmaDead",
                 "scenario": "s020_magma"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_MORPH_BALL",
             "pickup_type": "emmi",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "pickup_actordef": "actors/characters/core_x/charclasses/core_x.bmsad",
             "pickup_lua_callback": {
                 "args": 2,
                 "function": "golzuna",
                 "scenario": "s050_forest"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_LINE_BOMB",
             "pickup_type": "corex",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Energy Part acquired.\nEnergy capacity increased by 25.",
             "pickup_actordef": "actors/characters/emmyforest/charclasses/emmyforest.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnEmmyForestDead",
                 "scenario": "s050_forest"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_ICE_MISSILE",
             "pickup_type": "emmi",
             "resources": [
-                {
-                    "item_id": "ITEM_LIFE_SHARDS",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_LIFE_SHARDS",
+                        "quantity": 1
+                    }
+                ]
             ]
         },
         {
             "caption": "Missile Tank acquired.\nMissile capacity increased by 2.",
             "pickup_actordef": "actors/characters/emmylab/charclasses/emmylab.bmsad",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnEmmyBaseLabDead",
                 "scenario": "s030_baselab"
             },
             "pickup_string_key": "GUI_ITEM_ACQUIRED_SPEED_BOOSTER",
             "pickup_type": "emmi",
             "resources": [
-                {
-                    "item_id": "ITEM_WEAPON_MISSILE_MAX",
-                    "quantity": 2
-                }
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_MISSILE_MAX",
+                        "quantity": 2
+                    }
+                ]
             ]
         },
         {
             "caption": "Metroid DNA 2 acquired.",
             "pickup_lua_callback": {
                 "args": 0,
                 "function": "OnKraidDeath_CUSTOM",
                 "scenario": "s020_magma"
             },
             "pickup_type": "cutscene",
             "resources": [
-                {
-                    "item_id": "ITEM_RANDO_ARTIFACT_2",
-                    "quantity": 1
-                }
+                [
+                    {
+                        "item_id": "ITEM_RANDO_ARTIFACT_2",
+                        "quantity": 1
+                    }
+                ]
             ]
         }
     ],
     "spoiler_log": {
         "Flash Shift": "Artaria - David Jaffe Room",
         "Grapple Beam": "Burenia - Teleport to Ferenia",
         "Metroid DNA 1": "Artaria - Corpius Arena",
```

