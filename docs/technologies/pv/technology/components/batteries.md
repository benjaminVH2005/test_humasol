# Batteries

## What does the battery do?

The battery stores the solar energy that is not used immediately, so it can be used in the evening, at night or on a cloudy day. It is usually the **most expensive part to replace** during the lifetime of a system, so choose it carefully.

## Lithium or lead-acid?

| | Lithium (LiFePO4) | Lead-acid (gel, AGM) |
|---|---|---|
| Usable part of the capacity (DoD) | 80–95 % | about 50 % |
| Lifetime | Long | Shorter |
| Price to buy | Higher | Lower, often available locally |

The **depth of discharge (DoD)** is the share of the battery you can really use without damaging it. This makes a big difference: in [Bagaya-Kapelle](https://drive.google.com/file/d/1cs9qv8PgYiXLEbxHEyLIqb_XVVOg6__H/view) four batteries gave 10 kWh of storage, but only **5 kWh** was usable because of the DoD. Most recent Humasol projects therefore chose **lithium**.

## Voltage

Humasol systems almost always use **48 V**. A higher voltage means a lower current for the same power, so thinner cables and smaller fuses.

## How much storage do you need?

First decide **what the battery has to cover**:

- **Off-grid:** the battery must cover the evening and night, and ideally a bad-weather day. As a first estimate you can take the full daily consumption: capacity (Ah) = daily energy (Wh) ÷ (battery voltage × DoD). The Chaulmoogra team found about 384 Ah at 48 V (about 18.5 kWh) this way.
- **Hybrid:** the grid is the backup, so the battery can be smaller, or even be added later ([Gitaru Marigu](https://drive.google.com/file/d/1D3iP_NHe1bnwG8g8spbsb6MS3Cgx5PEH/view)).
- Do **not** oversize: during the day the panels supply most loads directly, so the battery mainly has to cover the night. The Chaulmoogra simulation ended up with a smaller battery (15 kWh) than the simple estimate, and [Kiyodel](https://drive.google.com/file/d/124zqvYch7JHpEYUP_ul1__plQ9Rwe_94/view) also sized only for the night and bad-weather days.

## Battery current

Besides the energy, also check the **current**. The battery cables and fuses must handle the larger of:

- the **charge current**: all MPPTs together, plus the grid charger in a hybrid system;
- the **discharge current**: all inverters together at full power.

See [4. Sizing](../sizing.md), step 7, where this is worked out for Emergi (748 A, so two cables in parallel).

## Practical tip

Use battery modules that can be **extended later** with the same type. Emergi chose the same 5.1 kWh modules as the existing installation, because up to 63 of them can be connected in parallel.
