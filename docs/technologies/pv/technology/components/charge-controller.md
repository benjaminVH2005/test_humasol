# Charge controller

## Info
Charges the batteries from the panels and protects them against overcharging.

## Relevant parameters

| Parameter | Meaning |
|---|---|
| Max. PV input voltage | Must be higher than the Voc of the panel string, also on cold mornings |
| Max. charge current | Determines how much PV power one controller can handle |
| Type | MPPT or PWM |

## Types + comparison

| Type | Advantages | Disadvantages |
|---|---|---|
| MPPT | Gets more energy out of the panels, allows higher string voltages | More expensive |
| PWM | Cheap, simple | Less efficient |

Humasol projects used **MPPT** controllers, mostly **Victron SmartSolar MPPT 250/85 or 250/100** (e.g. [Kiyodel](https://drive.google.com/file/d/124zqvYch7JHpEYUP_ul1__plQ9Rwe_94/view), [Ayonnah](https://drive.google.com/file/d/1WEOuCyAQanaq12DLHQQtdQrMjhzrDj8N/view), [Chaulmoogra](https://drive.google.com/file/d/1CjcOCPlSrWIydsPOc8KnPEB9xlv46_OT/view), [Hope for Girls & Women](https://drive.google.com/file/d/1Hf7LYZVS5rYBWHYoIerWkpYfLCCgrHsf/view)). Larger systems use several controllers in parallel.

## How to size it
1. Max. string voltage (Voc × number of panels in series, corrected for cold) < max. PV input voltage
2. Charge current ≈ PV power ÷ battery voltage, with a margin
