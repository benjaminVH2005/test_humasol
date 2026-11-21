# Charge controller

## Info
Controls how the batteries are charged from the panels and protects them against overcharging.

## Relevant parameters

| Parameter | Meaning |
|---|---|
| Current (A) | Maximum charging current |
| Max. input voltage (V) | Must be higher than the Voc of the panel string |
| Type | MPPT or PWM |

## Types + comparison

| Type | Advantages | Disadvantages |
|---|---|---|
| MPPT | Gets more energy out of the panels | More expensive |
| PWM | Cheap, simple | Less efficient, panel voltage must match the battery |

## How to size it

1. Current ≥ panel power ÷ battery voltage × 1.25
2. Check the maximum input voltage on cold mornings

**Suppliers:** see the [central supplier list on the Drive](https://drive.google.com/), filter on *PV* and the component.
