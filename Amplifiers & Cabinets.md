# 🔊 Amplifiers, Preamps & Cabinet Systems

Return to [[Home]] | [[Hardware & Routing]] | [[Silent Practice & Studio Audio]] | [[Tone Presets]]

---

## 1. Mesa/Boogie Mark VII (90W Tube Head/Combo)

The Mesa/Boogie Mark VII is the definitive modern American high-gain channel switcher, offering **9 distinct preamp voicings across 3 discrete channels**, a post-distortion 5-Band Graphic EQ, a Multi-Watt Simul-Class power section (**90W / 45W / 25W**), and an onboard **CabClone IR** system with a built-in reactive load.

### Channel & Mode Architecture

* **Channel 1 (Clean & Vintage Crunch Foundation):**
  * **Clean:** High-headroom, glassy, pristine American cleans with ultra-fast transient recovery.
  * **Fat:** Extended lower-mid warmth and harmonic thickness; ideal for single-coil splits (Heafy Voice 3 / Majesty middle split) and liquid clean jazz/prog arpeggios.
  * **Crunch:** Vintage British-flavoured edge-of-breakup to classic 70s rock drive; highly responsive to right-hand pick dynamics and guitar volume knob cleanup.
* **Channel 2 (Mid-Gain, Alt-Rock & Modern Rhythm):**
  * **Fat:** Duplicated from Channel 1 so you can dedicate Channel 1 to pristine cleans and Channel 2 to pushed edge-of-breakup cleans.
  * **Crunch:** Aggressive, mid-forward crunch with dense lower-mid bark. Bridges the gap between a hot-rodded Marshall JCM800 and a Mesa Mark—exceptional for **Tool (Adam Jones)**, **AC/DC**, and classic hard rock.
  * **Mark VII:** A modern, wide-bandwidth high-gain voicing unique to this amp. Tight, punchy, and slightly more open in the low-mids than Mark IIC+, ideal for modern hard rock (Shinedown) and 7-string rhythm.
* **Channel 3 (Legendary High-Gain Shred & Thrash):**
  * **Mark IIB:** Vintage, warm, singing lead tone with early cascading gain and thicker midrange sponge.
  * **Mark IIC+:** The legendary **John Petrucci (*Images & Words*)** and **Metallica (*Master of Puppets*)** rhythm/lead engine. Razor-sharp attack, focused upper-mids, surgical sub-bass tightness, and instant tracking.
  * **Mark IV:** Thicker, creamier saturation with enhanced low-mid density and liquid sustain (*Train of Thought*, *Black Album*, Joe Satriani-style singing leads).

### Dual-Stage EQ Philosophy (Pre vs. Post Distortion)

1. **Pre-Distortion Rotary Tone Stack (`GAIN`, `BASS`, `MID`, `TREBLE`):**
   * Located at the **very front of the preamp circuit** (Fender Blackface topology), *before* the cascading 12AX7 tube clipping stages.
   * **`TREBLE` is the Dominant Valve:** Signal flows through the Treble pot first; turning `TREBLE` up (**6.0 – 7.5** / 1:00–2:30) directly increases gain saturation, harmonic sizzle, and pick attack, while simultaneously reducing the effectiveness of the `BASS` and `MID` pots.
   * **The Golden High-Gain Rule — Keep `BASS` Low (`1.5 – 3.0` / 8:00–9:30):** Pushing `BASS` above 3.5 in Channel 3 floods the clipping tubes with low-end energy, causing "blocking distortion" (muddy, farty, indistinct palm mutes).
2. **Post-Distortion 5-Band Graphic EQ (`80Hz`, `240Hz`, `750Hz`, `2200Hz`, `6600Hz`):**
   * Located at the **end of the preamp** (after the distortion tubes), shaping the fully saturated waveform before the power section.
   * Because you starved the pre-distortion `BASS` knob for tightness, you restore massive chest-thumping low end by boosting the **`80Hz` slider** and carving out boxy mud with the **`750Hz` slider**. See [[EQ Guide#6. Mesa/Boogie Mark VII 5-Band Graphic EQ|EQ Guide]] for the exact slider curves.

### Simul-Class Power Section vs. Dual/Triple Rectifier Sag

* **Simul-Class Multi-Watt Design:**
  * **90W (Simul-Class):** Runs two inner power tubes in pentode Class A wired in parallel with two outer power tubes in pentode Class AB. Delivers massive headroom, zero low-end sag, and surgical tracking under high-speed alternate picking.
  * **45W (Class A/B Pentode):** Runs two tubes in traditional Class AB for tighter headroom and earlier power-tube compression.
  * **25W (Class A Triode):** Runs two tubes in Class A triode mode for spongy, sweet, harmonically rich lower-volume saturation.
* **Mark VII vs. Dual/Triple Rectifier Architecture:**
  * *Dual/Triple Rectifiers* place the rotary tone stack *after* the gain stages (derived from the Soldano SLO-100), often use 5U4G vacuum tube rectifiers, and minimize negative feedback in "Modern" mode—producing a slower, spongy attack and a massive, loose wall of sub-bass bloom (classic Linkin Park / Nu-Metal).
  * *Mark VII* uses solid-state diode rectification, pre-gain tone shaping, and tight negative feedback for clinical precision.
* **Slaving a Rectifier Preamp into the Mark VII:** Running an external Rectifier/Diezel preamp (e.g., Synergy SYN-1 with Dual Rectifier or Diezel VH4 module, or AMT R2) into the Mark VII's **FX Return** combines the massive, aggressive Recto/VH4 preamp roar with the ultra-tight Simul-Class 6L6 power section and post-loop Graphic EQ.

### Built-In Reactive Load, CabClone IR & Dry Line Out Engineering

* **Internal Reactive Load & Speaker Off Mode:**
  * Unlike vintage tube amps (and unlike earlier Mark V heads in full-power mode), the Mesa/Boogie Mark VII features a **built-in internal reactive load** wired into its output section.
  * Engaging the rear **`SPEAKER OFF`** switch (or unplugging the speaker cable from the speaker jacks) automatically routes the Simul-Class power amp's output into the internal dummy load for **100% silent direct recording or headphone practice**.
  * *Thermal Best Practice:* When running in **90W mode** for extended hours, the internal reactive load resistor dissipates substantial heat inside the chassis. Dropping the per-channel Multi-Watt switch to **25W or 45W** during silent headphone sessions—or leaving the combo speaker plugged in when using `LINE OUT`—keeps internal chassis temperatures significantly cooler.
* **`LINE OUT (Dry)` Tap Location (Post-Power Amp):**
  * Per the official Mesa/Boogie Mark VII manual, the 1/4" **`LINE OUT`** jack (controlled by the `LINE OUT LEVEL` knob) is an **uncompensated, raw duplication of the speaker output / internal reactive load signal**.
  * **Crucial Routing Implication:** Because the `LINE OUT` is tapped **post-power-amp** (after the Reverb, 5-Band Graphic EQ, Master Volume, Simul-Class 6L6 Power Section, and Output Transformer/Reactive Load), it **already contains full tube power-amp compression, transformer harmonics, and impedance interaction**.
  * Therefore, when routing `Mark VII LINE OUT -> Mooer Radar`, **Mooer Radar's internal Power Amp Simulation MUST be turned OFF** (otherwise you are double power-amping the signal, which smears transient clarity and adds artificial midrange bloat).
* **Onboard CabClone IR System & 8 Factory IR Slots:**
  * Each of the 3 channels has a dedicated **8-position rotary CabClone IR selector switch** on the rear panel. Both the **Balanced XLR Direct Out** and the **1/4" Stereo Headphone Out** are processed by whichever IR slot (`1`–`8`) is selected for the active channel.
  * Connects to PC/Mac as a **driverless USB Mass Storage Device (external flash drive)**—no proprietary Mesa software is required. Accepts **48kHz / 24-bit mono `.wav`** Impulse Responses.

| Slot # | Mesa Factory Pre-Loaded Cabinet IR | Recommended 3rd-Party Replacement (See [[Silent Practice & Studio Audio#5. Mesa/Boogie Mark VII CabClone IR USB Procedure|Silent Practice Guide]]) |
| :---: | :--- | :--- |
| **1** | 4x12 Recto Standard (Oversized Closed-Back, V30s — Dynamic Mic) | *Keep Stock* (Great baseline oversized Recto 4x12) |
| **2** | 4x12 Recto Traditional (Stiletto/Slant Closed-Back, V30s — Dynamic/Ribbon) | *Keep Stock* (Tighter traditional 4x12) |
| **3** | 2x12 Recto Horizontal (Closed-Back, V30s) | *Keep Stock* (Punchy, focused 2x12) |
| **4** | 1x12 Recto (Closed-Back, V30) | **Overwritten ->** `York Audio MES 412 OS-V2 Mix 01` *(57m + 121 — Liquid Lead / All-Rounder)* |
| **5** | 1x12 Boogie Thiele (Closed-Back Front-Ported, C90) | *Keep Stock* (Classic compact Mark-series C90 voice) |
| **6** | 2x12 Lone Star (Open-Back, C90s) | *Keep Stock* (Primary **Channel 1 Clean** IR — wide, airy open-back chime) |
| **7** | 1x12 Lone Star 23 (Open-Back, C90) | **Overwritten ->** `York Audio MES 412 OS-V2 Mix FRED` *(Dual Phased SM57s — Ch 2 Crunch / Tool Rhythm)* |
| **8** | 1x12 California Tweed 23 (Open-Back, Jensen Alnico) | **Overwritten ->** `York Audio MES 412 OS-V2 Mix JP` *(Petrucci Spec — Ch 3 Mark IIC+ / IV Rhythm)* |

---

## 2. Marshall JVM 410C (100W Tube Combo)

The Marshall JVM 410C is a 100-watt, 4-channel British tube flagship offering **12 distinct all-tube voicings** (3 modes per channel: **Green, Orange, Red**) driven by 5x ECC83/12AX7 preamp tubes and 4x EL34 power tubes into a 2x12 speaker configuration (Celestion Vintage 30 + Heritage G12H).

### Channel Voicing Matrix

| Channel | Green Mode | Orange Mode | Red Mode | Best Musical Application |
| :--- | :--- | :--- | :--- | :--- |
| **Clean** | Pure vintage preamp (Volume bypassed from post-gain path; Fender-like headroom) | Warm Plexi-style edge-of-breakup (Volume knob inserted in path) | Early JCM800-style dynamic crunch | Pristine cleans (Rush, Dream Theater), pedal platform, blues |
| **Crunch** | Classic 1959/1987 Plexi roar (shared cathode stage) | Hot-rodded JCM800 (2203) bite (adds gain stage) | High-gain JCM900 / modded 800 roar | Deep Purple, Led Zeppelin (*"Kashmir"*), AC/DC, 70s/80s hard rock |
| **OD1** | Classic British heavy metal rhythm | Searing NWOBHM lead & heavy rhythm | Maximum cascading British saturation | Iron Maiden, Judas Priest (*"Painkiller"*), Ozzy (*"Mama, I'm Coming Home"*), Satriani |
| **OD2** | OD1 architecture with **mid-peak shifted from ~650Hz down to ~500Hz** | Modern aggressive low-mid rhythm crunch | Ultra-saturated modern scooped metal lead | Drop tunings, Linkin Park / Tool alternatives, modern metal |

### Standby Switch "Silent Recording" Mode & Power Amp Sim Rule

* **How It Works:** Leaving the **MAINS** switch **ON** while keeping the **STANDBY** switch in the **OFF (Standby)** position disengages high-voltage B+ plate current from the 4x EL34 power tubes while keeping all low-voltage DC heaters, 12AX7 preamp tubes, MIDI switching, and FX loops 100% active.
* **Safe Silent Direct Practice:** You can safely practice or record silently from the **FX Loop Send** (or rear XLR Emulated Line Out) into your [[Silent Practice & Studio Audio|silent headphone chain]] **with zero speaker output and without requiring an external reactive load box**.
* **Crucial Mooer Radar Rule for JVM Standby Mode:** Because the EL34 power tubes are turned off in Standby mode, the signal leaving the JVM `FX Send` is **pure preamp signal**. When feeding `JVM FX Send -> Mooer Radar`, **Mooer Radar's Power Amp Simulation MUST be turned ON and set to `EL34` (Class AB)** (`Input Gain: 12:00`, `Presence: 1:00`, `Level: 12:00`) to restore British power-section sag and tame raw preamp fizz.

### Dual Effects Loop Architecture

1. **Loop 1 — Programmable Parallel / Series Loop:**
   * Footswitchable and MIDI-programmable per preset, featuring a rear **MIX knob (`Dry <-> Wet`)** and a **`+4dBu / -10dBV` level switch**.
   * **Digital Pedal Phase Warning:** When running digital pedals with AD/DA conversion latency (such as the [[EQ Guide#2. Boss EQ-200 Architecture, Internal Menu Setup & 4CM Routing|Boss EQ-200]] or [[Hardware & Routing#2. Effects Loop Pedals (Post-Preamp Chain)|TC Flashback Triple Delay]]) in this loop, you **MUST set the rear MIX knob to `100% WET`** (turning it into a true Series loop). Blending dry analog preamp signal with 1–2ms delayed digital signal creates severe hollow comb-filtering (phase cancellation).
2. **Loop 2 — Power Amp Insert / Serial Loop:**
   * Always-active pure serial loop located directly before the Master Volumes and power amp. Also serves as the **Preamp Out / Power Amp In** jack pair for 4-Cable Method routing or silent preamp tapping.

---

## 3. Marshall DSL5C Combo (Original 2012 Version)

A compact 5-watt all-tube British practice combo upgraded with a **10" Celestion G10 Greenback** speaker for woody midrange warmth and smoother top-end breakup than the stock Celestion Ten-30.

### Hardware Quirks, Power Tube Topology & Silent Recording

* **Differences Between Original 2012 DSL5C vs. Later DSL5CR:**
  * **Power Tube:** Uses a dual-triode **12BH7 / ECC99** configured in **push-pull** (providing genuine Class AB push-pull harmonic cancellation and tighter low-end punch than single-ended EL84 practice amps).
  * **Classic Gain Channel:** Features **only a `VOLUME` knob** (no separate Gain knob). It stays crystal clean at lower settings and transitions into natural British crunch only when cranked past 6–7 or pushed with a front-end boost ([[Hardware & Routing#1. Front-of-Amp Pedals (Input Chain) & Drive Gain Staging|Ibanez TS808 or TC Spark Mini]]).
  * **No Built-in Reverb & No Master Volume:** Relies on external pedals in the rear FX Loop for ambience, and channel volume knobs directly control overall output.
* **Safe Silent Recording Procedure (`0.5W Low Power Mode` Requirement):**
  * **5W Mode Has NO Internal Dummy Load:** Never unplug the internal Greenback speaker while the rear switch is set to **5W (High Power)**—doing so risks damaging the output transformer.
  * **0.5W Low Power Mode Internal Load:** Per Marshall's engineering spec for the original 2012 DSL5C, engaging the rear **Low Power (`0.5W`)** switch engages an internal attenuation load network. To record silently:
    1. Turn the amplifier **OFF**.
    2. Set the rear power switch to **`0.5W (Low Power)`**.
    3. Unplug the internal speaker cable from the rear `16Ω SPEAKER` jack (or connect the **`AUDIO OUT` / Emulated Headphone Out**), then power the amp on.
  * **Volume-Slaved Output Quirk:** Because the 2012 DSL5C lacks a separate Master Volume after the preamp, the rear `AUDIO OUT` signal level is directly governed by the front-panel Channel `VOLUME` knob (so turning Channel Volume to zero mutes the Line Out as well). For uncolored IR loading into the [[Silent Practice & Studio Audio#3. Mooer Radar Setup & Optimization|Mooer Radar]], tap the **FX Loop `SEND`** instead of the filtered `AUDIO OUT`, and turn Radar's **Power Amp Sim ON (`EL34` or `EL84`)**.

---

## 4. Standalone Preamps & Modular Upgrades

Integrating dedicated external preamps into the **FX Return (`Power Amp In`)** of the Mark VII or JVM 410C—or into the Mooer Radar for silent practice—unlocks entirely new amplifier architectures without buying bulky full-size heads:

1. **Synergy SYN-1 Tabletop/Pedalboard Preamp Dock + Diezel VH4 or Dual Rectifier Module:**
   * All-tube modular dock running two 12AX7 tubes that integrates seamlessly via 4-Cable Method (automatically bypassing your combo's preamp when engaged and routing the module straight into your amp's tube power section).
   * **Diezel VH4 Module:** Delivers the exact dry, ultra-compressed, percussive low-mid authority of **Adam Jones (Tool)** and modern progressive metal, pairing brilliantly with the Mark VII's Channel 3 or JVM's OD1 in a bi-amp/switching rig.
   * **Soldano SLO / Mesa Dual Rectifier Modules:** Adds classic loose Recto wall-of-sound rhythm or searing 80s/90s Soldano lead sustain.
2. **Victory V4 The Copper (All-Tube Vox AC30 Preamp Pedal):**
   * Runs 4 miniature NOS tubes (1x EC900, 3x CV4014) to recreate a true Class-A British **Vox AC30 Top Boost** circuit—the one major classic amp voice missing between a Fender/Mesa clean and a Marshall EL34 crunch.
   * Delivers jangly, chimey edge-of-breakup cleans and Brian May / Rory Gallagher / U2 harmonic roar when run via 4-Cable Method into the JVM or Mark VII.
3. **KSR Ceres (3-Channel Boutique Solid-State/FET High-Gain Preamp):**
   * Packs the exact circuit topology of KSR's flagship Orthos/Colossus heads into a compact pedal.
   * Features a selectable `Feel` switch (tight high-pass filter before clipping) and `Mode` switch that keeps 7-string **B-Standard and Drop-A** riffs surgical and articulate without needing a Tube Screamer in front.
4. **Effectrode Blackbird SR-71 (High-Voltage NOS Tube Clean/Overdrive Preamp):**
   * Class-A point-to-point tube preamp running three 12AX7/5751 tubes at true 300V plate voltage.
   * Channel 1 delivers ultra-3D Fender Blackface studio cleans; Channel 2 delivers cascading **Dumble Overdrive Special** liquid, blooming brass-like lead sustain (Eric Johnson / Robben Ford / Santana).
5. **Kingsley Harlot (250V 12AX7 Tube Overdrive / Preamp):**
   * Hand-wired, point-to-point tube overdrive/preamp running a real 12AX7 at ~250V plate voltage.
   * Excels into the Clean channel of the Mark VII or JVM for dynamic, touch-sensitive boutique tube breakup and harmonically rich plexi/boutique rhythm crunch.
6. **Two Notes Torpedo Captor X (Reactive Load Box, Tube Attenuator & Dual-IR Loader):**
   * Connects directly to the **Speaker Output** of the JVM 410C (8Ω or 16Ω) or Mark VII (8Ω), providing a studio-grade reactive load so you can crank the **real EL34 or Simul-Class 6L6 power tubes** silently or attenuate your combo speakers to bedroom volume (-20dB / -38dB).

---

## 5. Master Amplifier Comparison

| Feature | Mesa/Boogie Mark VII | Marshall JVM 410C | Marshall DSL5C (2012) |
| :--- | :--- | :--- | :--- |
| **Power Output & Tubes** | 90W / 45W / 25W Simul-Class (4x 6L6 or EL34) | 100W Class AB (4x EL34) | 5W / 0.5W Push-Pull (1x 12BH7/ECC99) |
| **Core Tonal Voice** | American surgical precision, tight sub-bass & liquid lead | British roaring EL34 crunch & vocal upper-mid bark | Vintage British bedroom crunch (10" Greenback) |
| **Gain & EQ Architecture** | Pre-gain tone stack + 9 modes + post-gain 5-Band Graphic EQ | 4 channels x 3 modes (12 voicings) + post-gain Marshall tone stack | Dual channel (Volume-only Classic Clean + Ultra Gain) |
| **Silent Direct Practice** | Built-in Reactive Load (`SPEAKER OFF`) + CabClone IR (48kHz USB) + Post-Power-Amp `LINE OUT` (Radar Power Sim **OFF**) | Standby "Silent Recording" mode via `FX Send` (safe without load; Radar Power Sim **ON - EL34**) | `0.5W` Low Power internal load + `FX Send` / `Audio Out` (speaker unplugged while OFF in 0.5W mode) |
| **MIDI Control** | Full PC & CC (Channels, EQ, Reverb, FX Loop) | PC-only (128 presets storing Channel/Mode, Master 1/2, Reverb, Loop) | None (Analog TRS Footswitch only) |
| **Best Musical Fit** | Dream Theater, Metallica, Tool, Linkin Park, modern shred | Iron Maiden, Judas Priest, Deep Purple, Ozzy, Led Zeppelin, Satriani | Low-volume tube breakup, classic rock bedroom jamming |
