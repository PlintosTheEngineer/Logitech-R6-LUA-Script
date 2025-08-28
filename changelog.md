# 📜 Changelog

## v1.0.0 — Initial Release (2025-08-28)
- 🚀 First public version of the Logitech LUA recoil control script.
- Added **preset system** with sample operator profiles (`BUCK`, `ZOFIA`, `R4C`, `SMG12`, `GOYO`, `SMG11`, `LESION`).
- Added **CUSTOM mode** for user-defined recoil (X/Y per tick).
- Implemented **HumanizeLevel (0–10)** slider:
  - 0 = “hacker beam” (perfect counter).
  - 10 = no compensation.
  - 5 = configurable “average” recoil control, tunable via `AverageCompAt5`.
- Added **global SpeedScale** multiplier for scaling both axes while keeping the angle.
- Implemented **optional toggle key gate** (`CapsLock`, `NumLock`, `ScrollLock`).
- Added **sub-pixel smoothing engine** (DDA accumulators) for consistent movements.
- Added **auto-reset** safety so movement stops immediately when firing/ADS ends.
- Grouped all **user-editable fields** at the top of the script for clarity.
