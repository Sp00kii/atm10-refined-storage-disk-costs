# ATM10 — Refined Storage + Extra Disks: Craft Cost per Disk

Cumulative **raw material** totals to craft **one** storage disk of each tier from scratch.  
Includes **Refined Storage** (1k–64k) and **Extra Disks** (256k–1048M).

> **ATM10 note:** Extra Disks and ExtraStorage both add high-tier parts — recipes can conflict in autocrafting. In JEI, use the recipe swap button and pick **Extra Disks** parts when crafting 256k+ disks.

---

## Quick reference

| Disk tier | Item capacity | 1k storage parts needed |
|-----------|---------------|-------------------------|
| **1k** | 1,000 | **1** |
| **4k** | 4,000 | **4** |
| **16k** | 16,000 | **16** |
| **64k** | 64,000 | **64** |
| **256k** | 256,000 | **256** |
| **1024k** (1M) | 1,024,000 | **1,024** |
| **4096k** (4M) | 4,096,000 | **4,096** |
| **16384k** (16M) | 16,384,000 | **16,384** |
| **64M** | 65,536,000 | **65,536** |
| **256M** | 262,000,000 | **262,144** |
| **1048M** (1G) | 1,048,000,000 | **1,048,576** |

Each tier uses **4×** the previous tier’s storage part in the crafting chain (`4^n` base 1k parts).

---

## Full material table (per 1 disk)

| Disk tier | Capacity | Glass | Redstone | Iron | Quartz | String | Slime | Gold | Diamonds | Nether Stars | **Total** | **1k parts** |
|-----------|----------|------:|---------:|-----:|-------:|-------:|------:|-----:|---------:|-------------:|----------:|-------------:|
| 1k | 1,000 | 5 | 4 | 3 | 5 | 0 | 0 | 0 | 0 | 0 | **17** | **1** |
| 4k | 4,000 | 11 | 11 | 10 | 18 | 2 | 1 | 0 | 0 | 0 | **53** | **4** |
| 16k | 16,000 | 29 | 32 | 24 | 56 | 4 | 2 | 4 | 0 | 0 | **151** | **16** |
| 64k | 64,000 | 83 | 95 | 69 | 171 | 14 | 7 | 12 | 4 | 0 | **455** | **64** |
| 256k | 256,000 | 245 | 284 | 201 | 518 | 42 | 21 | 38 | 17 | 0 | **1,366** | **256** |
| 1024k | 1,024,000 | 731 | 851 | 600 | 1,551 | 122 | 61 | 110 | 53 | 0 | **4,079** | **1,024** |
| 4096k | 4,096,000 | 2,189 | 2,552 | 1,794 | 4,649 | 366 | 183 | 326 | 161 | 0 | **12,220** | **4,096** |
| 16384k | 16,384,000 | 6,563 | 7,655 | 5,379 | 13,944 | 1,094 | 547 | 974 | 485 | 0 | **36,641** | **16,384** |
| 64M | 65,536,000 | 19,685 | 22,964 | 16,131 | 41,828 | 3,282 | 1,641 | 2,918 | 1,457 | 0 | **109,906** | **65,536** |
| 256M | 262,000,000 | 59,051 | 68,891 | 48,390 | 125,440 | 9,842 | 4,921 | 8,750 | 4,369 | **4** | **329,658** | **262,144** |
| **1048M** | **1,048,000,000** | **177,149** | **206,672** | **145,152** | **376,384** | **29,526** | **14,763** | **26,246** | **13,105** | **16** | **989,013** | **1,048,576** |

---

## 1048M disk alone

To craft **one 1048M storage disk** from scratch:

| Resource | Amount |
|----------|-------:|
| Glass | 177,149 |
| Redstone | 206,672 |
| Iron | 145,152 |
| Quartz | 376,384 |
| String | 29,526 |
| Slime | 14,763 |
| Gold | 26,246 |
| Diamonds | 13,105 |
| Nether Stars | 16 |
| **1k storage parts** (equivalent in chain) | **1,048,576** |
| **Total resource count** | **989,013** |

---

## Crafting chain (concept)

```
1k part
 └─×4→ 4k part
      └─×4→ 16k part
           └─×4→ 64k part
                └─×4→ 256k part (Extra Disks)
                     └─×4→ 1024k part
                          └─×4→ 4096k part
                               └─×4→ 16384k part
                                    └─×4→ 64M part
                                         └─×4→ 256M part
                                              └─×4→ 1048M part
```

Each **storage disk** = **1 storage part** + **1 storage housing** (shapeless).

---

## Tips for ATM10

- Craft **lower tiers in batches** before autocrafting 256k+ — patterns often hang on one big request.
- **256M** needs **4 nether stars**; **1048M** needs **16 nether stars** — plan ahead.
- Upgrade existing disks: combine a lower disk + higher **storage part** in a grid; the old part is returned ([RS2 upgrade](https://refinedmods.com/refined-storage/news/20250308-whats-new-in-refined-storage-2.html)).
- Verify recipes in **JEI** on your pack version — ATM10 may tweak costs between updates.
