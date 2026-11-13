# Controls, Config, FAQ & Content Index

## Controls

All keybinds can be changed in Minecraft Controls under **Velorise EMC**.

| Keybind | Function |
|---|---|
| Open EMC Hub | Opens personal EMC information and server-controlled EMC options. |
| Shift Alchemical Charge | Changes the selected charge or mode on supported equipment. |
| Repair Imbued Equipment | Manually spends EMC to repair the held or supported Core-bound item. |
| Aetheric Elytra Boost | Activates the Imbued Elytra boost while gliding. |
| Activate Aquatic Breathing | Activates the Imbued Turtle Helmet effects. |

Common interactions:

- Right-click Philosopher's Stone on a supported block to transmute it.
- Right-click Transmutation Tablet to open portable transmutation.
- Shift + Right-click an empty Knowledge Sharing Book to capture knowledge.
- Hold right-click with Magic Mirror to channel teleportation.
- Shift-use Magic Mirror for a linked Waypoint Anchor destination.
- Right-click Attraction Catalyst to toggle attraction.
- Use Chalice directly on a fluid or growable block.
- Right-click Void Translocator to teleport forward.
- Mouse wheel while using Far-Sight Glass to change zoom.
- Held portable workstations open their menu by right-clicking in air or inventory use.

---

---

## Server configuration overview

Server-authoritative settings are stored in `config/velorise_emc/gameplay.json`. Clients receive the normalized gameplay snapshot from the server.

Current configuration schema: **24**.

Major configurable groups:

### Economy

- Tax enabled in Default or Balanced mode
- Tax recovery rate
- Tax brackets and surcharges
- EMC value mode
- Custom item EMC values
- Burn, learn and materialization policies

### Machines

- Hourglass capacity, pulse rate, virtual ticks, cost and radius
- Furnace-family cooking-speed multipliers
- Tidal Conduit capacity, range and operating cost
- Matterburst radius, depth, damage and work rate
- Resonance Jukebox capacity and running cost
- Purification Grindstone operation cost

### Items and Arcane Weapons

- Utility costs, ranges and cooldowns
- Core armor and repair values
- Arcane damage, range, radius, duration, cost and cooldown
- Modded-item compatibility lists and per-item overrides

### Progression

- Every World Tier objective
- Contributor scaling mode and multiplier
- Boss objective scaling
- Maximum counted contributors

### World systems

- Resonance Spire generation and output
- Boss player-count scaling
- World Threat health and damage scaling
- Modded hostile inclusion and exclusions

The values in this README describe defaults, not guarantees on every server.

---

---

## Frequently asked questions

### Do Transmutation Tables generate EMC?

No. They store, teach, burn and materialize through the player's account. EMC must come from items, world systems or active generators implemented elsewhere.

### Is EMC shared between players?

No. Personal EMC funds and learned-item lists are player-specific. World Tier progression is shared by the world/server.

### Can I use the mod in an existing world?

Yes. Resonant ore retrogen is designed to bless existing chunks when new World Tiers unlock.

### Does Core IV make actions cheaper?

Usually no. Core IV increases power, range, throughput or capacity. The same successful unit of work normally keeps its fixed EMC price.

### Can Arcane Weapons run without EMC?

No. A shot, channel, teleport or powered action fails when the player cannot afford its complete required cost.

### Why are some weapons much stronger than others?

Core-I strength is balanced around the inspired mob, recipe difficulty, availability and weapon mechanic. Higher tiers then strengthen each weapon's identity. A multi-shot or control weapon is not balanced only by its displayed single-hit damage.

### Does Stormcaller use real Vanilla lightning?

It uses controlled lightning behavior. It can charge Creepers, but it does not freely apply every Vanilla lightning transformation or uncontrolled structure fire.

### Do fire weapons cook meat drops?

Yes, where the mob's Vanilla loot supports a cooked variant and the fire attack kills it while burning.

### Does Shulker Launcher home onto enemies?

No. The player aims every bolt manually. Core increases bolt count and control duration.

### Why does Evoker Fang repeat in one place?

The staff records the original five fang positions and repeats those exact positions for later waves. Higher Core tiers add waves, not a longer attack line.

### Is the Echobound Greatsword supposed to be extremely strong?

Yes. It is crafted only after defeating the final Echobound Dragon and is intentionally a post-boss reward.

### Are Condensed Core blocks passive generators?

They generate only for eligible Survival players standing within three blocks, and their fixed output is split between nearby players. They are not unlimited long-range chunk generators.

### Are all modded weapons and armor automatically compatible with Core upgrades?

The mod supports broad damageable-item compatibility, but custom item classes can behave differently. Servers can force-include items, restrict them to repair-only or provide per-item overrides.

---

---

## Complete content index

### Directly registered special items

- Philosopher's Stone
- Transmutation Tablet
- Tome of Knowledge
- Knowledge Sharing Book
- Wireless Core I–IV
- Condensed Core I–IV
- Infernal Ascension Template
- End Ascension Template
- Deep Convergence Template
- Void Translocator
- Attraction Catalyst
- Chalice of Transmutation
- Magic Mirror
- Cursed Igniter
- Purifying Milk
- Eye of the Last Echo
- Heart of the Last Echo
- Echobound Dragon Scale

### Arcane Weapons

- Inferno Rod
- Ghastfire Staff
- Dragonfire Scepter
- Resonant Echo
- Wither Scepter
- Shulker Launcher
- Guardian Lens
- Evoker Fang Staff
- Stormcaller
- Frostbolt Wand
- Webcaster

### Alchemical fuel

- Alchemical Coal
- Mobius Fuel
- Aeternalis Fuel
- Alchemical Coal Block
- Mobius Fuel Block
- Aeternalis Fuel Block

### Resonant material families

Each of Verdant, Infernal, Aetheric and Echoing includes:

- Ore
- Raw material
- Ingot
- Storage block
- Sword
- Pickaxe
- Axe
- Shovel
- Hoe
- Helmet
- Chestplate
- Leggings
- Boots

Verdant also has a Deepslate ore variant.

### Echobound equipment

- Echobound Helmet
- Echobound Chestplate
- Echobound Leggings
- Echobound Boots
- Echobound Greatsword
- Echobound Pickaxe

### Placeable and machine blocks

- Verdant Resonant Ore
- Deepslate Verdant Resonant Ore
- Infernal Resonant Ore
- Aetheric Resonant Ore
- Echoing Resonant Ore
- Four Resonant storage blocks
- Transmutation Table
- Arcane Transmutation Table
- Three fuel blocks (Alchemical Coal Block, Mobius Fuel Block, Aeternalis Fuel Block)
- Alchemical Hourglass
- Alchemical Anvil I–IV
- Purification Grindstone
- Portable Crafting Table
- Waypoint Anchor
- Matterburst TNT
- Matterburst Minecart
- Core Aura Machine
- Resonant Furnace I–IV
- Infernal Altar, Aetheric Altar, Deepbound Altar & Last Echo Altar

### Utility items & special conversions

- Attraction Catalyst
- Chalice of Transmutation
- Magic Mirror
- Void Translocator
- Cursed Igniter
- Eye of the Last Echo
- Eye of the Crucible
- Aetheric Bulwark Eye
- Deepbound Eye
- Purifying Milk
- Generic Core-bound weapons, tools and armor

### Content intentionally not present

The following older concepts were removed and are not part of current gameplay:

- Alchemical Dust & Alchemical Shears
- Tidal Heart & Bottomless Bucket
- Deepbound Chest, Barrel, Shulker Box & Ender Chest
- Tidal Conduit & Resonance Jukebox
- Separate Resonant Smoker & Resonant Blast Furnace (consolidated into Resonant Furnace I–IV)
- Far-Sight Glass, Bound Compass & Soulbound Recovery Compass
- Imbued Fishing Rod, Imbued Elytra & Imbued Turtle Helmet
- Resonant Beacon & Restorative Hearth
- Revealing Bell & Resonant Smithing Forge
- Verdant Ascension Template
- Passive EMC generation from Transmutation Tables
- Aegis Staff and Shield Staff

---

Velorise EMC is built around a simple rule: **everything may use EMC, but every system should still have a reason to explore, fight, build and progress.**
