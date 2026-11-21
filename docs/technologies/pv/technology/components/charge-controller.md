# Charge controller (MPPT)

## What does it do?

The charge controller sits between the panels and the battery. It converts the high voltage of a string of panels into the right voltage to charge the battery, and stops charging when the battery is full.

An **MPPT** (Maximum Power Point Tracking) controller constantly looks for the voltage at which the panels give the most power. That gives clearly more energy than a cheaper PWM controller, and it allows you to put several panels in series. All recent Humasol projects used MPPT controllers, mostly the **Victron SmartSolar MPPT 250/100** or **250/85**.

## What do the numbers mean?

For a Victron **SmartSolar MPPT 250/100**:

- **250** = the maximum voltage that may ever come from the panels (250 V). If the string voltage goes above it, even on a cold morning, the controller can be damaged.
- **100** = the maximum current the controller delivers to the battery (100 A).
- From the datasheet: the recommended **maximum PV power** per controller, for a 48 V battery 5.8 kW.

## The three checks

For every controller you must check three things. The full calculation is in [4. Sizing](../sizing.md), step 5.

1. **Voltage:** the open-circuit voltage of one string (number of panels in series × Voc), also on a cold morning, must stay **below** the maximum input voltage.
2. **Power:** the panel power on one controller must stay below the recommended maximum. Victron allows the panels to be oversized up to about **130 %**, because panels rarely give their full Wp in practice ([Emergi](https://drive.google.com/file/d/1dvwuWhsSH8iRaCqRwZrG4B46ZKS-dGI-/view)).
3. **Short-circuit current:** the number of parallel strings × Isc must stay below the controller's maximum PV short-circuit current.

If one controller is not enough, use **several controllers in parallel**, each with its own group of panels. You can check your design with the free **Victron MPPT calculator** on the Victron website.
