# Resonant Equipment & Arcane Weapons

## Resonant tools and armor

Each Resonant tier contains:

- Sword
- Pickaxe
- Axe
- Shovel
- Hoe
- Helmet
- Chestplate
- Leggings
- Boots

They use normal Vanilla-shaped crafting patterns with their matching ingot. They do not require separate Resonant smithing templates.

### Tool statistics

| Tier | Tool durability | Mining speed | Sword attack damage | Enchantability |
|---|---:|---:|---:|---:|
| Verdant | 1,800 | 8.5 | 7.5 | 12 |
| Infernal | 3,500 | 12.0 | 11.0 | 17 |
| Aetheric | 6,000 | 15.0 | 13.0 | 21 |
| Echoing | 10,000 | 18.0 | 15.0 | 26 |

### Armor statistics

The slot order below is Helmet / Chestplate / Leggings / Boots.

| Tier | Defense | Durability | Toughness | Knockback resistance per piece |
|---|---|---|---:|---:|
| Verdant | 3 / 8 / 6 / 3 | 310 / 451 / 423 / 366 | 2.5 | 0.05 |
| Infernal | 4 / 9 / 7 / 3 | 440 / 640 / 600 / 520 | 4.0 | 0.15 |
| Aetheric | 5 / 10 / 7 / 4 | 560 / 815 / 764 / 661 | 5.5 | 0.20 |
| Echoing | 6 / 11 / 8 / 5 | 760 / 1,105 / 1,036 / 899 | 7.5 | 0.25 |

### Full-set bonuses

Only a complete matching four-piece set activates its set bonus.

| Full set | Bonus |
|---|---|
| Verdant | Foundation equipment for the Resonance progression. |
| Infernal | 10% less incoming damage; +10% Inferno Rod, Ghastfire Staff and Wither Scepter power. |
| Aetheric | 20% less incoming damage; +10% Dragonfire and Shulker power; +10% Void Translocator range. |
| Echoing | 30% less incoming damage; +50% Resonant Echo power; +10% other Arcane Weapon power. |
| Echobound | 80% less incoming damage after normal armor reduction; Creative flight. |

The strongest matching damage-reduction set is applied once; reductions are not stacked together.

---

---

## Arcane Weapons

Arcane Weapons are crafted at Core I and upgraded through Alchemical Anvils. Their difficulty, ingredients and Core-I strength reflect the mob or location that inspired them. Higher Core tiers increase their signature mechanic as well as damage, range or duration.

Tooltips show:

- Current Core tier
- Damage or primary effect
- Range
- EMC cost
- Cooldown or reload behavior

### Shared staff recipe silhouette

Most Arcane Weapons use this shape:

```text
Empty | Optional material | Signature material
Empty | Wireless Core I   | Optional material
Stick | Empty             | Empty
```

Inferno Rod is the exception and uses a Fire Charge instead of a Stick.

### Complete weapon statistics

| Weapon | Core mechanic | Damage I / II / III / IV | Range I / II / III / IV | Default EMC | Main cooldown |
|---|---|---:|---:|---:|---:|
| Inferno Rod | Three rapid fire shots | 3 / 4 / 5 / 6 each | 10 / 15 / 20 / 25 | 128 / 256 / 512 / 1,024 per shot | 3 s after burst |
| Ghastfire Staff | Explosive fireball; radius 3 / 4 / 5 / 6 | 6 / 8 / 10 / 12 | 10 / 15 / 20 / 25 | 256 / 512 / 1,024 / 2,048 | 5 s |
| Dragonfire Scepter | Dragon fireball and five-second damage cloud | 8 / 12 / 16 / 20 direct | 15 / 20 / 25 / 30 | 256 / 512 / 1,024 / 2,048 | 6 s |
| Resonant Echo | Charged piercing sonic beam | 10 / 15 / 20 / 25 | 16 fixed | 512 / 1,024 / 2,048 / 4,096 | 6 s |
| Wither Scepter | Two casts; 1 / 2 / 3 / 4 skulls per cast | 7 / 10 / 13 / 16 each | 15 / 20 / 25 / 30 | 384 / 768 / 1,536 / 3,072 per cast | 5 s after second cast |
| Shulker Launcher | 1 / 2 / 3 / 4 manually aimed bolts | 4 each | 14 / 18 / 22 / 26 | 256 / 384 / 512 / 768 | 4 s |
| Guardian Lens | Channeled precision beam | 6 / 9 / 12 / 15 per damage step | 14 / 18 / 22 / 26 | 24 / 48 / 96 / 192 EMC/s | 3 s |
| Evoker Fang Staff | Five fang positions repeated for 1 / 2 / 3 / 4 waves | Vanilla fang damage | 8 / 11 / 14 / 17 | 384 / 768 / 1,536 / 3,072 | 5 s |
| Stormcaller | 1 / 2 / 3 / 4 lightning calls before reload | 8 / 11 / 14 / 17 | 16 / 20 / 24 / 28 | 1,024 / 2,048 / 4,096 / 8,192 per call | 8 s after final call |
| Frostbolt Wand | 1 / 2 / 3 / 4 slowing shots before recovery | 3 / 5 / 7 / 9 | 18 / 22 / 26 / 30 | 64 / 128 / 256 / 512 per shot | 1.5 s after final shot |
| Webcaster | Three shots; temporary web and venom | Poison I / I / I / II | 16 / 20 / 24 / 28 | 64 / 128 / 256 / 512 per shot | 3 s after burst |

### Inferno Rod

Recipe:

```text
Empty       | Blaze Rod       | Blaze Rod
Empty       | Wireless Core I | Blaze Rod
Fire Charge | Empty           | Empty
```

Behavior:

- Fires three small projectiles in a rapid burst.
- Ignites before applying direct damage.
- Burn duration is five seconds.
- Full Infernal armor increases its power by 10%.

### Ghastfire Staff

Recipe:

```text
Empty | Fire Charge     | Ghast Tear
Empty | Wireless Core I | Gunpowder
Stick | Empty           | Empty
```

Behavior:

- Fires an explosive Ghast-style projectile.
- Blast radius grows from 3 to 6 blocks.
- Ignites before direct damage.
- Full Infernal armor increases power by 10%.

### Dragonfire Scepter

Recipe:

```text
Empty | Dragon's Breath | Dragon Head
Empty | Wireless Core I | Fire Charge
Stick | Empty           | Empty
```

Behavior:

- Fires a Dragon-style projectile.
- Creates a five-second pulsing cloud.
- The cloud pulses every 0.5 seconds at a fraction of direct damage.
- Full Aetheric armor increases power by 10%.

### Resonant Echo

Recipe:

```text
Empty | Echo Shard      | Recovery Compass
Empty | Wireless Core I | Echo Shard
Stick | Empty           | Empty
```

Behavior:

- Charges for one second.
- Fires a piercing sonic beam through targets.
- Fixed 16-block range.
- Full Echoing armor increases its damage by 50%.

This is separate from the post-boss Echobound Greatsword. The Greatsword has its own much wider endgame Sonic Boom.

### Wither Scepter

Recipe:

```text
Empty | Wither Skeleton Skull | Wither Skeleton Skull
Empty | Wireless Core I       | Wither Skeleton Skull
Stick | Empty                 | Empty
```

Behavior:

- Allows two activations before its main cooldown.
- Each activation fires 1 / 2 / 3 / 4 skulls by Core tier.
- Applies Wither for 4 / 5 / 6 / 7 seconds.
- Skull explosion radius grows slightly by tier.
- Full Infernal armor increases power by 10%.

At Core IV, two complete casts release eight skulls before reload.

### Shulker Launcher

Registry ID: `velorise_emc:shulker_seeker`.

Recipe:

```text
Empty | End Rod         | Shulker Shell
Empty | Wireless Core I | Popped Chorus Fruit
Stick | Empty           | Empty
```

Behavior:

- Bolts are aimed by the player and do not automatically seek targets.
- Fires 1 / 2 / 3 / 4 bolts by Core tier.
- Every bolt deals 4 damage.
- Levitation lasts 3 / 4 / 5 / 6 seconds.
- Full Aetheric armor increases power by 10%.

### Guardian Lens

Recipe:

```text
Empty | Prismarine Crystals | Heart of the Sea
Empty | Wireless Core I     | Nautilus Shell
Stick | Empty               | Empty
```

Behavior:

- Channels a Guardian-style beam while held on a target.
- Maximum channel duration is 6 / 8 / 10 / 12 seconds.
- Charges EMC continuously while the beam operates.
- Cooldown begins after the channel ends.

### Evoker Fang Staff

Recipe:

```text
Empty | Bone Block      | Totem of Undying
Empty | Wireless Core I | Emerald Block
Stick | Empty           | Empty
```

Behavior:

- Chooses five fang positions once.
- Repeats the exact same positions for 1 / 2 / 3 / 4 delayed waves.
- Higher tiers do not extend the line farther; they repeat the original attack area.

### Stormcaller

Recipe:

```text
Empty | Lightning Rod   | Trident
Empty | Wireless Core I | Copper Block
Stick | Empty           | Empty
```

Behavior:

- Allows 1 / 2 / 3 / 4 calls before the main reload.
- Damages and ignites targets in a small Core-scaled area.
- The displayed lightning remains controlled and does not freely ignite structures.
- Creepers struck by Stormcaller can become charged Creepers.

### Frostbolt Wand

Recipe:

```text
Empty | Snowball        | Blue Ice
Empty | Wireless Core I | Amethyst Shard
Stick | Empty           | Empty
```

Behavior:

- Allows 1 / 2 / 3 / 4 rapid shots before recovery.
- Slowness lasts 3 / 4 / 5 / 6 seconds.
- Cheap per shot, intended for repeated single-target control.

### Webcaster

Recipe:

```text
Empty | Cobweb          | Fermented Spider Eye
Empty | Wireless Core I | Cobweb
Stick | Empty           | Empty
```

Behavior:

- Fires three shots before its normal cooldown.
- Creates temporary cobweb terrain for 15 / 30 / 45 / 60 seconds.
- Venom remains active for only 6 / 9 / 12 / 15 seconds.
- Core I–III apply Poison I.
- Core IV applies Poison II.
- Overlapping webs refresh the strongest valid effect instead of stacking repeated damage every tick.

### Armor synergy summary

| Armor | Arcane synergy |
|---|---|
| Infernal | +10% Inferno, Ghastfire and Wither power |
| Aetheric | +10% Dragonfire and Shulker power |
| Echoing | +50% Resonant Echo; +10% all other Arcane Weapons |
| Echobound | Counts as the strongest Echoing-family set for Arcane multipliers |

---
