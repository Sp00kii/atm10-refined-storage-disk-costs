# ATM10 — Fastest bulk resources for Refined Storage disks

Companion to [atm10-refined-storage-disk-costs.md](atm10-refined-storage-disk-costs.md).

For **700k+ quartz** (and the other RS disk mats), the answer in ATM10 is almost always **Mystical Agriculture + automation**, not more mining.

---

## TL;DR — best mods per resource

| Resource | Best mod(s) in ATM10 | Fastest method |
|----------|----------------------|----------------|
| **Quartz** | **Mystical Agriculture** + **Botany Pots Tiers** | Tiered pots (Ultra/Creative) + MA compat — usually beats field farms |
| **Quartz (RS shortcut)** | **Mystical Agriculture** | **Quartz Enriched Iron seeds** + **Silicon seeds** — skip raw quartz for parts |
| **Glass** | Mystical Agriculture / Create | Sand seeds → smelt; or Create sand washing + bulk smelting |
| **Redstone** | Mystical Agriculture | Redstone seeds |
| **Iron** | Mystical Agriculture + Mekanism | Iron seeds; optional 3x/5x ore processing for non-MA path |
| **String** | Mystical Agriculture | Cotton (or hemp/flax) seeds |
| **Slime** | Mystical Agriculture | Slime seeds |
| **Gold** | Mystical Agriculture | Gold seeds (tier 4) |
| **Diamonds** | Mystical Agriculture / Mekanism | Diamond seeds (tier 5) or Digital Miner |
| **Nether Stars** | Wither farm | Industrial Foregoing / RFTools / vanilla cage farm |

**Supporting mods:** Refined Storage (storage + autocraft), Mekanism (processing), Create (early bulk), Industrial Foregoing (harvesters), **Mining Dimension** (early manual ore).

**MA in pots (recommended if added):** Botany Pots + **Botany Pots — Mystical Agriculture Compat** + **Botany Pots Tiers**.

---

## Botany Pots Tiers vs growth accelerator fields

If you added **Botany Pots Tiers**, your instinct is **mostly correct** — it is often the faster path for bulk essence in ATM10.

### What Botany Pots Tiers does

| Pot tier | Growth speed | Output per harvest |
|----------|--------------|-------------------|
| Elite | 2× | 2× essence |
| Ultra | 6× | 6× essence |
| Creative | 10× | 10× essence |

Growth accelerators **do not** affect crops in pots — they only work on world-planted farmland. Pot speed comes from the **pot tier** + **soil tier** in the pot.

### Why pots usually win (especially Ultra / Creative)

1. **Output multiplier** — field farms only grow faster; they still drop ~1 essence per plant. Creative pots give **10× essence per harvest**. That alone is huge.
2. **Speed + output stack** — Creative is ~10× faster **and** ~10× yield → roughly **~100×** vs a basic botany pot on the same crop.
3. **Compact scaling** — tile hoppered pots in a grid; each pot is independent. No 60-block-deep accelerator pillars per crop.
4. **Less server load** — fewer crop block entities ticking in the world vs large 9×9 fields.
5. **Easier automation** — hopper pots → RS interface / drawer; no harvest pylon range or replant logic.

### When field farms can still compete

| Situation | Field farm advantage |
|-----------|---------------------|
| **Before Ultra/Creative pots** | Basic pots are slow; accelerator field + harvest pylon wins |
| **Huge horizontal scale** | Many 9×9 plots with max accelerators can match high pot counts |
| **Seed self-sufficiency** | Farmland can drop extra seeds / fertilized essence (pack-dependent) |
| **Crux crops** | Some crops need a crux block; pots accept crux as soil (+10% speed) |

### Optimal pot setup (for 700k quartz)

1. **Botany Pots — Mystical Agriculture Compat** (required for MA seeds in pots)
2. **Creative** or **Ultra** tier pots (Creative if craftable)
3. **Insanium farmland** as soil (+40% pot growth vs inferium soil)
4. **Hopper upgrade** on each pot → pipe to RS
5. Grow **Nether Quartz**, **Silicon**, or **Quartz Enriched Iron** seeds depending on what RS autocraft needs
6. Scale horizontally — **50–100+ pots** beats one “perfect” accelerator field for raw essence/hour

**Rough scale (Creative pot, tier 3 crop):** ~1 essence/sec per pot → **100 pots ≈ 360k essence/hour** (before autocraft). 700k quartz is a few hours of runtime, not days of mining.

### Verdict

| Method | Best for |
|--------|----------|
| **Botany Pots Tiers (Ultra/Creative)** | Bulk RS mats, compact bases, 700k+ quartz |
| **Growth accelerator + harvest pylon** | Early/mid MA, seed breeding, when pots aren’t tiered yet |
| **Both** | Pots for throughput; one small field for seed stock |

---

## #1 for 700k quartz: Mystical Agriculture farm

### Skip straight to RS crops (recommended)

ATM packs add seeds that feed **Refined Storage** directly:

- **Silicon seeds** — storage parts need lots of silicon
- **Quartz Enriched Iron seeds** — blocks + parts need QEI

Growing these is **faster than** farming nether quartz → crafting QEI/silicon by hand.

Check JEI for: `Silicon Seeds`, `Quartz Enriched Iron Seeds`.

### Nether Quartz seeds (if you need raw quartz)

| Step | What to do |
|------|------------|
| 1 | Progress MA: inferium → prosperity → **tier 3** altar |
| 2 | Craft **Nether Quartz seeds** (infusion altar + quartz) |
| 3 | **Preferred:** plant in **Creative/Ultra** botany pot with **Insanium farmland** soil |
| 3b | **Alt:** plant on **Essence Farmland** + growth accelerators + harvest pylon |
| 4 | Hopper pots → RS, or pylon → storage |
| 5 | RS autocraft essence → nether quartz (or grow QEI/Silicon seeds directly) |

**Throughput tips:**
- Use **Supremium** farmland + accelerators for endgame rates
- **Multiple 9×9 plots** beat one huge plot (easier to harvest)
- **Awakened / higher tier** seeds when available in pack
- Put **stack upgrades** on output barrels

**Rough scale:** One well-built MA plot produces thousands of essence per minute. For **700k quartz**, run **several parallel farms** + **RS autocraft** overnight rather than hand-crafting.

---

## Best automation mods (ATM10)

### Mystical Agriculture (primary)
- Grow almost every RS disk material as a crop
- Custom ATM10 crops: black quartz, certus, osmium, steel, etc.
- [ATM10 MA integration](https://deepwiki.com/AllTheMods/ATM-10/3.4-mystical-agriculture-integration)

### Mystical Agradditions / Harvest Pylon
- **Harvest Pylon** + hoes = hands-off crop collection
- Pair with growth accelerators under farmland

### Industrial Foregoing
- **Plant Sower** + **Plant Gatherer** for crop farms
- **Laser Drill** (late) for biome-specific ores — not for ATM ores

### Mekanism
- **Digital Miner** — diamonds, ores (not ATM tier ores)
- **Enrichment / crushing** — bonus yield on dusts
- **Factory** lines for silicon/QEI processing patterns

### Create
- Early **sand → glass**, **crushing**, **bulk smelting**
- Good before MA is online

### Refined Storage
- Store essences + autocraft processing chains
- **Pattern Grid** (processing mode): essence → quartz, quartz+iron → QEI, sand → glass
- Chain autocrafters for furnace / enrichment steps

### Mining Dimension (Aroma1997)
- Teleport pad → flat world full of normal ores
- Good **early** quartz/redstone/iron before MA

---

## Per-resource fast paths (for your disk table)

### Quartz (700k example)

**Path A — direct (best for RS):**
```
Quartz Enriched Iron seeds + Silicon seeds
  → essence → RS autocraft → storage parts
```

**Path B — raw quartz:**
```
Nether Quartz seeds → essence → nether quartz
  → (+ iron) → Quartz Enriched Iron
  → (+ silicon) → storage parts
```

**Path C — early game:**
- Nether mining + Fortune pick
- Mining dimension quartz veins
- Create crushing quartz ore

### Glass (731–177k per disk tier)

| Method | Notes |
|--------|-------|
| **Sand seeds** (MA) | Best long-term |
| Create + smelter | Sand washing → bulk furnace |
| RS pattern | Sand in → glass out (processing pattern) |

### Redstone

- **Redstone seeds** (MA tier 2) — trivial once MA is up
- Mining dimension / digital miner early

### Iron

- **Iron seeds** (MA tier 3)
- Mekanism ore multiplication if mining instead

### String

- **Cotton seeds** (MA) — check JEI exact name in ATM10

### Slime

- **Slime seeds** (MA)

### Gold & diamonds

| Tier | MA seed | Alt |
|------|---------|-----|
| Gold | Tier 4 gold seeds | Mining / laser drill |
| Diamonds | Tier 5 diamond seeds | Mek Digital Miner |

### Nether stars (256M = 4, 1048M = 16)

- **Wither farm** (mandatory for top disks)
- Industrial Foregoing wither builder or manual cage + spawner
- Stock **soul sand + skulls** early

---

## RS autocraft setup (minimal)

1. **Storage** — disks + external storage on MA farm output
2. **Processing patterns** (examples):
   - Nether quartz essence → nether quartz
   - 8 QEI essence → 8 quartz enriched iron (if MA recipe)
   - 3 iron + 1 quartz → 4 QEI (backup recipe)
   - Sand → glass (furnace)
   - Essence → resource for each crop
3. **Autocrafters** facing furnaces / machines
4. Request **1k storage part** — let RS chain subcrafts

**Tip:** Craft **lower disk tiers in batches** before requesting 256k+ — RS patterns often hang on one huge job.

---

## Suggested progression for a 1024k / 1048M disk

| Phase | Goal |
|-------|------|
| **1** | RS basic network + MA inferium/prosperity |
| **2** | Tier 3 seeds: iron, nether quartz, redstone, cotton |
| **3** | **Silicon + QEI seeds** — automate RS parts |
| **4** | Growth accelerator stack + harvest pylon |
| **5** | Gold/diamond seeds for higher disks |
| **6** | Wither farm before **256M** (needs nether stars) |
| **7** | Parallel MA plots + RS autocraft for **1048M** |

---

## What NOT to rely on for bulk quartz

| Method | Why |
|--------|-----|
| Hand mining nether | Too slow for 700k+ |
| Single Digital Miner | Good for ores, not MA-scale quartz |
| AE2 certus farm alone | Slower than MA in ATM packs ([ATM guides](https://allthemods.github.io/alltheguides/mods/ae2/setups/certusfarm/)) |
| One autocraft request for 1048M disk | Will stall — craft tiers in chunks |

---

## Links

- [ATM10 Mystical Agriculture (DeepWiki)](https://deepwiki.com/AllTheMods/ATM-10/3.4-mystical-agriculture-integration)
- [MA growth accelerators](https://blakesmods.com/wiki/1.19/mysticalagriculture/guides/speeding-up-crop-growth)
- [RS processing patterns](https://refinedmods.com/refined-storage/guides/processing-recipes.html)
- [ATM10 disk costs (this repo)](atm10-refined-storage-disk-costs.md)
