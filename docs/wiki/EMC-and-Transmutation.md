# EMC, Transmutation & Alchemical Fuel

## EMC and transmutation

### Personal EMC fund

Every player has a personal EMC account. The account is not stored inside one specific table, so the same balance is available through:

- Transmutation Table
- Arcane Transmutation Table
- Transmutation Tablet
- EMC Hub and HUD systems
- EMC-powered equipment and utility actions

Machine buffers are separate. Fuel placed into a machine belongs to that machine until used or recovered through its normal interaction rules.

### Burning items

Burning an item converts it into EMC and teaches that item when the server policy allows it.

Important rules:

- The item must have a positive EMC value.
- Blacklisted or non-materializable items may be prevented from being learned or recreated.
- Damaged items can be valued according to remaining durability.
- Stored EMC inside supported containers or equipment is handled by the relevant item logic.
- Enchantments do not automatically create extra resale value.

### Learning items

Once an item is learned, it can appear in the player's Transmutation interface and be recreated by spending EMC.

The learned-item system is personal. Two players do not automatically share knowledge.

### Materializing items

Materialization consumes the item's EMC value plus any active tax surcharge. The operation fails cleanly if the player cannot afford the complete cost.

Materialization does not create negative EMC and does not partially create an unaffordable stack.

### Default and Balanced value modes

The server selects one of two EMC value profiles:

| Mode | Purpose |
|---|---|
| Default | A permissive ProjectE-like economy with broad access to powerful conversions. |
| Balanced | Revalues important items, enables materialization tax by default and reduces easy inflation loops. |

Examples from the Balanced profile:

| Item | EMC |
|---|---:|
| Emerald | 512 |
| Diamond | 4,096 |

The server may also define custom EMC values, item blacklists and materialization permissions.

### Materialization tax

Balanced Mode enables a personal tax meter by default.

- Every materialized item adds one point.
- The meter recovers one point per real-time second.
- Tax never disables materialization.
- The current bracket adds a flat EMC surcharge to every created item.

| Tax points | Extra EMC per item |
|---:|---:|
| 0–64 | 0 |
| 65–128 | 2 |
| 129–256 | 4 |
| 257–512 | 8 |
| 513–1,024 | 32 |
| Above 1,024 | 64 |

This slows extreme bulk conversion without preventing ordinary use.

### Transmutation content

| Item or block | Function |
|---|---|
| Philosopher's Stone | Reusable crafting catalyst and block-transmutation tool. |
| Transmutation Table | Main personal EMC, learning and materialization interface. |
| Arcane Transmutation Table | Larger interface with double inventory space and integrated crafting access. |
| Transmutation Tablet | Portable Transmutation interface. |
| Tome of Knowledge | Consumed to learn every item currently permitted by the server EMC policy. |
| Knowledge Sharing Book | Stores one player's permitted learned-item list and imports it through a Transmutation interface. |

Neither Transmutation Table generates passive EMC.

### Knowledge Sharing Book

An empty Knowledge Sharing Book can be filled with the owner's permitted learned items by **Shift + Right-clicking** it.

A written book stores:

- Owner name
- Learned item registry IDs
- Number of stored entries

Use the written book through a Transmutation interface to import its permitted knowledge. The receiving server still applies its own current EMC policy.

---

---

## Philosopher's Stone

### Recipe

```text
Glowstone Dust | Redstone       | Glowstone Dust
Redstone       | Diamond        | Redstone
Glowstone Dust | Redstone       | Glowstone Dust
```

The Philosopher's Stone is reusable in supported crafting recipes and returns to the crafting grid instead of being consumed.

### Block transmutation

Right-click a supported block to cycle it into the next block in its family.

Supported families include:

- Wood planks
- Logs and stems
- Stripped logs and stems
- Wood blocks
- Leaves
- Saplings
- Wool and carpet colors
- Concrete and concrete powder colors
- Terracotta and glazed terracotta colors
- Stained glass and panes
- Candles
- Shulker box colors
- Stone and stone-brick variants
- Sandstone and red sandstone variants
- Dirt and soil variants
- Sand, red sand and gravel
- Ice variants
- Deepslate variants
- Quartz variants
- Copper oxidation and cut variants
- Nether and blackstone variants
- Prismarine variants
- Sponge and wet sponge

If the target block is worth more EMC than the source block, the Stone charges only the positive difference. Conversions to equal or cheaper blocks do not create an EMC refund.

Log and pillar orientation is preserved when both blocks support the same axis property.

---

---

## Alchemical fuel

The Philosopher's Stone is the reusable catalyst for the fuel chain.

| Fuel | Recipe | EMC | Burn time |
|---|---|---:|---:|
| Alchemical Coal | 4 Coal + Philosopher's Stone | 512 | 12,800 ticks |
| Mobius Fuel | 4 Alchemical Coal + Philosopher's Stone | 2,048 | 102,400 ticks |
| Aeternalis Fuel | 4 Mobius Fuel + Philosopher's Stone | 8,192 | 819,200 ticks |

Nine fuel items form the matching fuel block. Fuel blocks can also be unpacked.

| Fuel block | EMC |
|---|---:|
| Alchemical Coal Block | 4,608 |
| Mobius Fuel Block | 18,432 |
| Aeternalis Fuel Block | 73,728 |

These fuels work in Vanilla-compatible fuel slots, including every Resonant Furnace-family machine.

---
