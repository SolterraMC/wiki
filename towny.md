---
title: Towny
description: 
published: true
date: 2025-09-14T18:21:40.705Z
tags: 
editor: markdown
dateCreated: 2025-09-06T18:56:55.342Z
---

## What Towny Does

[Towny](https://townyadvanced.github.io/) is a land management and protection plugin that lets players create and manage towns. Think of it as adding a civilization-building layer on top of regular Minecraft survival. Players can claim chunks of land (16x16 blocks) as protected town territory where only town members can build and interact with blocks.

## Basic Flow for Players

Players start as nomads with no town. They can either:
- Create their own town (costs money from Jobs/McMMO earnings)
- Join an existing town when invited by a mayor or assistant

Once in a town, they get a personal plot within the town's claimed chunks where they can build safely. Their stuff is protected from griefing, theft, and mob damage (depending on your config).

## The Claim System That Encourages Cooperation

Here's where Towny gets clever: Each town has a maximum number of chunks it can claim, determined by the number of residents. For example, with default settings:
- 1 resident = 16 chunks available
- 2 residents = 32 chunks available  
- 3 residents = 48 chunks available

This creates natural pressure for players to band together rather than everyone making solo towns. A single player trying to go alone gets very limited space, while groups can claim significant territory. You can adjust these ratios in the config to match your server's vision.

## Econ Balance

Towns require daily upkeep (paid from the town bank) based on their size. This creates a constant money sink that keeps your Jobs/McMMO economy relevant. If a town can't pay upkeep, it falls into ruins and eventually deletes, returning the land to wilderness.

## How It Plays With WorldGuard

Towny and WorldGuard work on different layers:
- WorldGuard protects your server areas (spawn, shops, arenas) with absolute priority
- Towny handles player-claimed areas everywhere else
- If there's overlap, WorldGuard takes precedence

So you'd use WorldGuard regions for spawn and server builds, while Towny handles the player civilization areas in the wider world.



## Towny Commands

### For Players - Basic Town Commands

**Getting Started:**
- `/towny` - Shows your status and basic info
- `/towny ? or /towny help` - Shows help menu
- `/towny map` - Shows ASCII map of nearby claimed chunks
- `/towny time` - Shows time until next day (when upkeep is collected)
- `/towny top residents/land/balance` - Shows leaderboards

**Creating/Joining Towns:**
- `/town new [name]` - Creates a new town (costs money)
- `/town join [townname]` - Join a town (need invitation)
- `/town leave` - Leave your current town
- `/town list` - Lists all towns on server
- `/town` or `/town here` - Shows info about town you're standing in

**Town Management (Mayor/Assistants):**
- `/town add [playername]` - Invite player to town
- `/town kick [playername]` - Remove resident from town
- `/town claim` - Claim the chunk you're standing in
- `/town unclaim` - Unclaim the chunk you're standing in
- `/town claim outpost` - Claim land away from main town (costs extra)
- `/town deposit [amount]` - Add money to town bank
- `/town withdraw [amount]` - Take money from town bank (mayor only)
- `/town rank add [playername] [rank]` - Give assistant/other ranks

**Plot Management:**
- `/plot claim` - Claim a plot within town (if for sale)
- `/plot unclaim` - Abandon your plot
- `/plot forsale [price]` - Put plot up for sale
- `/plot notforsale` - Remove plot from market
- `/plot set perm [resident/ally/outsider] [build/destroy/switch/itemuse] [on/off]` - Set plot permissions
- `/plot set [shop/arena/embassy/wilds]` - Set plot type

**Town Settings (Mayor):**
- `/town set name [newname]` - Rename town
- `/town set mayor [playername]` - Transfer mayorship
- `/town set spawn` - Set town spawn point at your location
- `/town spawn` - Teleport to town spawn
- `/town toggle pvp` - Toggle PvP in town
- `/town toggle public` - Toggle if town is open to join without invite
- `/town toggle explosion` - Toggle explosion protection
- `/town toggle mobs` - Toggle hostile mob spawning
- `/town toggle fire` - Toggle fire spread

### For Admins - Management Commands

**Admin Overrides:**
- `/townyadmin` or `/ta` - Shows admin help menu
- `/townyadmin set mayor [town] [player]` - Force mayor change
- `/townyadmin town [townname] deposit [amount]` - Add money to any town
- `/townyadmin town [townname] add [player]` - Force add player to town
- `/townyadmin town [townname] delete` - Delete a town
- `/townyadmin unclaim [radius]` - Force unclaim area around you

**Maintenance:**
- `/townyadmin backup` - Force backup of Towny data
- `/townyadmin newday` - Force new day (collects upkeep)
- `/townyadmin purge [days]` - Remove players inactive for X days
- `/townyadmin reload` - Reload Towny config files
- `/townyadmin reset` - Full Towny database reset (WARNING: deletes everything!)

**Toggle Commands:**
- `/townyadmin toggle debug` - Toggle debug mode
- `/townyadmin toggle devmode` - Toggle development mode (disables upkeep)
- `/townyadmin toggle npc [playername]` - Exempt player from inactivity purge
- `/townyadmin toggle upkeep` - Toggle upkeep collection globally

### Nation Commands (If Enabled)

- `/nation new [name]` - Create nation (mayors only, costs money)
- `/nation join [nation]` - Join nation as a town (mayor only)
- `/nation leave` - Leave nation
- `/nation deposit [amount]` - Add to nation bank
- `/nation ally add [nation]` - Propose alliance
- `/nation enemy add [nation]` - Declare enemy
- `/nation spawn` - Teleport to nation spawn

### Chat Commands

- `/tc [message]` - Town chat (or toggle with just /tc)
- `/nc [message]` - Nation chat (or toggle with just /nc)
- `/gc [message]` - Global chat
- `/lc [message]` - Local chat

### Shortcuts

- `/t` - Shortcut for /town
- `/n` - Shortcut for /nation
- `/p` or `/plot` - Plot commands
- `/ta` - Shortcut for /townyadmin
- `/res` - Shortcut for /resident
