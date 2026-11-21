# Inverter

## Info
Converts the DC from the batteries into 230 V AC. Most Humasol projects used an **inverter/charger** (Victron MultiPlus-II), which can also charge the batteries from the grid or a generator.

## Relevant parameters

| Parameter | Meaning |
|---|---|
| Continuous power | What the inverter can always deliver |
| Peak (surge) power | For start-up currents of motors and pumps |
| Battery voltage | Must match the battery bank (Humasol mostly used 48 V) |
| AC input | Whether the grid or a generator can be connected (hybrid) |

## Types + comparison

| Type | Advantages | Disadvantages |
|---|---|---|
| Pure sine wave | Works with all appliances | More expensive |
| Modified sine wave | Cheap | Problems with motors and sensitive electronics |
| Inverter/charger (e.g. MultiPlus-II) | Also charges from grid/generator, fits hybrid systems | More expensive than a simple inverter |

## What Humasol used

| Project | Inverter |
|---|---|
| [Bagaya-Kapelle](https://drive.google.com/file/d/1cs9qv8PgYiXLEbxHEyLIqb_XVVOg6__H/view) (2021-22), [Unikin](https://drive.google.com/file/d/13ijhU7CS5DQhFOQN78BsV6r1Wj9dtBYr/view) (2024-25) | MultiPlus-II 48/3000 |
| [Chaulmoogra](https://drive.google.com/file/d/1CjcOCPlSrWIydsPOc8KnPEB9xlv46_OT/view) (2025-26) | MultiPlus-II 48/5000 |
| [Ayonnah](https://drive.google.com/file/d/1WEOuCyAQanaq12DLHQQtdQrMjhzrDj8N/view) (2025-26) | MultiPlus-II 48/10000 |
| [Apida](https://drive.google.com/file/d/1c8-2AVDGSzAgYXFXR_jMqJk__LChXEvR/view) (2024-25) | 3 × MultiPlus-II 48/10000 (three-phase supply for a medical centre) |
| [Emergi](https://drive.google.com/file/d/1dvwuWhsSH8iRaCqRwZrG4B46ZKS-dGI-/view) (2025-26) | Full design: 3 × MultiPlus-II 48/10000 in parallel |

## How to size it
1. Add up the power of all appliances that run at the same time
2. Add a margin, and check the start-up (surge) power of motors and pumps
3. See [4. Sizing](../sizing.md)
