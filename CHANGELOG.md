# Changelog

## 2026-06-29

### Changed

- Reworked right-half trackball automouse handling to use ZMK input processors instead of the PMW3610 driver's direct `automouse-layer`.
- Added the `zmk-input-processor-deadzone` module, pinned at `7ae1bcb0d367ad00b7fa8836cf9a9b197d88e555`.
- Kept normal pointer speed at the original `1600 CPI / 4` setting.
- Added a `10` threshold / `150 ms` reset deadzone to suppress trackball micro-vibrations.
- Added a `250 ms` keyboard idle gate before trackball movement can activate the `BUTTON` mouse-click layer.
- Kept the mouse-button layer active for `400 ms` after qualifying trackball movement.

### Built

- Built `crosses_left-nice_nano_v2-zmk.uf2`.
- Built `crosses_right-nice_nano_v2-zmk.uf2`.
