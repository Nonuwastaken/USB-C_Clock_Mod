# USB-C Clock Mod

A mechanical wall clock, originally battery-powered, modified to run off USB-C wall power instead — re-engineered from the movement's power requirements up, without altering the original gear mechanism.

## Motivation

The clock's gear-driven movement drew enough current that its battery needed replacing far too often for a wall clock that just sits and ticks. Rather than keep buying batteries, I decided to re-engineer its power path so it could run directly off wall power through a standard USB-C cable — a small, practical excuse to apply power electronics skills to an everyday object instead of letting it keep eating batteries.

## What it does

- Runs the clock off wall power via a USB-C cable, instead of a AA/coin cell battery
- Keeps the original mechanical gear-driven movement completely unchanged — only the power delivery was redesigned
- Regulates and steps down the incoming power to exactly what the movement's motor needs, so it runs at the correct speed without extra current draw or heat

## Resources

- Component List: [link]

## How it works

1. **Determined the movement's requirements:** Measured the clock's motor/movement operating voltage and current draw, since this wasn't documented anywhere.
2. **Designed the power path:** Used a buck converter (LM2596) to step down and regulate the input voltage to exactly what the movement needs, keeping the output stable regardless of USB-C source variation.
3. **Rewired the clock:** Removed the battery compartment's original contacts and wired the regulated output directly to the movement's power terminals, then routed a USB-C input into the clock's housing in place of the battery door.
4. **Validated:** Confirmed the movement ran at correct time-keeping speed on the new regulated supply, matching its original battery-driven behavior.

## Skills Involved

- **Power electronics:** buck converter-based voltage regulation to safely and efficiently step down input power to the movement's exact needs
- **Hands-on modification:** rewiring and repackaging an off-the-shelf product's internals to change its power source without damaging or altering its core mechanism

## Status

Complete — clock has been running on wall power via USB-C, with no battery replacements needed since the mod.
