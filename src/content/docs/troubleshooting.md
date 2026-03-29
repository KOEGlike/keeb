---
title: Troubleshooting
description: Common issues and how to fix them.
order: 5
---

## A Key Doesn't Work

1. Pull the keycap and switch
2. Check for bent switch pins — straighten with tweezers
3. Re-seat the switch firmly into the hot-swap socket
4. Test with a spare switch
5. If still dead, the hot-swap socket may need resoldering

## Multiple Keys Not Working

If an entire row or column is dead, it's likely a PCB issue:

- Check for cold solder joints on the controller
- Inspect the PCB for cracks or damaged traces
- Try re-flashing the firmware

## Stabilizer Rattle

Stabilizers can rattle if they're not properly lubed or seated:

1. Remove the keycap
2. Pull out the stabilizer
3. Apply a thin layer of dielectric grease to the wire ends
4. Re-clip and test

## USB Not Recognized

- Try a different cable
- Try a different USB port
- Check that the USB-C connector is fully seated on the PCB
- Try putting the board in bootloader mode (hold reset while plugging in)

## Keys Registering Wrong Characters

Your keymap might not match your OS layout:

- Check your OS keyboard language settings
- Re-flash the default firmware
- If using VIA, make sure you're editing the right layer

## Need More Help?

Jump into the [Hack Club Slack](https://hackclub.com/slack) and ask in the `#keeb` channel. Someone will help you out.
