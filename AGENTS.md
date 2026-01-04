# Chrono-Cycles Game - Agent Context

## Project Overview

Game Overview: CHRONO-CYCLES
Genre: Physics-Based Incremental / Idle ManagementPlatform: Web (HTML5/JavaScript)

1. The Core Loop
The player manages a "Chrono Engine" consisting of 10 concentric spinning rings.

Active Play: Clicking rings applies torque to increase RPM.
Economy: Each completed rotation (lap) generates resources unique to that layer (Time Shards, Genetic Code, etc.).
Upgrades: Players spend resources on three pillars: Auto-Motors (Minimum RPM), Kinetic Lubricants (Speed/Friction), and Matter Compression (Yield per lap).
Synergy: Progressing in inner layers provides a velocity boost to outer layers, encouraging a balanced upgrade strategy.
2. Dimension Tiers & Prestige
The game is structured into three distinct "Reality Tiers":

Standard Dimension: The 10-ring core engine.
Infinity Dimension: Unlocked at 3,000 RPM. Features a center Black Hole where players collect "Infinity Essence" via void particles.
Reality Dimension: The ultimate endgame area (Teaser phase).
3. Current Technical Challenge: The "Power Creep" Bug
During playtesting, we identified a scaling issue where the Prestige Currency (Chronons) and Layer Synergy create an exponential runaway effect.

The Issue: A player with high Chronon counts can prestige and "solve" all 10 layers in under 10 seconds. This removes the gameplay challenge and makes progression feel hollow.
The Fix: We are removing the boost the smaller rings give the outer temperaraly.
4. Future Roadmap (The "Peak" Concepts)
We have selected several high-concept mechanics to build out the endgame:

The Universe Multiplier: Once the first 10 layers are "perfected," the entire setup shrinks into a tiny "Nucleus," and the player begins building a second, much larger set of rings around it.
The Light Speed Barrier: At 1M RPM, rings transition from physical objects into solid beams of light, unlocking a new tier of "Relativistic" physics.
Quantum Threads: An active mechanic where players physically draw lines with the mouse to link rings across Parallel Universes to share multipliers.
Infinity Forge: A permanent progression shop where players spend late-game resources to forge items that persist through "Big Bang" hard resets.
The Big Bang: A final "Hard Prestige" that detonates the singularity, resetting all tiers in exchange for Reality Shards (God-tier currency).
Notes for the Developer (Dad):
The physics logic needs to handle extremely high numbers (scaling toward 1e100 and beyond) while maintaining a high frame rate. The current priority is decoupling the linear synergy boost  to fix the 10-second completion bug.


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
