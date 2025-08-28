# 🎯 Logitech-R6-LUA-Script

This project is a **Logitech G HUB Lua script** that provides customizable **recoil control** for Tom Clancy’s *Rainbow Six Siege*.  
The script is written in a **transparent and modular way**, so anyone can see exactly what values they are adjusting and how those changes affect recoil compensation.  

## 🔑 Features
- **Preset System:** Choose from built-in presets or create your own custom profile.  
- **Editable Settings Block:** All user-facing options (presets, multipliers, humanization, toggles) are grouped at the top for easy modification.  
- **Humanization Curve:** Adjustable `HumanizeLevel` (0–10) to simulate different skill levels, from “perfect beam” to natural recoil drift.  
- **Global Scaling:** Adjust overall recoil strength with `SpeedScale` without changing angles.  
- **Toggle Support:** Optional use of `CapsLock`, `NumLock`, or `ScrollLock` as a safety switch.  
- **Precision Engine:** Sub-pixel compensation and smoothing ensure consistent results.  

## 🎮 How It Works
1. Hold **Right Mouse Button** (ADS) to enable recoil control.  
2. Hold **Left Mouse Button** (fire) to apply recoil compensation.  
3. Script pulls the mouse smoothly according to the selected preset and humanization level.  

## ⚙️ Customization
- Add or rename presets in the `Presets` table.  
- Use `CUSTOM` mode with your own X/Y per-tick values.  
- Adjust `AverageCompAt5` to redefine what “average” recoil control feels like.  

## 🚧 Limitations in v1.0.0
- Presets cannot yet be cycled in-game (requires editing the script).  
- Single global tick rate (`DelayRateMS = 7`).  
- Humanization affects compensation amount, not recoil randomness.  
- Does not auto-scale with DPI or in-game sensitivity (values tuned for defaults).  

---
