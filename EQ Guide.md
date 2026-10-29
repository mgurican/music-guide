# 🎚️ Master EQ Guide: Mesa Mark VII & Boss EQ-200

Return to [[Home]] | [[Amplifiers & Cabinets]] | [[Hardware & Routing]] | [[Tone Presets]]

---

## 1. Guitar & Pickup Frequency Profiling

Before moving a single EQ slider, understand the acoustic and magnetic baseline of each guitar's pickups so your EQ curves work *with* the instrument rather than fighting it:

* **Music Man Majesty 6 (DiMarzio Rainmaker / Dreamcatcher):**
  * Naturally mid-forward, vocal, and balanced across the spectrum with sweet, rounded highs.
  * *EQ Strategy:* Requires almost zero corrective pre-amp filtering. Focus on post-preamp (Channel B / Mark VII 5-Band) sculpting—carving `750Hz` for rhythm tightness or boosting `1.6kHz – 3.2kHz` for liquid Petrucci solo cut.
* **Epiphone Matt Heafy 7-String (Fishman Fluence Custom MKH):**
  * **Voice 1 (Modern Active):** Enormous sub-bass energy on the low-B string (`61.7Hz` fundamental) and an aggressive upper-mid spike. **Pre-amp high-pass filtering (`30Hz` & `60Hz` cut on EQ-200 Channel A) is mandatory** to stop low-B palm mutes from overwhelming the amplifier's V1 input stage.
  * **Voice 2 (Passive / Organic):** Warmer, broader midrange bark with looser vintage low-end bloom. Benefits from a gentle `120Hz` pre-cut and a `+2dB` upper-mid nudge at `800Hz – 1.6kHz` when playing classic British metal.
  * **Voice 3 (Single-Coil Split):** Experiences a natural ~6–8dB volume/gain drop compared to Voice 1/2. Compensate by boosting **EQ-200 Channel A `LEVEL` by `+4dB to +6dB`** (or engaging the [[Hardware & Routing#1. Front-of-Amp Pedals (Input Chain) & Drive Gain Staging|TC Spark Mini]]) and shaving `-2dB` at `6.4kHz` if the bridge split sounds too glassy under gain.
* **Schecter Reaper-6 FR (DiMarzio Crunch Lab / LiquiFire):**
  * **Crunch Lab (Bridge):** Huge low-mid density (`200Hz – 400Hz`) designed to make Swamp Ash bodies sound massive. In **Drop D / Drop C#**, cut `120Hz – 200Hz` by `-2dB to -3dB` in Channel A (Pre-Amp) to eliminate boxiness before distortion.
  * **LiquiFire (Neck):** Thick, tubular midrange; boosting `1.6kHz` by `+2dB` in Channel A makes fast alternate picking and sweeping articulate like a bridge pickup while keeping neck-pickup warmth.

---

## 2. Boss EQ-200 Architecture, Internal Menu Setup & 4CM Routing

The **Boss EQ-200** features two independent 10-band studio graphic EQ engines (**Channel A** and **Channel B**) running at 32-bit AD/DA and 96kHz internal sampling rate, with three selectable frequency centers (default Guitar mode: **`30Hz`, `60Hz`, `120Hz`, `200Hz`, `400Hz`, `800Hz`, `1.6kHz`, `3.2kHz`, `6.4kHz`, `12.8kHz`**).

### Series vs. Parallel vs. Independent Dual-Mono (4CM) Signal Flow

A common misconception in the Boss manual is the naming of the **`STRUCTURE`** parameter (`SERIES` vs. `PARALLEL`):
* **`STRUCT = SERIES`:** Routes `Input A -> Channel A -> Channel B -> Output A` internally on a single mono path. **Do NOT use `SERIES` when wired via the 4-Cable Method**, or Channel A and Channel B will bleed together in front of your amp!
* **`STRUCT = PARALLEL` (`PARA`):** When cables are plugged into **all four jacks** (`INPUT A`, `OUTPUT A`, `INPUT B`, `OUTPUT B`), setting `STRUCT = PARALLEL` completely separates the two EQ engines into **two 100% isolated, independent mono signal paths**:
  * **Channel A (`INPUT A -> OUTPUT A`):** Lives **in front of the amplifier** (Pre-Distortion Pickup Shaper & Sub-Bass Tightener).
  * **Channel B (`INPUT B -> OUTPUT B`):** Lives **inside the amplifier's FX Loop** (Post-Distortion Studio Console EQ & Solo Volume Boost).

```
[GUITAR] ──> [WAH] ──> [IN A] Boss EQ-200 Channel A (Pre-Amp) [OUT A] ──> [COMP / DRIVES / SPARK] ──> [AMPLIFIER INPUT]
                                                                                                         │ (Tube Preamp Gain)
[AMPLIFIER FX SEND] ──> [IN B] Boss EQ-200 Channel B (FX Loop) [OUT B] ──> [MODULATION / DELAY] ──> [AMP FX RETURN]
```

### Mandatory Boss EQ-200 Internal System Menu Setup
Press **[MEMORY] + [PANEL]** simultaneously to open the **MENU**, use the **[MEMORY]** knob to scroll, and configure these exact parameters:

| Menu Parameter | Required Setting | Engineering Reason |
| :--- | :--- | :--- |
| **`STRUCT` (Structure)** | **`PARA` (Parallel)** | Splits `IN A -> OUT A` and `IN B -> OUT B` into two isolated mono paths for 4-Cable Method routing. |
| **`LINK` (Channel Link)** | **`OFF`** | Allows Channel A (Pre-Amp) and Channel B (FX Loop) to have completely independent slider curves and bypass states. |
| **`RANGE`** | **`±15dB`** | Provides full ±15dB surgical cut/boost range (can be set to `±6dB` if you prefer finer, subtler resolution). |
| **`MEM EXT` (Memory Extent)** | **`1 – 4`** *(or `1 – 8`)* | **Crucial Live Workaround:** By default, the `MEMORY` footswitch cycles through all 127 presets before wrapping back to Preset 1! Setting `MEM EXT Max = 4` makes the `MEMORY` switch loop cleanly `1 -> 2 -> 3 -> 4 -> 1`. |
| **`M.SW` (Memory Switch)** | **`MEMORY`** *(or `B ON/OFF`)* | Controls what the right onboard footswitch does (steps through presets `1–4`, or toggles Channel B directly). |
| **`C1 FNC` (External CTL 1)** | **`A ON/OFF`** *(or `MEM INC`)* | Assigns external footswitch button 1 (Tip) to toggle Channel A (Pre-Amp EQ) or step preset UP. |
| **`C2 FNC` (External CTL 2)** | **`B ON/OFF`** *(or `MEM DEC`)* | Assigns external footswitch button 2 (Ring) to toggle Channel B (FX Loop Solo Boost) or step preset DOWN. |

### How to Read Both Channels on the Single OLED Screen ("Slider Catch" Method)
Because the EQ-200 has **one set of physical sliders** that edits **two virtual channels (A & B)** across **128 presets**, the physical plastic sliders will rarely match the stored curve of the inactive channel:
1. **The OLED Graphic Display Always Shows the Truth:** When you press the **`[CH A/B]`** button to switch the active view between Channel A and Channel B, the **OLED screen graphic immediately updates** to display the exact stored EQ curve of the selected channel.
2. **Physical Slider Catch / Pickup:** Moving a physical slider immediately overwrites that band's stored value for whichever channel LED (`A` or `B`) is currently lit. To check a stored value without accidentally changing it, simply read the bar graph on the OLED screen!
3. **Locking Your Sliders (`PANEL LOCK`):** Hold the **`[CH A/B]`** button for 2 seconds until `LOCKED` appears on the screen. This prevents accidental foot bumps from moving the physical sliders after you save a preset (write a preset by holding `[MEMORY] + [PANEL]`, selecting the slot number, and holding `[MEMORY] + [PANEL]` again to confirm `WRITING...`).

---

## 3. Boss EQ-200 Channel A & Channel B Master Curves

### Channel A: Pre-Amp Conditioning (In Front of the Amplifier)
* **Objective:** Re-voice pickups, cut sub-bass mud before tube clipping, or create special lo-fi filter effects.

| Curve Name | `30Hz` | `60Hz` | `120Hz` | `200Hz` | `400Hz` | `800Hz` | `1.6k` | `3.2k` | `6.4k` | `12.8k` | `LEVEL` | Target Guitar & Use Case |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| **1. 7-String Sub-Bass Tightener** | `-12dB` | `-8dB` | `-2dB` | `0dB` | `0dB` | `+3dB` | `+2dB` | `0dB` | `-2dB` | `-4dB` | `0dB` | **Heafy 7 (Voice 1 Active):** Eliminates low-B flub and pushes `800Hz` into the amp like a precision Tube Screamer. |
| **2. Drop C# / Drop D De-Mud** | `-8dB` | `-4dB` | `-3dB` | `-2dB` | `0dB` | `+2dB` | `+2dB` | `+1dB` | `0dB` | `-2dB` | `0dB` | **Schecter Reaper (Crunch Lab):** Removes boxy 120–200Hz build-up in Drop C# (*"One Step Closer"*) and Drop D (*"Schism"*). |
| **3. Coil-Split Gain Compensator** | `0dB` | `+2dB` | `+2dB` | `+1dB` | `0dB` | `0dB` | `0dB` | `-1dB` | `-2dB` | `0dB` | **`+5dB`** | **Heafy 7 (Voice 3 Split) / Majesty Split:** Restores fullness and matches volume/gain to humbucker channels (Deep Purple). |
| **4. Jack White "AM Radio" Lo-Fi Filter** | `-15dB` | `-15dB` | `-10dB` | `-5dB` | `+5dB` | **`+10dB`** | `+5dB` | `0dB` | `-10dB` | `-15dB` | `0dB` | **Any Guitar:** Band-pass telephone filter for the intro/breakdown of Jack White's *"You'll Never Fix Me"* (*Frozen Charlotte*). |

### Channel B: FX Loop Console Sculpting & Solo Boost (Post-Preamp)
* **Objective:** Shape the fully distorted preamp signal with studio console precision, or kick in a `+3.5dB` vocal solo boost.

| Curve Name | `30Hz` | `60Hz` | `120Hz` | `200Hz` | `400Hz` | `800Hz` | `1.6k` | `3.2k` | `6.4k` | `12.8k` | `LEVEL` | Target Amp & Use Case |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| **1. Liquid Solo Boost (Petrucci / Satch)** | `-3dB` | `0dB` | `+1dB` | `+2dB` | `+2dB` | `+3dB` | **`+4dB`** | `+2dB` | `-1dB` | `-3dB` | **`+3.5dB`** | **Mark VII or JVM 410C:** Pushes single notes forward in the mix with thick, singing midrange and zero top-end ear fatigue. |
| **2. JVM British NWOBHM Push (Maiden/Priest)** | `-4dB` | `+2dB` | `+3dB` | `+1dB` | `-2dB` | `+3dB` | `+3dB` | `+2dB` | `0dB` | `-4dB` | `+1dB` | **Marshall JVM (OD1):** Adds 4x12 cabinet thump at `120Hz`, clears `400Hz` boxiness, and accentuates twin-lead `800Hz–1.6kHz` bite. |
| **3. JVM Modern Prog / Tool Tightener** | `-6dB` | `+3dB` | `+4dB` | `0dB` | `-4dB` | `-2dB` | `+3dB` | `+3dB` | `+1dB` | `-6dB` | `0dB` | **Marshall JVM (Crunch Red / OD2):** Gives the EL34 Marshall a Mesa/Diezel-style post-gain low-end punch (`60–120Hz`) and mid carve. |
| **4. Ultra-Glossy Studio Clean (90s Rack)** | `-2dB` | `+2dB` | `+2dB` | `-2dB` | `-3dB` | `0dB` | `+1dB` | `+3dB` | `+4dB` | `+3dB` | `+1dB` | **Mark VII Ch 1 / JVM Clean:** Scoops `200–400Hz` mud and adds hi-fi `6.4kHz–12.8kHz` air for *"Pull Me Under"* / *"Endless Sacrifice"*. |

---

## 4. Marshall JVM 410C FX Loop Gain-Staging & Phase Rules

When running **Boss EQ-200 Channel B** inside the **Marshall JVM 410C** effects loop, follow these three electrical rules to prevent digital clipping and phase cancellation:

1. **Set the JVM Parallel/Series Loop `MIX` Knob to `100% WET`:**
   * Because the Boss EQ-200 converts analog audio to 32-bit/96kHz digital and back (`~1.2ms` latency), leaving the JVM's loop `MIX` knob at 50% blends dry analog signal with delayed digital signal. This causes **comb-filtering** (making your tone sound thin, hollow, and out-of-phase like a stuck flanger). Turning the rear **`MIX` knob all the way clockwise to `100% WET`** converts the loop into a pure **100% Serial Loop**.
2. **Set the JVM Loop Level Switch to `-10dBV` (Instrument Level):**
   * The Boss EQ-200 has a maximum nominal input headroom of **+7dBu**. In `-10dBV` mode, the JVM steps down the hot preamp output before sending it to the pedal, and steps it back up at the Return jack.
3. **Keep JVM Front-Panel `CHANNEL VOLUME` Knobs Between `9:00 and 11:00` (`3.0 – 4.5`):**
   * On the JVM 410C, the individual **Channel `VOLUME` knobs sit *before* the FX Loop Send**, while **`MASTER 1` and `MASTER 2` sit *after* the FX Loop Return**.
   * If you crank a JVM Channel `VOLUME` knob to `8–10`, you will overdrive the Boss EQ-200's input ADC into ugly digital crackle—even if your Master Volume is at `1`! Keep Channel Volumes moderate (`9:00 – 11:00`) and use **`MASTER 1 / MASTER 2`** to control room volume.

---

## 5. External Footswitch Comparison & Setup (`CTL 1, 2 / EXP`)

Connecting an external dual footswitch to the EQ-200's **`CTL 1, 2 / EXP`** jack via a **1/4" TRS (Stereo) cable** unlocks hands-free control over both EQ channels or preset up/down stepping:

| Footswitch Model | Power Required | Polarity / Mode Switches | Footprint & Ergonomics | Verdict |
| :--- | :--- | :--- | :--- | :--- |
| **Boss FS-7** (Dual Footswitch) | None (Passive works for switching; 9V only needed for LED indicators, which only light in Latching mode) | Rear **`MODE` (`MOMENTARY`)** & **`POLARITY` (`I`)** switches | **Ultra-compact vertical tandem footprint** (`62 x 131 mm`); saves half the pedalboard width of an FS-6 | **Best Choice.** Fits tightly right next to the EQ-200. |
| **Boss FS-6** (Dual Footswitch) | 9V Battery (if using Latching LEDs; drains battery whenever TRS cable is left plugged in!) | Rear Momentary/Latching & Polarity switches per pedal | Wide horizontal side-by-side enclosure (`188 x 91 mm`) | Good if you prefer wide switch spacing, but wastes board space and eats 9V batteries. |
| **2x Boss FS-5U** (Unlatched Single) | **Zero Power Required** (100% passive mechanical momentary) | Rear Polarity switch | Interlocks side-by-side; requires a **1/4" TRS-to-Dual-TS Insert ("Y") cable** | Bulletproof passive reliability with zero battery drain. |

> **Important Setup Rule:** The Boss EQ-200 requires **Momentary (Unlatched, Normally-Open)** switches. Set your FS-6 or FS-7 rear switch to **`MOMENTARY`**!

---

## 6. Mesa/Boogie Mark VII 5-Band Graphic EQ

The Mark VII's onboard analog inductor-based 5-Band Graphic EQ (`80Hz`, `240Hz`, `750Hz`, `2200Hz`, `6600Hz`) sits **post-preamp** and is the defining tonal engine of every Mark-series amplifier.

```
Frequencies:  [ 80Hz ]   [ 240Hz ]   [ 750Hz ]   [ 2200Hz ]   [ 6600Hz ]
Top Line (+12dB) ───────────────────────────────────────────────────────
Center (0dB)     ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─
Bottom (-12dB)   ───────────────────────────────────────────────────────
```

### Master 5-Band Graphic EQ Reference Curves

| Curve Name | `80Hz` | `240Hz` | `750Hz` | `2200Hz` | `6600Hz` | Target Artist / Tone Application |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **1. Classic Petrucci "V" (Modern Rhythm)** | **`+70%`** *(Just below top line)* | **`+15%`** *(Slightly above center)* | **`-75%`** *(Just above bottom line)* | **`+55%`** *(Halfway up)* | **`+35%`** *(1/3 above center)* | **Dream Theater (*Images & Words*, *Train of Thought*), Linkin Park, Trivium:** Massive sub-thump with surgical midrange scoop. |
| **2. 1986 *Master of Puppets* Extreme Scoop** | **`+85%`** *(Touching top line)* | **`0%`** *(On center line)* | **`-95%`** *(Bottomed out)* | **`+50%`** *(Halfway up)* | **`+45%`** *(Halfway up)* | **Metallica (*Master of Puppets* / *...And Justice for All*):** Hollow, percussive, hyper-scooped 80s thrash crunch (Ch 3 Mark IIC+ unboosted). |
| **3. Singing Lead "Mid-Balanced W"** | **`+35%`** | **`+25%`** | **`-15% to 0%`** *(Near center!)* | **`+40%`** | **`+10%`** | **Petrucci & Satriani Leads:** Raising `750Hz` back near the center line restores thick, liquid, vocal sustain and prevents thin high-fret notes. |
| **4. Adam Jones (Tool) "Flat-Mid Growl"** | **`+60%`** | **`+20%`** | **`-10%`** *(Barely dipped)* | **`+45%`** | **`+15%`** | **Tool (*"Schism"*, *"Jambi"* — Ch 2 Crunch / Ch 3 Mark VII):** Retains the dry, chesty, barking Diezel/Marshall midrange authority. |
