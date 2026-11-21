# 4. Sizing

The method most Humasol teams used:

1. **Make a load table**: every appliance, its power (W) and how many hours a day it runs → daily energy need (kWh/day) and peak power (W)
2. **Reduce the demand where possible**: efficient appliances, and planning heavy loads (irons, pumps) during sunny hours
3. **Find the solar resource** for the site (peak sun hours, e.g. with PVGIS)
4. **Size the panels**: PV power ≈ daily need ÷ peak sun hours ÷ loss factor
5. **Size the batteries** from the hours they must cover and the DoD (see [Batteries](components/batteries.md))
6. **Size the inverter** on the peak power, and the **charge controllers** on PV power and string voltage
7. **Check the budget** and, if needed, build in phases

**Sizing tool:** [on the Drive](https://drive.google.com/) *(add link)*

## Examples from projects

| Project | Daily need | Result |
|---|---|---|
| [Ayonnah](https://drive.google.com/file/d/1WEOuCyAQanaq12DLHQQtdQrMjhzrDj8N/view) (2025-26) | about 26 kWh/day | 33 × 600 Wp panels and a 25 kWh battery |
| [Gitaru Marigu](https://drive.google.com/file/d/1D3iP_NHe1bnwG8g8spbsb6MS3Cgx5PEH/view) (2025-26) | about 18 kWh/day | about 8 × 620 W panels, hybrid with the grid, batteries later |
| [Kiyodel](https://drive.google.com/file/d/124zqvYch7JHpEYUP_ul1__plQ9Rwe_94/view) (2024-25) | max. 2500 W peak | 12 panels and 8 batteries, off-grid |
| [Emergi](https://drive.google.com/file/d/1dvwuWhsSH8iRaCqRwZrG4B46ZKS-dGI-/view) (2025-26) | Fleet of 28 electric three-wheelers | Full need 75 kWp PV, 96.9 kWh battery, 3 × MultiPlus-II 48/10000: built in two phases because of the budget |

!!! tip "Learn from Emergi"
    When the full system is too expensive, size the complete design anyway and **build it in phases**, so later teams can expand without redesigning.
