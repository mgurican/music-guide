# 🎚️ Master EQ Guide (Mesa Mark VII & Boss EQ-200)

Return to [[Home]] | [[Hardware & Routing]] | [[Amplifiers & Cabinets]]

This guide breaks down EQ strategies utilizing your **Mesa/Boogie Mark VII** built-in 5-Band EQ alongside the **Boss EQ-200** (wired in a 4-cable method: Ch A Pre-Amp, Ch B FX Loop). These settings are tailored precisely for the unique frequency responses of your three primary guitars, taking into account their specific voicings.

---

## 🎸 1. Guitar & Pickup Profiling

Before adjusting EQ sliders, it is critical to understand the natural frequencies your pickups output:

* **Music Man Majesty 6 (2019 Kinetic Blue):** The 2019 Majesty shifted to DiMarzio Rainmaker (Neck) and Dreamcatcher (Bridge) pickups. These are heavily mid-focused, extremely thick, and very hot. They naturally push the amp hard, so extreme EQ correction is not needed—focus should be on subtle shaping and letting the natural midrange cut through.
* **Epiphone Matt Heafy 7 (Fishman Fluence):** 
  * **Modern Mode (Active/High Gain):** Extremely punchy, aggressive, and compressed. The low-B string throws a lot of energy. *Crucial:* High-pass filtering (cutting extreme lows) *before* the amplifier is mandatory here to prevent muddy, "farting" distortion.
  * **Vintage Mode (Passive/Organic):** More dynamic, warmer, and less compressed. The high-end is rounder. When using this mode, you might not need to cut the bass as aggressively, and can add slightly more presence/highs in the FX loop.
* **Schecter Reaper-6 (CrunchLab / LiquiFire):** Extremely thick midrange with tight tracking. Excellent for drop tunings, but the neck pickup can get overly "flutey" or the bridge can get "honky" if lower-mids aren't managed properly.

---

## 🎛️ 2. Boss EQ-200 Routing & Strategy

Your Boss EQ-200 is wired to process both Pre-Amp (Channel A) and FX Loop (Channel B), granting you dual-stage control:

### Channel A: Pre-Amp (Before the Amp)
* **Goal:** Condition the raw guitar signal *before* it hits the amplifier's distortion gain stages. This tightens up the tracking and removes input mud.
* **For 7-String (Heafy - Modern Mode):** 
  * Cut 30Hz and 60Hz heavily (prevents low-B frequency flub).
  * Apply a slight bump at 800Hz to push the preamp tubes harder for tighter attack.
* **For 7-String (Heafy - Vintage Mode):** 
  * Leave lows a bit flatter for warmth; bump 1.6kHz slightly for clarity.
* **For Drop Tunings (Schecter CrunchLab):**
  * Cut 120Hz slightly to remove low-mid boominess.
  * Boost 1.6kHz and 3.2kHz slightly to accentuate pick attack.

### Channel B: FX Loop (After the Preamp)
* **Goal:** Shape the final distorted tone. This acts similarly to a studio mixing console EQ.
* **Lead Boost (Majesty 2019):**
  * The Rainmaker/Dreamcatcher pickups already have huge mids. Instead of boosting 800Hz heavily, try boosting **1.6kHz and 3.2kHz** slightly to add "slice" and cut without making it too boxy.
  * Raise the overall level slider for a volume jump.
* **Rhythm Scoop / Polish (Heafy 7 / Schecter):**
  * Boost 120Hz and 200Hz for cabinet "chug" resonance.
  * Leave mids relatively flat (let the Mesa handle the main scoop).
  * Boost 6.4kHz for top-end sizzle.

---

## 🔊 3. Mesa/Boogie Mark VII 5-Band Graphic EQ

The Mark VII's legendary graphic EQ is placed *post-preamp* (similar to the FX Loop) and is iconic for carving out the "Classic V" shape. 
Frequencies: **80Hz | 240Hz | 750Hz | 2200Hz | 6600Hz**

### Setting 1: The "Classic V" (For Epiphone 7-String & Schecter)
Best utilized with Mark IV or Mark VII modes for tight, aggressive metal rhythm.
* **80Hz:** +60% (Boost for chest-thumping lows and cabinet resonance)
* **240Hz:** +10% to +15% (Slight boost for warmth; avoid pushing too high to keep the 7-string clear)
* **750Hz:** -80% (Deep scoop. Removes the nasal "honk" of the pickups and opens up the metal tone)
* **2200Hz:** +50% (Boost for aggressive bite, scrape, and articulation)
* **6600Hz:** +40% (Boost for presence and high-end air)

### Setting 2: The "Lead Mid-Push" (For Majesty 2019 Kinetic Blue)
Best utilized with Mark VII or Fat modes for soaring, liquid Petrucci-style lead lines.
* **80Hz:** +20% (Adds subtle body)
* **240Hz:** +30% (Thickens single-note lines)
* **750Hz:** 0% to +10% (Leave flat or push slightly for mid-range dominance; do not scoop)
* **2200Hz:** +20% (Clarity and pick definition without harshness)
* **6600Hz:** 0% to -10% (Keeps the extreme highs smooth and round, avoiding "ice-pick" tones)

---

## 🛠️ Summary Workflow

1. **Clean up the lows:** Use **Boss EQ-200 Channel A (Pre-amp)** to cut sub-bass on your Heafy 7-string (especially in Modern mode) and drop-tuned Schecter *before* the signal distorts.
2. **Shape the core:** Use the **Mesa Mark VII Graphic EQ** to carve out the main amp voice (V-scoop for metal rhythm, flat/mid-push for leads).
3. **Final Polish / Solo Boost:** Use **Boss EQ-200 Channel B (FX Loop)** as a footswitchable solo boost (pushing upper mids and level) to instantly jump out of the mix during solos.
