# Deadly Deadly Dungeon — Wiki - WIP

> **Deadly Deadly Dungeon (DDD)** is a Minecraft datapack that adds large, procedurally generated dungeons with bosses, loot, and exploration-focused mechanics. This repository-style wiki is written for placement on GitHub (README.md + docs) and aims to remove common confusions players have about the datapack.

---

## Table of Contents

- [Quick Links](#quick-links)
- [Quick Start (installation)](#quick-start-installation)
- [Supported Versions & Platforms](#supported-versions--platforms)
- [What the pack adds (overview)](#what-the-pack-adds-overview)
- [Dungeon types — detailed](#dungeon-types--detailed)
- [Major vs Minor dungeons (performance note)](#major-vs-minor-dungeons-performance-note)
- [Generation mechanics (double randomization)](#generation-mechanics-double-randomization)
- [Vaults, Keys & Boss Spawners (the most confused bits)](#vaults-keys--boss-spawners-the-most-confused-bits)
- [Loot & Difficulty progression](#loot--difficulty-progression)
- [Player tips & recommended workflow](#player-tips--recommended-workflow)
- [Server / Multiplayer notes](#server--multiplayer-notes)
- [Compatibility & known mod interactions](#compatibility--known-mod-interactions)
- [Troubleshooting & Known Issues](#troubleshooting--known-issues)
- [Reporting bugs](#contributing--reporting-bugs)
- [FAQ (short answers to common confusions)](#faq-short-answers-to-common-confusions)
- [Changelog & credits](#changelog--credits)

---

## Quick Links

- Modrinth page (download & description)
- Issues / Feedback: GitHub (open an issue for bugs / texture problems / feature requests)

---

## Quick Start (installation)

**Two main install routes:**

1. **Datapack-only (vanilla compatible)**
   - Drop the `.zip` (or unpacked datapack folder) into your world `datapacks/` folder.
   - **Important:** if you are NOT running the modded version, make sure to copy the datapack into **both** the `datapack` folder and the **resourcepack** folder (or install the provided resourcepack). This supplies the new textures for items added by the datapack.

2. **Modded (Fabric / Forge / Quilt / NeoForge)**
   - Use the `+mod` release of the mod (the packaged mod version). Place it in your `mods/` folder and the matching datapack in `datapacks/` if required by the release. Follow the loader-specific installation steps.
   - The mod version it's just a datapack loader, there are no added features, it's there just to avoid manual loading.

**Notes**
- If you want the **Major** dungeons (very large variants), use the experimental Data Pack build (see the versions page on Modrinth). Major dungeons can be extremely expensive to generate — see the Performance note section.

---

## Supported Versions & Platforms

- **Minecraft Java:** 1.21.x, 1.20.6 (see Modrinth for exact supported sub-versions).
- **Platforms:** Data Pack, Fabric, Forge, NeoForge, Quilt.
- **Environments:** server-side; client & server (depending on install route).

---

## What the pack adds (overview)

- Procedurally generated dungeons of multiple types with **double-randomized** layouts (see generation section). Each dungeon contains rooms, corridors, mobs, bosses, vaults and special loot tables.
- Nine dungeon types are included (see detailed list below).
- Difficulty and loot scale as you descend through deeper levels.
- There are 4 difficulty levels, every times you descend a floor with stuff like stairs or jumps the difficulty level increase, after level 4 difficulty level will not increase further even if lower floors are present

---

## Dungeon types — detailed

There are nine main dungeon archetypes. Each entry below lists where they spawn and what to expect.

### Major Plains / Major Desert / Major Frozen
- **Where:** Plains / Desert / Frozen biomes respectively. Major variants are extremely large; they are only available in *experimental* builds (they have long generation times).
- **What to expect:** sprawling, multi-thousand-block complexes with huge room counts, long corridors, and many bosses. Exploration can take a very long time.
- **Bosses:** The Fallen Knights, The Rotten One and The Ugly one, Bob and Billy

### Minor Plains / Minor Desert / Minor Frozen
- **Where:** Same biome families as the major variants.
- **What to expect:** smaller (but still substantial) versions of the major dungeons. Designed to be more server-friendly while preserving the core features.
- **Bosses:** The Fallen Knights, The Rotten One and The Ugly one, Bob and Billy

### Spider Lair
- **Where:** Hot / temperate biomes.
- **What to expect:** labyrinthine tunnels and chambers, dense with spider-type mobs. Extremely easy to lose your sense of direction.
- **Bosses:** Mater Octavia or Pater Fidelis

### Monolithic Tower
- **Where:** Forested areas.
- **What to expect:** a tower with floors that contain loot, enemies and a boss on top
- **Bosses:** The Tower Guardian and the Praetorians

### Wizard Tower
- **Where:** Forested areas.
- **What to expect:** a huge vertical structure with multiple floors, wizard-themed rooms, a very unpolite wizard on top
- **Bosses:** The Wizard and the adepti

---

## Major vs Minor dungeons

- **Major dungeons** are designed as huge experiences and are marked as *experimental* builds. Generation of a major dungeon **can take a long time** (spawn/generation delays reported up to a few minutes on some hardware). Use with caution on live servers or low-end machines.
- **Minor dungeons** are intended to be the safer standard more performace friendly alternative.

---

## Generation mechanics (double randomization)

The datapack uses a two-layer randomization process:
1. **Layout randomization** — the arrangement of corridors, rooms and their connections changes each generation.
2. **Room randomization** — the internal content/layout of individual rooms varies between runs.

This makes every dungeon run feel unique: you may recognize the dungeon *type* but not the exact room contents or layout.

---

## Vaults, Keys & Boss Spawners (the most confused bits)

### Vaults — the two types
- **Normal Vault** — standard high-tier chest; you have to kill the boss to obtain the key.
- **Ominous Vault** — riskier/higher-tier variant; you have to kill the boss after you drink the ominous potion.

**Important rules (short):**
- Vaults are **always** located in the boss room area where you collect the boss key (i.e., the same room where you fight/collect the key), **except** for the *Wizard Tower*, where the vaults are on the **top floor** instead of next to the boss spawner.
- Vaults are placed in **close proximity to the boss spawner** (the block/area that spawns the boss).

### Keys
- **Where to get them:** Keys are collected in the boss rooms — you obtain the key from the trial spawner after defeating the boss. The key is needed to open the vaults located in that room.
- Normal keys open normal vault, ominous keys open ominous vaults as vanilla

### Boss Spawners
- The **boss spawner** is modified trial spwaner from which the boss (or boss wave) originates. It’s a reliable reference point: **vaults are placed near this spawner** in most dungeons.
- **Tip:** mark the boss spawner location (sign / block marker / coordinates) so you can return later if you are not ready.

---

## Loot & Difficulty progression

- Difficulty increases as you descend deeper into dungeon floors; deeper floors contain better loot and tougher encounters.
- Expect the best rewards to be guarded by the hardest rooms and bosses — risk vs reward.
- The general rule is that when you go down a stairs or a jump you descend on an other level. There are 4 levels, after that, if there are lower floors the difficulty level stays at 4.

---

## Player tips & recommended workflow

1. **Bring light** — torches / glow items to help navigation, especially in spider lairs.
2. **Explore methodically** — use your brain, calculate your actions, in the dungeons there are a lot of dangers but also a lot of resources you can use and room you cand find.
3. **Ender chest / bed / map strategy** — bring an ender chest in case you need a safe deposit of valuables, and set a bed nearby to reduce travel upon death, often you can finds bedrooms to set your spawn.
4. **Buddy runs** — consider running with a friend; dungeons are designed for serious challenges.
5. **Bosses can wait** - if you are not ready avoid entering a boss room, return when you are equipped

---

## Server / Multiplayer notes

- The pack is **server-side compatible** but large structures (major dungeons) can cause heavy load during generation.
- Remember to enable command blocks in the server files
- If you host a public server consider pre-generate the map.

---

## Compatibility & known mod interactions

- Designed to be compatible with **Terralith** and **Biomes O’ Plenty**, and generally compatible with mods that do not totally remove vanilla biomes or registered modded biomes, of course if vanilla or registeted biomes are rarer, dungeons will be rarer.

---

## Troubleshooting & Known Issues

- **Missing textures**: If new item textures look wrong, ensure you installed the resourcepack (see Quick Start). This is a common cause of odd icons and missing visuals.
- **Generation hangs / lag**: Major dungeons can take a long time to generate and may cause lag. Use the non-experimental builds.
- **Open issues:** There are community-reported issues (texture bugs, QoL feature requests) tracked in the GitHub feedback repository — check there before filing duplicates.

---

## Contributing & Reporting bugs

- To report a bug or file feedback, open an issue on the official GitHub feedback repo. When opening an issue include:
  - Minecraft version, pack version, platform (Data Pack / Fabric / Forge / Quilt / NeoForge)
  - A short description of the bug and steps to reproduce
  - Screenshots or a short video/GIF if helpful
  - Server vs singleplayer and any other datapacks/mods present
---

## FAQ (short answers to common confusions)

**Q:** Where are the vaults?  
**A:** In the boss room near the boss spawner — *except* Wizard Tower (top floor). Keys are dropped by the trial spawners after you kill the boss.

**Q:** There are no vaults and there are commands block suspended, what can i do?  
**A:** You are probably on a server with command blocks disabled, go in the server properties file and enable them.

**Q:** I don’t see textures for new items.  
**A:** Install the resourcepack or copy the datapack into the resourcepack folder (see Quick Start).

**Q:** How do I enable Major dungeons?  
**A:** Download & install the experimental Data Pack build from the versions list.

**Q:** Can I run this on a server?  
**A:** Use the non-experimental builds for best performance or consider pre-generate the chuncks.

---

## Changelog & Credits

- See the Modrinth page and the changelog for version-specific notes.
- Created by Caesius_Leo. Community feedback and issue tracking on GitHub (link in Quick Links).

---



