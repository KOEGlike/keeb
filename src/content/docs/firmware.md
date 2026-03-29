---
title: Firmware
description: Flashing and customizing your keyboard firmware.
order: 4
---

Your PCB comes pre-flashed with a default keymap, but you can customize it to do whatever you want.

## Default Keymap

Out of the box, your keyboard uses a standard 60% ANSI layout. The `Fn` key (bottom right) activates a second layer with:

- `Fn + 1-0` → F1-F10
- `Fn + -/=` → F11/F12
- `Fn + Arrow keys` → Media controls
- `Fn + ESC` → Grave/tilde

## Customizing with VIA

The easiest way to remap your keyboard:

1. Go to [usevia.app](https://usevia.app) in Chrome
2. Plug in your keyboard
3. Click "Authorize device" when prompted
4. Drag and drop keys to reassign them
5. Changes are instant — no flashing required

## Customizing with QMK

For more advanced customization (macros, tap-dance, layers):

1. Clone the QMK firmware repo
2. Find the Keeb keymap directory
3. Edit `keymap.c` to your liking
4. Compile and flash:

```bash
qmk compile -kb keeb -km default
qmk flash -kb keeb -km default
```

## Resetting to Default

If something goes wrong, hold the reset button on the back of the PCB (or short the reset pins) while plugging in USB. This puts the board in bootloader mode so you can re-flash.
