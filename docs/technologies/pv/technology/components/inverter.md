# Inverter

## What does it do?

The inverter turns the 48 V DC from the battery into 230 V AC for normal appliances. Humasol projects mostly use an **inverter/charger** (Victron **MultiPlus-II**): besides inverting, it can also take AC from the grid or a generator, supply the loads with it and charge the battery. That makes it possible to turn an off-grid system into a hybrid one later without replacing the inverter ([Chaulmoogra](https://drive.google.com/file/d/1CjcOCPlSrWIydsPOc8KnPEB9xlv46_OT/view)).

## How large must it be?

The inverter is sized on **power**, not on energy: it must be able to deliver the **highest power that is used at the same moment**.

1. List all appliances with their power and when they are used, and find the hour with the highest total. Do not simply add up everything: the Chaulmoogra team made a load profile per 15 minutes with the partner and found a realistic peak of **3000 W**, much lower than all appliances together.
2. Look at the **continuous power** on the datasheet, not the VA rating. A MultiPlus-II 48/5000 delivers 4000 W continuously at 25 °C, but only 3700 W at 40 °C. In hot countries this matters.
3. Check the **start-up power** of motors and pumps.
4. If one inverter is not enough, Victron inverters can be put **in parallel** (or one per phase for three-phase).

Examples: MultiPlus-II 48/3000 in [Bagaya-Kapelle](https://drive.google.com/file/d/1cs9qv8PgYiXLEbxHEyLIqb_XVVOg6__H/view) and [Unikin](https://drive.google.com/file/d/13ijhU7CS5DQhFOQN78BsV6r1Wj9dtBYr/view); 48/5000 in [Chaulmoogra](https://drive.google.com/file/d/1CjcOCPlSrWIydsPOc8KnPEB9xlv46_OT/view); 48/10000 in [Ayonnah](https://drive.google.com/file/d/1WEOuCyAQanaq12DLHQQtdQrMjhzrDj8N/view); three 48/10000 units for the three-phase supply of [Apida](https://drive.google.com/file/d/1c8-2AVDGSzAgYXFXR_jMqJk__LChXEvR/view).

## Pure sine wave

Always use a **pure sine wave** inverter (all Victron models are). Cheap "modified sine" inverters cause problems with motors, pumps and sensitive electronics.

## The current on the battery side

The DC current between battery and inverter is large. For a 10 kW inverter at 48 V with 96 % efficiency: 10 000 ÷ (0.96 × 48) = **217 A**. That current determines the cable and fuse between busbar and inverter (see [4. Sizing](../sizing.md), step 6).
