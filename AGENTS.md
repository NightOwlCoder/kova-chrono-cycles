# Chrono-Cycles - Agent Context

## Overview

**CHRONO-CYCLES** - Physics-Based Incremental / Idle Game  
**Platform:** Web (HTML5/JavaScript)  
**File:** Single HTML file (~90KB) - intentional design by tututi!  
**Current Version:** v8.3 (Reality Patch - Stable)

**Original Creator:** @tututi (21-year-old, built with Gemini AI)  
**Enhanced By:** Kova (bug fixes, polish, portfolio integration)

---

## The Core Loop

Players manage a "Chrono Engine" with 10 concentric spinning rings:

1.  **Active Play** - Click rings to apply torque and increase RPM.
2.  **Economy** - Each rotation generates layer-specific resources (Time Shards, Genetic Code, etc.).
3.  **Upgrades** - Three pillars per layer:
    - **Perpetual Motor** - Maintains minimum RPM.
    - **Kinetic Lubricant** - Increases speed multiplier.
    - **Matter Compression** - Boosts yield per lap.
4.  **Synergy** - Inner layers boost outer layers (balanced upgrade strategy).

---

## Dimension Tiers

### Standard Dimension (Current)
The 10-ring core engine with prestige system (Chronons).
* **Update v8.0:** Rings reaching **1,000,000 RPM** break the "Light Speed Barrier" and turn into solid beams of light (Bloom effect).
* **Update v8.3:** Ticking sounds now fade out at max speed to prevent audio clutter.

### Infinity Dimension
* Unlocked at 3,000 RPM on all 10 layers.
* Features center Black Hole.
* Collect "Infinity Essence" via void particles.
* **New Feature (v8.2): Constellations** - Essence accumulation passively connects stars in the background, boosting generation.
* **New Feature (v8.0): The Infinity Forge** - Spend Essence to craft permanent Artifacts (e.g., *Time Prism*, *Dark Matter Anchor*) that persist through resets.

### Reality Dimension (Active)
* **Unlock:** 1 Trillion Essence or via Time Prism artifact.
* **The Mechanic:** When "REALITY" is clicked, the entire previous game (10 rings) shrinks into a tiny "Microcosm" in the center.
* **Physics:** Total Inner RPM is converted via Logarithmic math into **Reality Torque** to power the massive outer Reality Ring.
* **Economy:** Reality Shards are earned only when the Reality Ring completes a full rotation.
* **Upgrades:** *Temporal Threads* (Speed) and *Universal Scales* (Value).

---

## Known Issues

### Power Creep Bug
High Chronon counts + Layer Synergy creates exponential runaway effect. Players can "solve" all 10 layers in under 10 seconds after prestige.
* **Temporary Fix:** Removed inner ring synergy boost.
* **Balancing (v8.3):** Reality Mode acts as the new sink for this power.

### Audio/Save Glitches (Fixed v8.3)
* **Fix:** "Force Wipe" now nukes the entire domain storage and reloads to prevent corrupted saves.
* **Fix:** Max speed sound now plays once and fades to silence over 2 seconds.

---

## Roadmap (Peak Concepts)

* **Universe Multiplier** - [IMPLEMENTED v8.0] 10 perfected layers shrink into a "Nucleus", new larger rings spawn around it.
* **Light Speed Barrier** - [IMPLEMENTED v8.0] At 1M RPM, rings become solid beams of light.
* **Infinity Forge** - [IMPLEMENTED v8.0] Permanent progression shop, items persist through Big Bang resets.
* **Constellations** - [IMPLEMENTED v8.1] Draw lines to link stars based on Essence.
* **Singularity Manual** - [IMPLEMENTED v8.2] In-game documentation book.
* **Quantum Threads** - Draw lines to link rings across Parallel Universes (Future).
* **The Big Bang** - Hard Prestige that resets all tiers for Reality Shards (Future).

---

## Technical Details

| Component | Implementation |
| :--- | :--- |
| **Structure** | Single HTML file with inline CSS/JS |
| **Canvas** | Spinning colored rings per layer + Reality Ring |
| **Audio** | Web Audio API synthesized sounds (Oscillators) with Fade logic |
| **Save** | `localStorage`, auto-save every 30s. Includes "Nuclear Wipe". |
| **Animation** | `requestAnimationFrame` game loop |

---

## Branding

* **Footer:** `💜 Enhanced by Kova · Original by @tututi`
* **Colors:** Purple/pink/cyan theme (Kova brand).
* **First 4 layers:** Purple (#bf5af2), Cyan (#64ffda), Dark Purple (#9b4dca), Pink (#ff6b9d).
* **Reality:** Gold (#ffd700).

---

## Features

* ✅ Click rings to add velocity
* ✅ RPM generates resources
* ✅ Buy upgrades with resources
* ✅ Prestige system (Chronons) for global bonuses
* ✅ Dimension shift to Infinity mode
* ✅ Random events (Solar Flare, Time Warp, etc.)
* ✅ Achievements
* ✅ Dev console (press ~ key)
* ✅ **[UPDATED]** Per-layer auto-buy toggles (10 individual buttons in Shop)
* ✅ [AUTO] badge on layer headers
* ✅ NEW GAME button in Settings
* ✅ **[NEW]** Reality Mode (Zoom-out mechanic)
* ✅ **[NEW]** Infinity Forge (Artifact Crafting)
* ✅ **[NEW]** Visual Floater Toggles (Eye icon per layer)
* ✅ **[NEW]** Singularity Manual (In-game Guide)