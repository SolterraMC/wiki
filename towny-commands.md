---
title: Towny
description: 
published: true
date: 2025-11-23T00:30:11.275Z
tags: towny
editor: markdown
dateCreated: 2025-10-15T16:32:19.926Z
---

![Towny Town](/towny-solterra.jpg)

[Towny](https://townyadvanced.github.io/) is a land management plugin that lets players create and manage towns. Players can claim chunks of land (16x16 blocks) as protected town territory.

## Getting Started

**New players start as Nomads.** You can either:
- Join an existing town (if invited or open)
- Create your own town for **$1,000** with `/town new [name]`

**GUI Alternative:** Use `/tmenu` for an interactive menu interface

**Quick Reference:** 
- View available plots: `/town catalog`
- Check town list: `/town list`
- See who's online: `/town online`

---

### Town Levels
Towns automatically advance through levels based on resident count:

| Level | Residents | Title | Max Townblocks | Outposts | Buy Bonus Limit |
|-------|-----------|-------|----------------|----------|-----------------|
| 0 | 0 | Ruins | 1 | 0 | 10 |
| 1 | 1 | Settlement | 50 | 0 | 0 |
| 2 | 2+ | Hamlet | 80 | 1 | 0 |
| 3 | 6+ | Village | 125 | 1 | 0 |
| 4 | 10+ | Town | 250 | 2 | 0 |
| 5 | 14+ | Large Town | 325 | 2 | 100 |
| 6 | 20+ | City | 475 | 3 | 150 |
| 7 | 24+ | Large City | 550 | 3 | 200 |
| 8 | 28+ | Metropolis | 700 | 4 | 300 |

---

## /town Commands


### Information & Navigation


| Command | Description |
|---------|-------------|
| `/town` or `/t` | View your town's information |
| `/town [name]` | View another town's information |
| `/town here` | View info for the town you're standing in |
| `/town list` | List all server towns (sortable by name/residents/balance/etc.) |
| `/town online` | See online players in your town |
| `/town spawn` | Teleport to your town's spawn |
| `/town spawn [town]` | Teleport to another town's spawn (if public) |
| `/town outpost [#]` | Teleport to an outpost |
| `/town catalog` | Browse plots for sale |

### Joining & Leaving
| Command | Description |
|---------|-------------|
| `/town join [name]` | Join an open town |
| `/town leave` | Leave your current town |

### Money Management
| Command | Description |
|---------|-------------|
| `/town deposit [amount]` | Add money to town bank |
| `/town deposit all` | Deposit all your money |
| `/town withdraw [amount]` | Withdraw from town bank (Mayor only) |
| `/town withdraw all` | Withdraw all money (Mayor only) |
| `/town bankhistory [#]` | View transaction history (Mayor only) |
| `/town baltop` | View richest players in town |

### Town Creation & Claims (Mayor)
| Command | Description |
|---------|-------------|
| `/town new [name]` | Create a new town ($1,000) |
| `/town claim` | Claim current chunk ($50 per chunk) |
| `/town claim outpost` | Claim an outpost (must be in nation) |
| `/town claim [radius]` | Claim area around you |
| `/town claim auto` | Claim as many chunks as possible |
| `/town unclaim` | Unclaim current chunk |
| `/town unclaim all` | Unclaim all town land |
| `/town buy bonus [amount]` | Buy additional townblocks |

### Resident Management (Mayor)
| Command | Description |
|---------|-------------|
| `/town add [player]` or `/town invite [player]` | Invite player to town |
| `/town kick [player]` | Remove resident from town |
| `/town rank add [player] [rank]` | Grant rank (assistant, etc.) |
| `/town rank remove [player] [rank]` | Remove rank |
| `/town ranklist` | Display all residents and their ranks |

### Town Settings (Mayor)
| Command | Description |
|---------|-------------|
| `/town set board [message]` | Set town message board |
| `/town set mayor [resident]` | Transfer mayorship |
| `/town set homeblock` | Set new town center |
| `/town set spawn` | Set spawn point (must be in homeblock) |
| `/town set spawncost [amount]` | Set cost for public spawning |
| `/town set name [name]` | Rename town |
| `/town set tag [4chars]` | Set town tag for chat |
| `/town set taxes [amount]` | Set daily tax (percentage by default) |
| `/town set taxpercentcap [amount]` | Maximum tax when using percentage |
| `/town set plottax [amount]` | Set tax per plot owned |
| `/town set plotprice [amount]` | Set default plot price |
| `/town set shopprice [amount]` | Set shop plot price |
| `/town set shoptax [amount]` | Set shop plot tax |
| `/town set embassyprice [amount]` | Set embassy plot price |
| `/town set embassytax [amount]` | Set embassy plot tax |

### Permissions (Mayor)
| Command | Description |
|---------|-------------|
| `/town set perm [on/off]` | Edit all permissions |
| `/town set perm [resident/ally/outsider] [on/off]` | Set group permissions |
| `/town set perm [build/destroy/switch/itemuse] [on/off]` | Set specific permissions |
| `/town set perm reset` | Apply town perms to all plots |

### Town Toggles (Mayor)
| Command | Description |
|---------|-------------|
| `/town toggle pvp` | Enable/disable PVP (30s cooldown) |
| `/town toggle public` | Allow/deny public spawning |
| `/town toggle open` | Allow/deny open joining |
| `/town toggle explosion` | Toggle explosions |
| `/town toggle fire` | Toggle fire spread |
| `/town toggle mobs` | Toggle hostile mob spawning |
| `/town toggle taxpercent` | Switch between percentage/flat tax |
| `/town toggle nationzone` | Toggle nation zone |

### Other Mayor Commands
| Command | Description |
|---------|-------------|
| `/town say [message]` | Broadcast to online town members |
| `/town outlaw add/remove [player]` | Manage outlaw list |
| `/town jail [player] [hours] [bail]` | Jail a resident |
| `/town unjail [player]` | Release from jail |
| `/town delete` | Delete your town |
| `/town merge [townname]` | Request to merge with another town |

---

## /plot Commands

### Basic Commands
| Command | Description |
|---------|-------------|
| `/plot claim` | Claim a plot for sale |
| `/plot unclaim` | Unclaim your plot |
| `/plot perm` | View plot permissions |
| `/plot perm hud` | Toggle permission HUD |

### Buying & Selling
| Command | Description |
|---------|-------------|
| `/plot forsale [price]` or `/plot fs [price]` | Put plot up for sale |
| `/plot notforsale` or `/plot nfs` | Remove from sale |
| `/plot evict` | Evict plot owner (Mayor/Assistant) |

### Plot Configuration
| Command | Description |
|---------|-------------|
| `/plot set reset` | Reset to normal plot |
| `/plot set shop` | Set as shop plot |
| `/plot set embassy` | Set as embassy plot |
| `/plot set arena` | Set as arena plot |
| `/plot set wilds` | Set as wilds plot |
| `/plot set inn` | Set as inn plot |
| `/plot set jail` | Set as jail plot |
| `/plot set farm` | Set as farm plot |
| `/plot set bank` | Set as bank plot |
| `/plot set name [name]` | Name your plot |

### Plot Permissions
| Command | Description |
|---------|-------------|
| `/plot set perm [on/off]` | Edit all permissions |
| `/plot set perm [resident/ally/outsider] [on/off]` | Set group permissions |
| `/plot set perm [build/destroy/switch/itemuse] [on/off]` | Set specific permissions |
| `/plot set perm reset` | Reset to default permissions |

### Plot Toggles
| Command | Description |
|---------|-------------|
| `/plot toggle fire` | Toggle fire spread |
| `/plot toggle pvp` | Toggle PVP |
| `/plot toggle explosion` | Toggle explosions |
| `/plot toggle mobs` | Toggle hostile mobs |
| `/plot toggle taxed` | Toggle if plot is taxed |

### Plot Groups
| Command | Description |
|---------|-------------|
| `/plot group add [name]` | Create/add to plot group |
| `/plot group remove` | Remove plot from group |
| `/plot group delete` | Delete entire group |
| `/plot group rename [name]` | Rename group |
| `/plot group forsale [price]` | Sell entire group |
| `/plot group notforsale` | Remove group from sale |
| `/plot group set [type]` | Set group plot type |

### Plot Trust
| Command | Description |
|---------|-------------|
| `/plot trust add [player]` | Add trusted player |
| `/plot trust remove [player]` | Remove trusted player |

---

## /resident Commands

### Basic Commands
| Command | Description |
|---------|-------------|
| `/resident` or `/res` | View your resident info |
| `/resident [player]` | View another player's info |
| `/resident list` | List online residents |
| `/resident tax [player]` | View taxes paid |
| `/resident jail paybail` | Pay to leave jail |

### Friend Management
| Command | Description |
|---------|-------------|
| `/resident friend add [player]` | Add friend (can build on your plots) |
| `/resident friend add+ [player]` | Add offline player as friend |
| `/resident friend remove [player]` | Remove friend |
| `/resident friend clearlist` | Clear all friends |
| `/resident friend list` | View friend list |

### Personal Settings
| Command | Description |
|---------|-------------|
| `/resident set perm [on/off]` | Set all permissions for your plots |
| `/resident set perm [friend/ally/outsider] [on/off]` | Set group permissions |
| `/resident set perm [build/destroy/switch/itemuse] [on/off]` | Set specific permissions |
| `/resident set perm reset` | Apply perms to all your plots |
| `/resident set about [message]` | Set your bio/about message |

### Toggles
| Command | Description |
|---------|-------------|
| `/resident toggle pvp` | Toggle PVP on your plots |
| `/resident toggle fire` | Toggle fire on your plots |
| `/resident toggle explosion` | Toggle explosions on your plots |
| `/resident toggle mobs` | Toggle mobs on your plots |
| `/resident toggle map` | Toggle town map display |
| `/resident toggle townclaim` | Auto-claim when crossing borders |
| `/resident toggle plotborder` | Show plot borders |
| `/resident toggle constantplotborder` | Keep borders visible |

---

## /nation Commands

### Information & Navigation
| Command | Description |
|---------|-------------|
| `/nation` or `/n` | View your nation's info |
| `/nation [name]` | View another nation's info |
| `/nation list` | List all nations (sortable) |
| `/nation online` | Show online nation members |
| `/nation townlist [nation]` | List all towns in nation |
| `/nation allylist [nation]` | List nation's allies |
| `/nation enemylist [nation]` | List nation's enemies |
| `/nation ranklist` | Display residents and ranks |

### Nation Creation & Management (King/Mayor)
| Command | Description |
|---------|-------------|
| `/nation new [name]` | Create nation ($20,000 from town bank) |
| `/nation delete` | Delete your nation |
| `/nation leave` | Leave nation (Mayor command) |
| `/nation join [nation]` | Join open nation |

### Town Management (King)
| Command | Description |
|---------|-------------|
| `/nation add [town]` | Invite town to nation |
| `/nation kick [town]` | Remove town from nation |
| `/nation invite sent` | View sent invites |

### Money Management (King)
| Command | Description |
|---------|-------------|
| `/nation deposit [amount]` | Add money to nation bank |
| `/nation deposit all` | Deposit all money |
| `/nation withdraw [amount]` | Withdraw from nation bank |
| `/nation withdraw all` | Withdraw all money |
| `/nation deposit [amount] [town]` | Deposit to member town's bank |
| `/nation bankhistory [#]` | View transaction history |
| `/nation baltop` | View richest players in nation |

### Nation Settings (King)
| Command | Description |
|---------|-------------|
| `/nation set king [resident]` | Transfer leadership |
| `/nation set capital [town]` | Set capital town |
| `/nation set board [message]` | Set nation board |
| `/nation set spawn` | Set nation spawn |
| `/nation set spawncost [amount]` | Set public spawn cost |
| `/nation set name [name]` | Rename nation |
| `/nation set tag [4chars]` | Set nation tag |
| `/nation set taxes [amount]` | Set nation tax on towns |
| `/nation set conqueredtax [amount]` | Set conquered town tax |
| `/nation set taxpercentcap [amount]` | Max tax when using percentage |
| `/nation set mapcolor [color]` | Set dynmap color |

### Permissions & Ranks (King)
| Command | Description |
|---------|-------------|
| `/nation rank add [player] [rank]` | Grant nation rank |
| `/nation rank remove [player] [rank]` | Remove nation rank |
| `/nation set title [player] [title]` | Set player title |
| `/nation set surname [player] [surname]` | Set player surname |

### Diplomacy (King)
| Command | Description |
|---------|-------------|
| `/nation ally add [nation]` | Add ally |
| `/nation ally remove [nation]` | Remove ally |
| `/nation ally sent` | View sent ally requests |
| `/nation ally received` | View received ally requests |
| `/nation ally accept [nation]` | Accept alliance |
| `/nation ally deny [nation]` | Deny alliance |
| `/nation enemy add [nation]` | Add enemy |
| `/nation enemy remove [nation]` | Remove enemy |

### Nation Toggles (King)
| Command | Description |
|---------|-------------|
| `/nation toggle neutral` | Toggle neutral status (costs extra) |
| `/nation toggle open` | Allow open joining |
| `/nation toggle taxpercent` | Toggle percentage-based taxation |

### Other Commands
| Command | Description |
|---------|-------------|
| `/nation say [message]` | Broadcast to online nation members |
| `/nation merge [nation]` | Request to merge nations |
| `/nation sanctiontown add/remove [town]` | Manage sanctioned towns |

---

## Important Information

### Economy
- **Town Creation:** $1,000
- **Daily Upkeep:** $100/day per town
- **Chunk Claims:** $50 per chunk
- **Nation Creation:** $15,000 (from town bank)
- **Peaceful Town:** +$25/day
- **Peaceful Nation:** +$100/day
- **Bankruptcy Protection:** 7-day debt limit before deletion

### Limits & Mechanics
- **Townblocks:** 8 per resident + nation bonus + purchased blocks
- **Outposts:** Varies by town size (0-4, see Town Levels below)
- **Max Claim Radius:** 4 chunks at once
- **Chunks:** 16x16 blocks, infinite height
- **Protection:** Town areas protected from griefing
- **Keep Inventory:** Items retained on death in towns
- **Wilderness:** Building/destroying restricted by default
- **Teleport Warmup:** 3 seconds (movement cancels)
- **Spawn Cooldowns:** 30 seconds between uses

### Tax System
- **Daily Collection:** Taxes collected every 24 hours
- **Tax Types:** Flat rate or percentage (toggleable)
- **Plot Tax:** Additional tax per plot owned
- **Nation Tax:** Towns pay tax to their nation



### Plot Types
- **Normal:** Standard residential plot
- **Shop:** Commercial plots for trading
- **Embassy:** Plots for non-residents
- **Arena:** PVP-enabled plots
- **Wilds:** Allows wilderness permissions
- **Inn:** Healing/bed spawn plots
- **Jail:** Prisoner holding plots
- **Farm:** Agricultural plots
- **Bank:** Town bank access plots

### Other Costs
- **Outpost Claim:** $500
- **Town Rename:** $100
- **Nation Rename:** $1,000
- **Reclaim Ruined Town:** $500
- **Buy Bonus Blocks:** $100 per block (price increases with each purchase)

---

## Tips for New Players

1. **Before Creating a Town:**
   - Save at least $1,500 (creation + buffer for upkeep)
   - Consider joining an existing town first to learn
   - Check `/town list` to see successful towns

2. **Managing Your Town:**
   - Set reasonable taxes to maintain treasury
   - Claim strategically - each chunk costs daily upkeep
   - Use plot types to organize your town
   - Sell plots to residents for income

3. **Protection & Permissions:**
   - Default town perms apply to all unconfigured plots
   - Use `/plot set perm` for specific plot permissions
   - Add trusted players with `/res friend add`
   - Configure PVP settings per plot or town-wide

---

*For detailed documentation, visit the [Official Towny Wiki](https://github.com/TownyAdvanced/Towny/wiki)*