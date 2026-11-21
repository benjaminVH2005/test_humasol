# Solar panels

## What does a panel do?

A solar panel turns sunlight into DC electricity. Its output depends on the amount of sunlight, the temperature (hotter means less output) and whether it is clean and free of shade.

## The parameters on a datasheet

When you compare panels, you will find these values on the datasheet. As an example, the 550 Wp panels used in [Emergi](https://drive.google.com/file/d/1dvwuWhsSH8iRaCqRwZrG4B46ZKS-dGI-/view):

| Parameter | Meaning | Emergi panel |
|---|---|---|
| Maximum power (Pmax) | Power under standard test conditions, in Wp | 550 Wp |
| Voltage at maximum power (Vmp) | Voltage while working normally | 40.9 V |
| Current at maximum power (Imp) | Current while working normally | 13.45 A |
| Open-circuit voltage (Voc) | Highest voltage, when nothing is connected. **Use this to check the charge controller's maximum voltage.** | 49.62 V |
| Short-circuit current (Isc) | Highest current. **Use this to size fuses.** | 14.03 A |
| Maximum series fuse rating | Largest fuse allowed per string | 25 A |

**Temperature matters.** On a cold morning the voltage of a panel is a few percent higher than on the datasheet; in the heat it is lower. The Chaulmoogra team calculated that a 10 °C colder panel gives about 3 % more voltage, and checked that their string still stayed below the controller limit.

## Monocrystalline or polycrystalline?

Recent Humasol projects all chose **monocrystalline** panels: they have a higher efficiency, need less roof space and are now about the same price per Wp as polycrystalline panels ([Chaulmoogra](https://drive.google.com/file/d/1CjcOCPlSrWIydsPOc8KnPEB9xlv46_OT/view)).

## How do you choose a panel?

1. Ask **local suppliers** which panels they have. Availability decides a lot.
2. Prefer **higher-Wp panels** if the price per Wp is similar: you need fewer panels, fewer cables and less mounting material.
3. Check the **roof or ground space** and the **tilt**. Panels should face the equator; on a roof, the roof slope often fixes the tilt ([Kiyodel](https://drive.google.com/file/d/124zqvYch7JHpEYUP_ul1__plQ9Rwe_94/view) installed on a roof with a 34° slope).

How many panels you need, and how to connect them, is explained in [4. Sizing](../sizing.md).
