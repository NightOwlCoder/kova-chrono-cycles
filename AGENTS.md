# Chrono-Cycles - Agent Context

## Overview

**CHRONO-CYCLES** - Physics-Based Incremental / Idle Game  
**Platform:** Web (HTML5/JavaScript)  
**File:** Single HTML file (~90KB) - intentional design by tututi!

**Original Creator:** @tututi (10-year-old, built with Gemini AI)  
**Enhanced By:** Kova (bug fixes, polish, portfolio integration)

---

## The Core Loop

Players manage a "Chrono Engine" with 10 concentric spinning rings:

1. **Active Play** - Click rings to apply torque and increase RPM
2. **Economy** - Each rotation generates layer-specific resources (Time Shards, Genetic Code, etc.)
3. **Upgrades** - Three pillars per layer:
   - **Perpetual Motor** - Maintains minimum RPM
   - **Kinetic Lubricant** - Increases speed multiplier
   - **Matter Compression** - Boosts yield per lap
4. **Synergy** - Inner layers boost outer layers (balanced upgrade strategy)

---

## Dimension Tiers

### Standard Dimension (Current)
The 10-ring core engine with prestige system (Chronons).

### Infinity Dimension
- Unlocked at 3,000 RPM on all 10 layers
- Features center Black Hole
- Collect "Infinity Essence" via void particles

### Reality Dimension (Coming Soon)
Ultimate endgame area - teaser phase.

---

## Known Issues

### Power Creep Bug
High Chronon counts + Layer Synergy creates exponential runaway effect. Players can "solve" all 10 layers in under 10 seconds after prestige.

**Temporary Fix:** Removed inner ring synergy boost.

---

## Roadmap (Peak Concepts)

- **Universe Multiplier** - 10 perfected layers shrink into a "Nucleus", new larger rings spawn around it
- **Light Speed Barrier** - At 1M RPM, rings become solid beams of light (Relativistic tier)
- **Quantum Threads** - Draw lines to link rings across Parallel Universes
- **Infinity Forge** - Permanent progression shop, items persist through Big Bang resets
- **The Big Bang** - Hard Prestige that resets all tiers for Reality Shards

---

## Technical Details

| Component | Implementation |
|-----------|---------------|
| Structure | Single HTML file with inline CSS/JS |
| Canvas | Spinning colored rings per layer |
| Audio | Web Audio API synthesized sounds |
| Save | localStorage, auto-save every 30s |
| Animation | requestAnimationFrame game loop |

---

## Branding

- **Footer:** `💜 Enhanced by Kova · Original by @tututi`
- **Colors:** Purple/pink/cyan theme (Kova brand)
- **First 4 layers:** Purple (#bf5af2), Cyan (#64ffda), Dark Purple (#9b4dca), Pink (#ff6b9d)

---

## Features

- ✅ Click rings to add velocity
- ✅ RPM generates resources
- ✅ Buy upgrades with resources
- ✅ Prestige system (Chronons) for global bonuses
- ✅ Dimension shift to Infinity mode
- ✅ Random events (Solar Flare, Time Warp, etc.)
- ✅ Achievements
- ✅ Dev console (press ~ key)
- ✅ Per-layer auto-buy toggles
- ✅ [AUTO] badge on layer headers
- ✅ NEW GAME button in Settings
