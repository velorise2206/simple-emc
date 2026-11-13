# World Tiers, Resonant Ores & Spires

## World Tier progression

The world has four shared progression stages. Each stage unlocks a Wireless Core tier and a Resonant material tier.

### World Tier requirements

| World Tier | Default objectives | Unlock |
|---|---|---|
| I — Overworld Hunt | 180 total hostile kills; Zombie family 40; Skeleton family 35; Spider family 25; Creeper 20; Enderman 8; Witch 5; Illager 12 | Core I and Verdant Resonance |
| II — Nether Conquest | 180 total Nether hostile kills; Piglin family 35; Zombified Piglin 40; Blaze 25; Magma Cube 20; Ghast 8; Wither Skeleton 20; Wither 1 | Core II and Infernal Resonance |
| III — End Conquest | Enderman 50; Shulker 20; Ender Dragon 1 | Core III and Aetheric Resonance |
| IV — Deep World Conquest | Guardian 40; Elder Guardian 3; Warden 1 | Core IV, Echoing Resonance and the Last Echo route |

### Multiplayer contribution scaling

Default progression scaling is multiplicative:

```text
Requirement × 1.20^(additional contributors)
```

The final scale is capped at 3× by default. Boss objectives do not scale unless the server enables that option.

The server can change:

- Scaling mode: none, linear or multiplicative
- Per-player multiplier
- Maximum scale
- Maximum counted contributors
- Whether boss objectives scale
- Every individual kill requirement

### World Progress screen

A book button in the Transmutation interface opens the read-only World Progress screen.

It shows:

- Current World Tier
- Every objective and current count
- Contributor scaling
- Next Wireless Core unlock
- Progress shared by the current world/server

### Retrogen and existing worlds

Unlocking a World Tier does not require creating a new world.

The mod applies deterministic Resonant ore retrogen to existing chunks and marks processed chunks by tier. Newly unlocked ore can therefore appear in previously explored areas without repeatedly reprocessing the same tier.

---

---

## Resonant ores and materials

### Ore tiers

| Tier | Dimension and region | Required pickaxe | Raw/ore EMC | Ingot EMC | Cooking time |
|---|---|---|---:|---:|---:|
| Verdant | Overworld stone and deepslate | Diamond, Netherite or Verdant+ | 32,768 | 33,024 | 200 ticks / 10 s |
| Infernal | Nether | Netherite or Verdant+ | 65,536 | 66,048 | 400 ticks / 20 s |
| Aetheric | End | Infernal+ | 131,072 | 132,096 | 800 ticks / 40 s |
| Echoing | Deep Overworld | Aetheric+ | 262,144 | 264,192 | 1,600 ticks / 80 s |

Every ore drops its matching raw material.

- Fortune can increase the drop.
- Final output is capped at four raw items per ore.
- Silk Touch returns the ore block.
- Ore and raw material can be cooked in a Furnace, Blast Furnace or Smoker.

### Storage blocks

Nine ingots form one storage block.

| Block | EMC |
|---|---:|
| Verdant Resonant Block | 297,216 |
| Infernal Resonant Block | 594,432 |
| Aetheric Resonant Block | 1,188,864 |
| Echoing Resonant Block | 2,377,728 |

Infernal, Aetheric and Echoing material items are fire resistant. Verdant remains burnable.

---

---

## Resonance Spires

Resonance Spires are world-generated EMC structures activated by World Tier.

They alternate between an active output phase and a recharge phase.

| Tier | Reserve | Output per nearby player per second | Radius | Siphon damage per second | Default spacing |
|---|---:|---:|---:|---:|---:|
| I | 1,228,800 | 2,048 | 8 | 1 | 600 blocks |
| II | 4,915,200 | 8,192 | 12 | 2 | 1,000 blocks |
| III | 19,660,800 | 32,768 | 16 | 4 | 1,500 blocks |
| IV | 78,643,200 | 131,072 | 24 | 8 | 2,000 blocks |

Default cycle:

- Approximately 10 active minutes.
- Approximately 10 recharge minutes.
- During recharge, nearby players may suffer **Vital Siphon**.

Other defaults:

- No Spire within 256 blocks of world spawn.
- 50% deterministic chance for a Tier IV Spire at an Ancient City structure start.

World Spires and Condensed Core Generators are separate systems. Spires are progression structures; Condensed Core Generators are player-crafted short-range blocks.

---

---

## World Threat and multiplayer scaling

### World Threat

Hostile mobs can become stronger as World Tier increases.

Default scaling:

- +10 maximum health per World Tier.
- +2 attack damage per World Tier.
- Existing low-health mobs preserve at least half-health proportionality when scaling is applied.
- Modded hostile mobs are included by default unless excluded by server configuration.

Eligible Vanilla hostile mobs may also spawn with legal Vanilla equipment and enchantments based on World Tier.

- Generated equipment has zero drop chance.
- Already-loaded mobs are not repeatedly upgraded.
- The system does not inject Velorise EMC equipment into ordinary mob loot.

### Boss player scaling

The Ender Dragon, Wither and Warden can scale with nearby eligible players.

Defaults:

- Enabled.
- Maximum counted players: 10.
- +100 health per counted player.
- +2 damage per counted player.

Advancements track defeating bosses at higher configured scaling levels.

---
