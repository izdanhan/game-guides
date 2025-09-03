# Unlocking FPS in Skyrim Special Edition (SSE)

Skyrim Special Edition is capped at 60 FPS by default. You can unlock it using the following steps.

---

## 1. Edit `SkyrimPrefs.ini`

1. Navigate to:  
   `Documents\My Games\Skyrim Special Edition\`
2. Open `SkyrimPrefs.ini` with a text editor.
3. Find the line under `[Display]`:

iPresentInterval=1


4. Change it to:

iPresentInterval=0


> This disables V-Sync and allows the game to go above 60 FPS.

---

## 2. Edit `Skyrim.ini` for Physics Fix

1. Open `Skyrim.ini` in the same folder.
2. Under `[General]`, add or edit:

bLockFrameRate=0


3. Under `[Papyrus]`, add or edit for more stability:

fUpdateBudgetMS=10.0
fExtraTaskletBudgetMS=5.0


> These tweaks help reduce physics glitches and script-related crashes at higher FPS.

---

## 3. Disable V-Sync in GPU Settings

Even with `iPresentInterval=0`, your GPU may still cap FPS.

- **NVIDIA:**  
  `NVIDIA Control Panel → Manage 3D Settings → Program Settings → Skyrim Special Edition → Vertical Sync → Off`
- **AMD:**  
  `Radeon Settings → Graphics → Wait for Vertical Refresh → Off`

---

## 4. Optional: Use a Mod for Stability

For the most stable high-FPS experience, use a mod like:

- **[Skyrim Special Edition FPS Unlock](https://www.nexusmods.com/skyrimspecialedition/mods/1187)**

> This patch fixes engine limitations and improves physics at higher FPS.

---

## ⚠️ Warnings

- Unlocking FPS above 60 may break:
  - Ragdoll physics
  - Projectile speeds
  - Animations and combat timing
- Very high FPS (144+) can cause crashes.
- Always back up your `.ini` files before editing.

---

**Tip:** If you want stable FPS above 120+, combine the `.ini` tweaks with the FPS Unlock mod.


