---
title: Player Warps
description: 
published: true
date: 2025-12-07T04:36:13.704Z
tags: 
editor: markdown
dateCreated: 2025-12-07T04:36:13.704Z
---

# Player Warps

![Player Warps](/playerwarps-solterra.jpg)

[Player Warps](https://docs.olziedev.com/projects/playerwarps) lets you create public teleport points that other players can visit. Share your builds, shops, or cool locations with the community and even earn money when players visit!

## [¶](#getting-started) Getting Started

**To create your first warp:**

1. Stand where you want your warp to be
2. Make sure you're inside a **Towny town** (required!)
3. Run `/pw set <name>` (costs **$500**)

Players can now visit your warp with `/pw <name>`. You'll earn $5 every time someone teleports there!

**GUI Alternative:** Use `/pw open` for an interactive menu interface

**Quick Reference:**

* Browse warps: `/pw list`
* Search for warps: `/pw search <query>`
* Find nearby warps: `/pw near`

---

## [¶](#teleporting) Teleporting

| Command | Description |
| --- | --- |
| `/pw <warp>` | Teleport to a warp ($5 fee) |
| `/pw list [page]` | Browse all available warps |
| `/pw near [page]` | Find warps within 100 blocks |
| `/pw search <query>` | Search for warps by name |
| `/pw open` | Open the GUI menu |
| `/pw rtp` | Teleport to a random warp |
| `/pw help` | Show all available commands |

---

## [¶](#creating-managing-warps) Creating & Managing Warps

| Command | Description |
| --- | --- |
| `/pw set <name>` | Create a new warp at your location ($500) |
| `/pw remove <warp>` | Delete your warp (full refund) |
| `/pw reset <warp>` | Move your warp to your current location |
| `/pw rename <warp> <newname>` | Change your warp's name |
| `/pw setowner <warp> <player>` | Transfer warp ownership |
| `/pw amount` | Check how many warps you have |
| `/pw info <warp>` | View detailed info about a warp |

---

## [¶](#customizing-your-warp) Customizing Your Warp

### [¶](#descriptions) Descriptions

| Command | Description |
| --- | --- |
| `/pw desc set <warp> <description>` | Add a description |
| `/pw desc remove <warp>` | Remove the description |

### [¶](#icons) Icons

| Command | Description |
| --- | --- |
| `/pw icon set <warp>` | Set icon to item in your hand |
| `/pw icon remove <warp>` | Remove custom icon |

### [¶](#categories) Categories

| Command | Description |
| --- | --- |
| `/pw category set <warp> <category>` | Assign a category |
| `/pw category remove <warp>` | Remove from category |
| `/pw category list <warp>` | See current categories |

---

## [¶](#ratings-reviews) Ratings & Reviews

Players can rate warps from 1-5 stars with a short comment. Good ratings help your warp get noticed!

| Command | Description |
| --- | --- |
| `/pw rate <warp> <1-5> <comment>` | Rate a warp |

**Note:** You can't rate your own warps, and banned players can't leave ratings.

---

## [¶](#managing-access) Managing Access

### [¶](#banning-players) Banning Players

| Command | Description |
| --- | --- |
| `/pw ban set <warp> <player>` | Ban someone from your warp |
| `/pw ban remove <warp> <player>` | Unban a player |
| `/pw ban list <warp>` | See who's banned |

### [¶](#managers) Managers

Add managers who can help moderate your warp (they can't delete it or transfer ownership).

| Command | Description |
| --- | --- |
| `/pw managers set <warp> <player>` | Add a manager |
| `/pw managers remove <warp> <player>` | Remove a manager |
| `/pw managers list <warp>` | List all managers |

---

## [¶](#favorites) Favorites

| Command | Description |
| --- | --- |
| `/pw favourite <warp>` | Add/remove from your favorites |

Run the same command again to remove a warp from favorites.

---

## [¶](#important-information) Important Information

### [¶](#economy) Economy

| Action | Cost |
| --- | --- |
| Creating a warp | $500 |
| Teleporting to a warp | $5 |
| Deleting your warp | Full refund |

**Earn passive income!** Every time someone teleports to your warp, you receive the $5 teleport fee.

### [¶](#limits-mechanics) Limits & Mechanics

* **Warp Names:** Maximum 14 characters (spaces show as underscores)
* **Teleport Warmup:** 3 seconds (movement cancels)
* **Teleport Cooldown:** 5 seconds between teleports
* **World Restrictions:** Cannot set warps in the Nether

### [¶](#towny-integration) Towny Integration

Warps can only be created inside Towny towns:

* You must be standing in a town plot to create a warp
* If your town gets deleted, warps in that town will also be removed
* This keeps warps in safe, established areas

### [¶](#bluemap) BlueMap

All player warps automatically appear on the web map with:

* Warp name and owner
* Visit count
* Description and ratings

---

## [¶](#tips-for-new-players) Tips for New Players

1. **Setting Up Your Warp:**
   * Choose a memorable name that's easy to type
   * Add a clear description so visitors know what to expect
   * Set an appropriate category to help players find you
   * Use a custom icon to stand out in the list

2. **Good Warp Etiquette:**
   * Don't trap players or put warps in dangerous locations
   * Keep your warp area tidy and welcoming
   * Respond to ratings and feedback

3. **Making Money:**
   * Popular warps can be a nice source of passive income
   * Shops, farms, and unique builds tend to attract visitors
   * Good ratings help your warp get discovered

---

*For detailed documentation, visit the [Official PlayerWarps Docs](https://docs.olziedev.com/projects/playerwarps)*