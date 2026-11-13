# Machines & Utility Items

## Utility items

### Attraction Catalyst

Right-click to toggle item and entity attraction.

| State | Area diameter |
|---|---:|
| No Core | 3 |
| Core I | 5 |
| Core II | 7 |
| Core III | 9 |
| Core IV | 11 |

- Cost: 8 EMC per active tick.
- Pull strength: 0.25 by default.
- Core increases area, not unit price.

Recipe:

```text
Iron Block     | Empty           | Iron Block
Redstone Block | Empty           | Lapis Block
Redstone Block | Wireless Core I | Lapis Block
```

### Chalice of Transmutation

Use directly on a growable block or fluid.

| State | Horizontal area |
|---|---:|
| No Core | 3×3 |
| Core I | 5×5 |
| Core II | 7×7 |
| Core III | 9×9 |
| Core IV | 11×11 |

Default costs:

- Grow one valid plant: 64 EMC
- Begin fluid-clearing operation: 200 EMC
- Water removed: 10 EMC per block
- Lava removed: 50 EMC per block
- Other supported fluid: 20 EMC per block

Only successful blocks are charged.

### Magic Mirror

Hold right-click for three seconds to return to:

- Bed spawn
- World spawn when no valid bed is available
- A linked Waypoint Anchor when using the alternate interaction

| Core | Same-dimension maximum range | EMC per block |
|---|---:|---:|
| I | 1,024 | 2.0 |
| II | 2,048 | 1.5 |
| III | 4,096 | 1.0 |
| IV | 8,192 | 0.5 |

- Cross-dimension surcharge: 2,500 EMC.
- Channel time: 3 seconds.
- Cooldown: 15 seconds.

### Waypoint Anchor

A placed destination that can be linked to the Magic Mirror.

Recipe materials:

- Obsidian around the edges
- Ender Pearl
- Wireless Core I
- Lodestone

### Void Translocator

Right-click to teleport safely in the direction you are looking.

| Core | Range |
|---|---:|
| I | 15 blocks |
| II | 20 blocks |
| III | 25 blocks |
| IV | 30 blocks |

- Cost: 1,024 EMC per use.
- Cooldown: 6 seconds.
- Full Aetheric or Echoing-family armor adds 10% range.

### Purifying Milk

A reusable Core-powered Milk Bucket conversion.

- Removes harmful effects according to the installed Core's eligibility.
- Fixed cost: 4,096 EMC per successful use.
- Higher Core tiers increase what may be removed rather than reducing the price.

### Portable workstations

These fixed Core-I utilities open their Vanilla-style menus while held and retain normal placed-block behavior:

- Resonant Crafting Table
- Portable Stonecutter
- Portable Loom
- Portable Cartography Table

They have no higher Core levels and do not scan nearby storage inventories.

---

---

## Machines and special blocks

### Resonant Furnace family

Core I applied to the matching Vanilla machine in an Alchemical Anvil creates:

- Resonant Furnace (`velorise_emc:resonant_furnace`)
- Resonant Smoker (`velorise_emc:resonant_smoker`)
- Resonant Blast Furnace (`velorise_emc:resonant_blast_furnace`)

Each family member uses one permanent registry ID. Core level is stored on the item and Block Entity, so separate `_i`, `_ii`, `_iii` and `_iv` block registrations are not used. Breaking and replacing the machine preserves its installed Core.

Upgrade each machine sequentially with Core II, III and IV in the matching Alchemical Anvil tier.

| Core | Cooking speed |
|---|---:|
| I | ×2 |
| II | ×4 |
| III | ×8 |
| IV | ×16 |

Rules:

- The fuel slot uses normal Vanilla fuel logic. Coal, wood, Alchemical Fuel and compatible modded fuels work normally.
- The family has no personal-EMC loading button and no local EMC heat buffer.
- Core level multiplies cooking progress; it does not duplicate output or alter recipe output count.
- Furnace uses smelting recipes.
- Smoker prefers smoking recipes and supports the shared smelting fallback implemented by the machine family.
- Blast Furnace prefers blasting recipes and supports the same smelting fallback.
- A valid recipe, fuel and enough output space are still required.
- Resonant ores may be processed in any compatible member of the family; ore tier is not gated by machine Core.
- The Vanilla flame and arrow progress animations are rendered on both Forge 1.20.1 and NeoForge 1.21.1.
- All three machines are exposed as JEI catalysts and appear in the Velorise EMC creative tab as Core I stacks.

### Alchemical Hourglass

The Hourglass uses a full three-dimensional frame, glass chamber and visible sand model. It accelerates compatible nearby machines once per second.

Default behavior:

- Local EMC capacity: 2,000,000.
- Pulse interval: 20 ticks.
- Adds a fixed +20 virtual machine ticks per pulse.
- Costs 2 EMC for each virtual tick that actually advances a target.
- Failed or ineligible targets are not charged.

| Core | Radius |
|---|---:|
| I | 4 blocks |
| II | 6 blocks |
| III | 8 blocks |
| IV | 10 blocks |

The crafting recipe already consumes Core I, so the Hourglass has no Core-0 variant. Existing untagged Hourglasses are normalized to Core I. Upgrade the same item sequentially with Core II-IV in the exactly matching Alchemical Anvil tier. Core increases reachable area, not the +20 tick bonus.

### Purification Grindstone

A Core-powered Grindstone conversion for extracting enchantments.

- Fixed cost: 8,096 EMC per successful operation.
- Core I can extract all normal enchantments from the primary item.
- Core II can extract one normal enchantment.
- Core III–IV unlock the second input slot for curse extraction.
- Extracted operations return experience according to the preview.
- The operation does not complete unless the player can afford the full EMC cost.

### Tidal Conduit

A Core-powered Conduit aura machine.

| Core | Range |
|---|---:|
| I | 32 blocks |
| II | 64 blocks |
| III | 96 blocks |
| IV | 128 blocks |

- Local EMC capacity: 2,000,000.
- Operating cost: 64 EMC per second.
- Pulses every 10 seconds and maintains an 11-second effect duration by default.

### Matterburst TNT and Minecart

A Core may be applied directly to TNT or TNT Minecart at any unlocked tier.

| Core | Excavation radius |
|---|---:|
| I | 4 |
| II | 8 |
| III | 16 |
| IV | 32 |

Default excavation profile:

- Depth multiplier: 0.625× radius
- Minimum depth: 3
- Entity damage radius: 1.5× excavation radius
- Base entity damage: 24
- Additional damage: 4 per radius block
- Work is spread across ticks to avoid deleting the full area in one server tick

Matterburst Minecart places a Core-tagged TNT Minecart on rails.

### Deepbound Ender Chest

A personal expanded Ender-linked storage block.

- Core I conversion from an Ender Chest.
- Storage follows the player rather than one physical chest.
- It is the only active Deepbound storage block in the current version.

### Resonance Jukebox

A Core-powered multi-disc Jukebox.

| Core | Accessible disc slots |
|---|---:|
| I | 8 |
| II | 12 |
| III | 16 |
| IV | 20 |

Features:

- Stacked duplicate discs are consolidated where possible.
- Play, stop, next and previous controls.
- Repeat modes.
- Shuffle.
- Adjustable volume from 10% to 100%.
- Redstone comparator output follows the selected disc.
- Local EMC capacity: 250,000.
- Default operating cost: 1 EMC per second.

The advancement **The World's Soundtrack** asks for every available music-disc type, capped at 20 distinct discs.

### Resonant Crafting Table

A fixed Core-I portable Crafting Table.

- Held use opens crafting.
- Placed use behaves like a normal crafting station.
- It does not access nearby inventories.
- It has no Core levels or range upgrade.

---
