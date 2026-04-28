# Silakka54 — Wireless ZMK Config

> 54-key wireless split keyboard firmware with nice!view display support

[![Build ZMK firmware](https://github.com/Atsaev/zmk-config/actions/workflows/build.yml/badge.svg)](https://github.com/Atsaev/zmk-config/actions/workflows/build.yml)
![ZMK](https://img.shields.io/badge/ZMK-firmware-blue)
![nice!nano v2](https://img.shields.io/badge/controller-nice!nano%20v2-green)
![nice!view](https://img.shields.io/badge/display-nice!view-purple)

---

## What is the Silakka54?

The **Silakka54** is a wireless 54-key split keyboard based on the popular **Lily58** layout. It removes 4 keys from the original 58-key design (inner thumb cluster + encoder positions), resulting in a cleaner, more compact thumb cluster without sacrificing the columnar stagger feel.

This config uses the official **Lily58 shield** with the 4 missing positions mapped to `&none`.

**Hardware:**
- Controller: [nice!nano v2](https://nicekeyboards.com/nice-nano/) (Bluetooth + USB-C)
- Display: [nice!view](https://nicekeyboards.com/nice-view/) (ultra low-power sharp memory display)
- Firmware: [ZMK](https://zmk.dev)

---

## Keymap

### Base Layer

```
┌─────┬────┬────┬────┬────┬────┐                 ┌────┬────┬────┬────┬────┬───────┐
│ ESC │ 1  │ 2  │ 3  │ 4  │ 5  │                 │ 6  │ 7  │ 8  │ 9  │ 0  │   `   │
├─────┼────┼────┼────┼────┼────┤                 ├────┼────┼────┼────┼────┼───────┤
│CTRL │ Q  │ W  │ E  │ R  │ T  │                 │ Y  │ U  │ I  │ O  │ P  │   -   │
├─────┼────┼────┼────┼────┼────┤                 ├────┼────┼────┼────┼────┼───────┤
│RAISE│ A  │ S  │ D  │ F  │ G  │                 │ H  │ J  │ K  │ L  │ :  │   '   │
├─────┼────┼────┼────┼────┼────┼──────┐   ┌──────┼────┼────┼────┼────┼────┼───────┤
│LOWER│ Z  │ X  │ C  │ V  │ B  │  —  │   │  —  │ N  │ M  │ ,  │ .  │ /  │   \   │
└─────┴────┴────┼────┼────┼────┼──────┤   ├──────┼────┼────┼────┼────┴────┴───────┘
                │GUI │SHFT│SPC │  —  │   │  —  │ENT │TAB │DEL │
                └────┴────┴────┴──────┘   └──────┴────┴────┴────┘
```

### Lower Layer — Media & Function Keys
Hold the bottom-left key (`LOWER`).

```
┌─────┬─────┬─────┬─────┬──────────┬──────────┐               ┌─────┬────┬────┬─────┬─────┬─────┐
│     │     │     │     │          │          │               │     │    │    │     │     │     │
├─────┼─────┼─────┼─────┼──────────┼──────────┤               ├─────┼────┼────┼─────┼─────┼─────┤
│     │     │     │     │   PLAY   │  VOL UP  │               │     │ F4 │ F5 │ F6  │ F11 │ F12 │
├─────┼─────┼─────┼─────┼──────────┼──────────┤               ├─────┼────┼────┼─────┼─────┼─────┤
│     │     │     │     │   NEXT   │  VOL DN  │               │     │    │    │     │     │     │
├─────┼─────┼─────┼─────┼──────────┼──────────┼────┐     ┌────┼─────┼────┼────┼─────┼─────┼─────┤
│     │     │     │     │          │          │ — │     │ — │     │    │    │     │     │     │
└─────┴─────┴─────┼─────┼──────────┼──────────┼────┤     ├────┼─────┼────┼────┼─────┴─────┴─────┘
                  │     │          │          │ — │     │ — │     │    │    │
                  └─────┴──────────┴──────────┴────┘     └────┴─────┴────┴────┘
```

### Raise Layer — Numpad & Navigation
Hold the middle-left key (`RAISE`).

```
┌─────┬─────┬─────┬─────┬─────┬─────┐               ┌─────┬─────┬─────┬──────┬──────┬───────┐
│     │     │     │     │     │     │               │     │     │     │      │      │       │
├─────┼─────┼─────┼─────┼─────┼─────┤               ├─────┼─────┼─────┼──────┼──────┼───────┤
│     │     │     │     │     │     │               │  7  │  8  │  9  │      │      │       │
├─────┼─────┼─────┼─────┼─────┼─────┤               ├─────┼─────┼─────┼──────┼──────┼───────┤
│     │     │     │     │     │     │               │  4  │  5  │  6  │      │  ↑   │       │
├─────┼─────┼─────┼─────┼─────┼─────┼────┐     ┌────┼─────┼─────┼─────┼──────┼──────┼───────┤
│     │     │     │     │     │     │ — │     │ — │  1  │  2  │  3  │  ←   │  ↓   │   →   │
└─────┴─────┴─────┼─────┼─────┼─────┼────┤     ├────┼─────┼─────┼─────┼──────┴──────┴───────┘
                  │     │     │     │ — │     │ — │     │  0  │     │
                  └─────┴─────┴─────┴────┘     └────┴─────┴─────┴─────┘
```

---

## Combos

All combos are available on the Base layer.

| Keys | Output |
|------|--------|
| `R` + `T` | `=` |
| `E` + `R` | `+` |
| `S` + `D` | `[` |
| `A` + `S` | `{` |
| `F` + `G` | `]` |
| `J` + `K` | `}` |

---

## Building Firmware

### Via GitHub Actions (recommended)

1. Fork this repository
2. Edit `config/lily58.keymap` to your liking
3. Push your changes
4. Go to the **Actions** tab
5. Download `firmware.zip` from the latest successful run

### Building Locally

See the [ZMK documentation](https://zmk.dev/docs/development/setup) for local build setup.

---

## Flashing

### What you need
- USB-C cable
- The `.uf2` files from the firmware build:
  - `lily58_left-nice_nano_v2-zmk.uf2`
  - `lily58_right-nice_nano_v2-zmk.uf2`
  - `settings_reset-nice_nano_v2-zmk.uf2` (for pairing reset)

### Flash each half

1. Connect the half via USB-C
2. Enter bootloader: **double-tap** the reset button on the back of the board
3. It mounts as a USB drive named `NICENANO`
4. Copy the correct file:
   - Left half → `lily58_left-nice_nano_v2-zmk.uf2`
   - Right half → `lily58_right-nice_nano_v2-zmk.uf2`
5. The board restarts automatically
6. Repeat for the other half

---

## Pairing Reset

If the two halves lose sync or won't connect to each other:

1. Turn off both halves
2. For **each** half (start with the right):
   - Connect via USB-C
   - Double-tap reset → bootloader mode
   - Copy `settings_reset-nice_nano_v2-zmk.uf2` to `NICENANO`
   - Wait for restart
   - Double-tap reset again
   - Copy the correct firmware `.uf2`
3. Turn on both halves and simultaneously press reset on both to re-pair
4. Connect to the **left half** (master) via Bluetooth

---

## ZMK Studio

This firmware ships with **ZMK Studio** enabled — remap keys without reflashing:

1. Open [ZMK Studio](https://zmk.studio) in Chrome or Edge
2. Connect the keyboard via USB
3. Edit your keymap live — changes are applied instantly

> The 4 keys absent on the Silakka54 will appear in ZMK Studio but are non-functional.

---

## nice!view Display

The nice!view shows at a glance:
- Current active layer name
- Bluetooth connection status
- Battery percentage

Power consumption is negligible thanks to the display's ultra-low-power architecture and ZMK's dedicated display work queue (`CONFIG_ZMK_DISPLAY_WORK_QUEUE_DEDICATED`).

---

## Repository Structure

```
zmk-config/
├── config/
│   ├── lily58.keymap    # Keymap (54 keys, 4 as &none)
│   ├── lily58.conf      # Firmware settings (display, BT power, Studio...)
│   └── west.yml         # ZMK dependencies
├── build.yaml           # Build matrix
└── .github/
    └── workflows/
        └── build.yml    # GitHub Actions workflow
```

---

## Documentation

- [Keymap Editor Tutorial](keymap_editor_tutorial.md) — how to remap keys, add combos, behaviors and macros without editing code

---

## Contributing

Found a bug or have a keymap idea? Open an issue or a pull request — all contributions are welcome.

---

## License

MIT — do whatever you want with it.
