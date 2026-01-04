# Chrono-Cycles Game - Agent Context

## Project Overview

**Chrono-Cycles** is an incremental/idle game with multiple resource layers, prestige mechanics, and dimension shifting.

**Original Creator:** @tututi (10-year-old, built with Gemini AI)  
**Enhanced By:** Kova (bug fixes, polish, portfolio integration)

**File:** Single HTML file (~90KB) - intentional design by tututi!

---

## Current Issues to Fix

### 1. Auto-Buy Indicator Missing
**Where:** Layer title rows (e.g., "ENTROPY GEAR (X1.0)")  
**Need:** Show `[AUTO]` badge right-aligned when auto-buy is active  
**Example:** `ENTROPY GEAR (X1.0)                    [AUTO]`

### 2. Wipe Save Button Broken
**Where:** Settings modal  
**Issue:** Doesn't clear localStorage  
**Fix:** `localStorage.clear(); location.reload();`

### 3. No Restart Game Button
**Where:** Settings modal  
**Need:** Add button to reload game without wiping save  
**Fix:** `<button onclick="location.reload()">🔄 Restart Game</button>`

### 4. Per-Layer Auto-Buy Toggles
**Current:** Global auto-buy only  
**Need:** Each layer should have its own auto-buy toggle  
**Where:** On the upgrade card itself or in settings

### 5. Kova Color Theme
Change first 4 layer colors:
```javascript
layers[0].color = "#bf5af2";  // Entropy - purple
layers[1].color = "#64ffda";  // Biomass - cyan
layers[2].color = "#9b4dca";  // Aether - dark purple
layers[3].color = "#ff6b9d";  // Plasma - pink
// Keep 4-9 as-is
```

---

## Game Mechanics (Don't Break!)

- Click spinning rings to add velocity
- RPM generates resources
- Buy upgrades with resources
- Prestige system (Chronons) for global bonuses
- Dimension shift to Infinity mode
- Random events (Solar Flare, Time Warp)
- Achievements
- Dev console

---

## Technical Details

**Structure:** Single HTML file with inline CSS/JS  
**Canvas:** Spinning colored rings for each layer  
**Audio:** Web Audio API synthesized sounds  
**Save:** localStorage with auto-save every 30s  
**Animation:** requestAnimationFrame game loop

---

## Branding

**Footer:** `💜 Enhanced by Kova | Original by @tututi`  
**Colors:** Purple/pink/cyan theme (Kova brand)  
**Keep:** Single file format (tututi's achievement!)

---

## Testing Checklist

- [ ] Auto-buy indicator shows on layer titles
- [ ] Wipe Save clears localStorage and reloads
- [ ] Restart Game button reloads page
- [ ] Per-layer auto-buy toggles work
- [ ] Kova colors applied to first 4 layers
- [ ] Canvas rings show new colors
- [ ] Game saves/loads correctly
- [ ] All original features still work
