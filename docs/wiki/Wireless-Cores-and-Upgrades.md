# Wireless Cores, Anvils & Upgrades

## Wireless Cores

Wireless Cores are the main upgrade currency for equipment, machines and utility items.

### Core I recipe

```text
Diamond    | Ender Pearl           | Diamond
Ender Pearl| Verdant Resonant Ore  | Ender Pearl
Diamond    | Ender Pearl           | Diamond
```

Core I has a fixed EMC value of **67,584**.

### Nine-to-one condensation

Every Condensed Core requires nine matching Wireless Cores:

```text
Core | Core | Core
Core | Core | Core
Core | Core | Core
```

Nine matching Condensed Cores create a Condensed Core Generator block.

### Core-bound equipment bonuses

Core upgrades are passive. They do not require an operating mode and do not continuously drain EMC.

| Core | Damage bonus | Armor per piece | EMC repair cost per durability |
|---|---:|---:|---:|
| I | +1 | +1 | 64 |
| II | +2 | +2 | 32 |
| III | +4 | +4 | 16 |
| IV | +8 | +8 | 8 |

Core binding does not increase the mining speed or mining tier of ordinary pickaxes, axes, shovels or other tools. Its universal tool benefit is EMC repair; damage-capable items also receive the configured damage bonus. The Echobound Pickaxe is a separate post-boss item whose universal near-instant mining is intrinsic to that pickaxe, not granted by a Core.

### Core ascension chain

Core II–IV use the Vanilla Smithing Table.

| Result | Template | Base | Addition | Fixed result EMC |
|---|---|---|---|---:|
| Core II | Infernal Ascension Template | Condensed Core I | Alchemical Coal Block | 719,328 |
| Core III | End Ascension Template | Condensed Core II | Mobius Fuel Block | 6,685,440 |
| Core IV | Deep Convergence Template | Condensed Core III | Aeternalis Fuel Block | 60,709,152 |

### Ascension templates

#### Infernal Ascension Template

Uses a Netherite Upgrade Smithing Template in the center, surrounded by:

- Blaze Rod
- Ghast Tear
- Magma Cream
- Crying Obsidian
- Wither Skeleton Skull
- Ancient Debris
- Nether Wart
- Gilded Blackstone

Fixed EMC: **106,464**.

#### End Ascension Template

Uses the Infernal Ascension Template in the center, surrounded by:

- Dragon's Breath
- Shulker Shell
- Dragon Head
- End Crystal
- Chorus Flower
- End Rod
- Purpur Block
- Spire Armor Trim Smithing Template

Fixed EMC: **193,056**.

#### Deep Convergence Template

Uses the End Ascension Template in the center, surrounded by:

- Echo Shard
- Recovery Compass
- Disc Fragment 5
- Sculk Catalyst
- Silence Armor Trim Smithing Template
- Heart of the Sea
- Sponge
- Tide Armor Trim Smithing Template

Fixed EMC: **466,464**.

### Condensed Core Generators

A Condensed Core Generator produces EMC only for eligible Survival players standing within a three-block cube around it.

| Generator | Total output per second |
|---|---:|
| Condensed Core Generator I | 256 EMC/s |
| Condensed Core Generator II | 2,304 EMC/s |
| Condensed Core Generator III | 20,736 EMC/s |
| Condensed Core Generator IV | 186,624 EMC/s |

Rules:

- Creative and Spectator players do not receive output.
- A generator has one fixed total output.
- Nearby eligible players split that output instead of duplicating it.
- Multiple nearby generators can contribute independently.
- The player must remain close; these are not unlimited chunk-wide generators.

---

---

## Alchemical Anvils and Core installation

### Creating the anvil line

The four Alchemical Anvils are crafted as shapeless recipes. They are not created inside a Vanilla Anvil:

| Ingredients | Result |
|---|---|
| Vanilla Anvil + Core I | Alchemical Anvil I |
| Alchemical Anvil I + Core II | Alchemical Anvil II |
| Alchemical Anvil II + Core III | Alchemical Anvil III |
| Alchemical Anvil III + Core IV | Alchemical Anvil IV |

An Alchemical Anvil:

- Does not degrade through use.
- Removes the Vanilla “Too Expensive!” limit.
- Can pay missing experience levels with EMC.
- Charges 128 EMC per missing level by default.
- Gates the highest Core tier that may be installed.

### Exact station tiers

| Core being installed | Required station |
|---|---|
| Core I | Alchemical Anvil I |
| Core II | Alchemical Anvil II |
| Core III | Alchemical Anvil III |
| Core IV | Alchemical Anvil IV |

The tier must match exactly. A Vanilla Anvil cannot install a Core, and a lower or higher Alchemical Anvil cannot substitute. The corresponding World Tier must also be unlocked.

### Sequential upgrades

Most already-upgraded equipment and machines must progress one Core at a time.

Special cases:

- Matterburst TNT and Matterburst Minecart can be created directly at the inserted Core tier.
- Crafted Arcane Weapons begin at Core I and must advance one tier at a time in the exactly matching Alchemical Anvil.
- Fixed Core-I portable workstations do not store upgrade tiers.

### Shared passive Core bonuses

| Core | Damage bonus when the item deals damage | Armor per piece | EMC repair cost per durability |
|---|---:|---:|---:|
| I | +1 | +1 | 64 EMC |
| II | +2 | +2 | 32 EMC |
| III | +4 | +4 | 16 EMC |
| IV | +8 | +8 | 8 EMC |

Core upgrades normally increase capability rather than reducing the unit cost of the same action.

---

---

## Universal Core upgrades

Many Vanilla and compatible modded items can be imbued through an Alchemical Anvil.

### Generic damageable equipment

Eligible weapons, tools and armor can receive:

- Core tier data
- Passive weapon damage
- Armor bonus
- EMC repair
- Active mode where the item category supports it

Core binding does not make normal pickaxes, axes or shovels mine faster. Server compatibility lists can force specific modded items to be included or restricted to repair-only behavior.

### Core-bound hoes

A mature-crop harvest expands by Core tier:

| Core | Harvest area |
|---|---:|
| I | 3×3 |
| II | 5×5 |
| III | 7×7 |
| IV | 9×9 |

Only successful mature-crop interactions are processed.

### Imbued Fishing Rod

A successful catch creates more catch output while charging one fixed successful-catch price.

| Core | Catch output |
|---|---:|
| I | 2× |
| II | 4× |
| III | 8× |
| IV | 16× |

Default successful-catch cost: **256 EMC**.

### Imbued Elytra

The Elytra boost key applies a forward impulse while gliding.

| Core | Boost impulse |
|---|---:|
| I | 0.90 |
| II | 1.10 |
| III | 1.35 |
| IV | 1.65 |

- Cooldown: 3 seconds.
- EMC cost: the current EMC value of one Firework Rocket per successful boost.
- The Elytra also receives the normal Core armor bonus.

### Imbued Turtle Helmet

Activation costs **2,048 EMC** and grants:

- Water Breathing for 60 seconds
- Dolphin's Grace for 30 seconds

### Far-Sight Glass

A Core-I Spyglass conversion with mouse-wheel zoom while in use. It has no artificial gameplay zoom cap.

### Bound Compass

A Core-I Compass conversion that locks to a chosen block position.

Default lock cost: **256 EMC**.

### Soulbound Recovery Compass

A Core-I Recovery Compass conversion that channels toward the player's stored death position.

- Channel time: 3 seconds.
- Movement tolerance: 0.5 blocks.
- Cooldown: 15 seconds.
- Cost: distance-based EMC plus a cross-dimension surcharge when applicable.
- The destination safety search checks a small horizontal and vertical area.

### Cursed Igniter

Created by applying Core I to Flint and Steel.

- Places custom blue Soul Fire on valid blocks.
- Block placement has no durability loss and no normal block-use cooldown.
- Entity ignition costs 1,024 EMC at every tier.
- Entity cooldown: 6 seconds.

| Core | Direct damage | Burn duration |
|---|---:|---:|
| I | 4 | 5 s |
| II | 8 | 8 s |
| III | 12 | 12 s |
| IV | 16 | 16 s |

Fire-based Arcane attacks ignite targets before damage, allowing supported food-dropping mobs to produce cooked drops when killed by the attack.

---
