---
title: Towny
description: 
published: true
date: 2025-09-16T03:49:20.828Z
tags: 
editor: markdown
dateCreated: 2025-09-06T18:56:55.342Z
---

# Towny
![Towny Town](/towny-solterra.jpg)

[Towny](https://townyadvanced.github.io/) is a land management and protection plugin that lets players create and manage towns. Think of it as adding a civilization-building layer on top of regular Minecraft survival. Players can claim chunks of land (16x16 blocks) as protected town territory where only town members can build and interact with blocks.


## Getting Started
When you join the server, you'll start as a nomad without a town. You have two options:
- Join an existing town (if invited or if the town is open)
- Create your own town for **$1,000**

## Essential Player Commands

### Town Basics
- `/t spawn` - Teleport to your town's spawn point
- `/t` - View your town's info
- `/t list` - See all towns on the server
- `/t online` - See who's online in your town
- `/t leave` - Leave your current town
- `/t deposit [amount]` - Add money to town bank

### Claiming & Plots
- `/plot claim` - Claim a plot you're standing on (if for sale)
- `/plot forsale/fs [price]` - Put your plot up for sale
- `/plot notforsale/nfs` - Remove plot from sale
- `/plot perm` - View plot permissions

### Social
- `/res friend add [player]` - Add a friend (they can build on your plots)
- `/res friend remove [player]` - Remove a friend
- `/n` - View your nation's info (if in one)

## Mayor Commands

### Town Management
- `/t new [name]` - Create a new town ($1,000)
- `/t claim` - Claim the chunk you're standing in ($50 per chunk)
- `/t unclaim` - Unclaim a chunk
- `/t invite [player]` - Invite a player to your town
- `/t kick [player]` - Remove a resident

### Financial Management
- `/t set taxes [amount]` - Set daily tax (0-1000, can be percentage if enabled)
- `/t set plottax [amount]` - Set tax per plot owned
- `/t withdraw [amount]` - Take money from town bank
- `/t bankhistory` - View transaction history
- **Daily Upkeep**: Your town pays $100/day automatically. If it can't pay, the town goes into debt (bankruptcy enabled)

### Plot Management
- `/plot forsale [price]` - Sell a town plot to residents
- `/plot notforsale` - Stop selling a plot
- `/plot set [type]` - Change plot type (shop, arena, bank, jail, etc.)
- `/plot perm [type] [resident/ally/outsider] [on/off]` - Set plot permissions

### Town Settings
- `/t set spawn` - Set town spawn location
- `/t set homeblock` - Set new homeblock (town center)
- `/t set name [name]` - Rename town
- `/t set board [message]` - Set town message board
- `/t toggle pvp` - Toggle PVP in town (30s cooldown)
- `/t toggle public` - Allow/deny public spawning to your town

### Permissions & Ranks
- `/t rank add [player] assistant` - Make someone an assistant mayor
- `/t set perm [type] [on/off]` - Set default town permissions
- `/t trust add [town]` - Trust another town

## Important Notes
- Towns can claim up to 8 blocks per resident + bonus blocks from nation
- Bankruptcy system prevents deletion if you can't pay upkeep (debt cap: 7 days)
- Peaceful/neutral status costs extra daily ($25 for towns)
- You keep items on death in town areas
- Wilderness building/destroying is restricted by default