# 🛠 1. Configuring the Script

At the very top of the .lua file, you’ll find a block of editable settings. These control how the script behaves:

PresetName → Select a weapon preset (ALL CAPS) or "CUSTOM".

Custom_VxPerTick, Custom_VyPerTick → Only used if PresetName = "CUSTOM".

SpeedScale → Multiplies both axes (keep angle, scale strength).

HumanizeLevel → 0 = perfect beam, 10 = no compensation.

AverageCompAt5 → Adjust how strong “average” recoil control feels.

RequireToggle + ToggleKey → Optional safety gate (CapsLock / NumLock / ScrollLock).

# 🎮 2. Using the Script In-Game

Hold Right Mouse Button (ADS) → script becomes active.

Hold Left Mouse Button (fire) → recoil compensation applies.

If RequireToggle = true, you must enable the chosen lock key (Caps/Num/Scroll).

# 🔧 3. Adding New Presets

To add a new gun/operator recoil profile:

Find the local Presets = { ... } table.

Add a new line like:

MYGUN = { vx = 0.25, vy = 4.10 },


Save the file and set PresetName = "MYGUN".

🚨 Notes

Script values must be tuned for your specific dpi and sensitivity. You cannot use the values originally in the table if you don't have the same settings they were made for. 

If you use different sensitivity/DPI, values may need manual adjustment.

Works only while G HUB is running and bound to your mouse profile.****

You can change the names of presets, you can also add or remove as many as you like as long as you dont change anything else in the code. 
