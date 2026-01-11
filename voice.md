---
title: Voice Chat
description: How to install Simple Voice Chat mod to use proximity voice chat on Solterra
published: true
date: 2026-01-11T00:00:00.000Z
tags: voice chat, mod, installation
editor: markdown
dateCreated: 2026-01-11T00:00:00.000Z
---

# Voice Chat

Solterra uses [Simple Voice Chat](https://modrinth.com/plugin/simple-voice-chat) for in-game proximity voice chat. This mod lets you talk to nearby players without needing Discord or other external software.

> **You must install this mod on your client to connect to the server.**
> The server requires the mod, so you won't be able to join without it installed.
{.is-info}

---

## [¶](#requirements) Requirements

Before installing, make sure you have:

* **Fabric Loader** or **Forge/NeoForge** installed for your Minecraft version
* **Fabric API** (only if using Fabric)
* A working microphone

---

## [¶](#installation) Installation

Choose the method that matches your launcher:

### [¶](#curseforge-app) CurseForge App

1. Open the **CurseForge App** and go to Minecraft
2. Select your modded profile (or create one with Fabric/Forge)
3. Click **Add More Content** and search for "Simple Voice Chat"
4. Click **Install** on the correct version for your mod loader
5. If using Fabric, also search for and install **Fabric API**
6. Launch the game

### [¶](#prism-launcher) Prism Launcher

1. Open **Prism Launcher** and select your instance
2. Click **Edit** → **Mods** → **Download Mods**
3. Choose **Modrinth** or **CurseForge** as your source
4. Search for "Simple Voice Chat" and install it
5. If using Fabric, also install **Fabric API**
6. Launch the game

### [¶](#modrinth-app) Modrinth App

1. Open the **Modrinth App** and select your profile
2. Click **Add content** and search for "Simple Voice Chat"
3. Click **Install** on the matching version
4. If using Fabric, also install **Fabric API**
5. Launch the game

### [¶](#manual-installation) Manual Installation

1. Download the mod from [Modrinth](https://modrinth.com/plugin/simple-voice-chat) or [CurseForge](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat)
   * Make sure to select the correct version for your Minecraft version and mod loader
2. If using Fabric, also download [Fabric API](https://modrinth.com/mod/fabric-api)
3. Place the `.jar` file(s) in your `.minecraft/mods` folder
4. Launch the game with your mod loader

---

## [¶](#in-game-controls) In-Game Controls

Default keybinds:

| Key | Action |
| --- | --- |
| `V` | Open voice chat settings |
| `Caps Lock` | Push-to-talk (hold to speak) |
| `M` | Mute/unmute yourself |
| `N` | Toggle voice chat on/off |
| `H` | Hide/show player icons |
| `G` | Open group menu |

> These defaults may conflict with other mods (e.g., `M` is often used by map mods). You can rebind these in **Options** → **Controls** → **Key Binds** or through the voice chat settings (`V`).
{.is-warning}

---

## [¶](#first-time-setup) First-Time Setup

1. Join the server and press `V` to open voice chat settings
2. Click the microphone icon to select your input device
3. Adjust your activation threshold if using voice activation
4. Test your mic by speaking - your icon should light up

---

## [¶](#troubleshooting) Troubleshooting

### Can't hear others or they can't hear you

* Check that your microphone is selected in the voice chat settings (`V`)
* Make sure you're not muted (press `M` to toggle)
* Verify voice chat is enabled (press `N` to toggle)

### Voice chat not connecting

* Some ISPs (notably T-Mobile in the US) may block the UDP ports used by voice chat
* Try using a VPN if you're experiencing connection issues
* Check your firewall settings

### No voice chat option in-game

* Make sure you downloaded the correct mod version for your mod loader (Fabric/Forge)
* Verify the mod is in your mods folder and loaded (check the Mods menu)

### macOS microphone issues

* Go to **System Preferences** → **Security & Privacy** → **Privacy** → **Microphone**
* Make sure your Minecraft launcher has microphone permission

---

## [¶](#links) Helpful Links

* [Simple Voice Chat on Modrinth](https://modrinth.com/plugin/simple-voice-chat)
* [Simple Voice Chat on CurseForge](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat)
* [Official Installation Guide](https://modrepo.de/minecraft/voicechat/wiki/installation)
* [Fabric API on Modrinth](https://modrinth.com/mod/fabric-api)
