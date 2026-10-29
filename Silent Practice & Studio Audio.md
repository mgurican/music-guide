# 🎧 Silent Practice, IR Cabinets & Studio Audio

Return to [[Home]] | [[Amplifiers & Cabinets]] | [[Hardware & Routing]] | [[Tone Presets]]

---

## 1. Studio-Grade Silent Headphone Signal Chain

Practicing through 90W–100W high-gain tube amplifiers with reference studio headphones requires an uncompromising analog/digital signal path. Standard headphone jacks built into guitar amplifiers or micro-pedals use inexpensive op-amps with high output impedance (`30Ω–100Ω`) and low voltage rails (`5V–9V`) that clip on palm-mute transients and smear stereo/room depth.

### The Reference Signal Path (Mesa Mark VII vs. Marshall JVM 410C)

```
[Guitar] ──> [Front Pedalboard: Dimebag Wah -> EQ-200 Ch A -> HyperGravity -> SD-1 -> TS808 -> Spark Mini]
   │
   ▼
[Amplifier Input & Tube Preamp / Power Section]
   ├── PATH A: Mesa/Boogie Mark VII (Set rear switch to "SPEAKER OFF" -> activates internal reactive load)
   │      └── Tap 1/4" "LINE OUT (Dry)" (Tapped POST-Power-Amp -> already has 6L6 Simul-Class power tube tone!)
   │
   └── PATH B: Marshall JVM 410C (Leave STANDBY switch in "OFF/Standby" -> Silent Recording Mode, no load needed)
          └── Tap 1/4" "FX SEND / Preamp Out" (Tapped PRE-Power-Amp -> EL34 power tubes are bypassed!)
   │
   ▼
[Amplifier FX Loop Pedals: EQ-200 Ch B -> TC Dreamscape -> TC Triple Delay (Mono Out)]
   │
   ▼
[Mooer Radar (24-Bit / 44.1kHz IR Cabinet Loader)]
   ├── Power Amp Sim for Mark VII (Path A): MUST BE **OFF** (Mark VII Line Out is already post-power-amp!)
   ├── Power Amp Sim for JVM 410C (Path B): MUST BE **ON -> EL34** (Restores bypassed Marshall power section!)
   ├── Cabinet IR: York Audio MES 412 OS-V2 or MRSH 412 M25 (Custom IR replaces both Cab + Mic blocks)
   └── Master Output Level: 90 – 95%
   │
   ▼  **CRITICAL CABLE:** Short (<3m) 1/4" TRS Male ──> Dual RCA Male Insert ("Y") Cable
[Rupert Neve Designs RNHP — INPUT B (Unbalanced RCA, -10dBV)]
   │  (NEVER connect Radar TRS output into RNHP Input A Balanced TRS — causes phase cancellation!)
   ▼
[Reference Studio Headphones (Sennheiser HD600/HD650, Beyerdynamic DT 1990 Pro, Focal Clear)]
```

---

## 2. Rupert Neve Designs RNHP (Headphone Precision Amplifier)

The **RNHP** (**Rupert Neve Headphone Precision** amplifier) is a dedicated studio reference headphone amplifier derived directly from the output circuit of the flagship Rupert Neve 5060 Centerpiece console.

### Official Hardware Specifications & Engineering Advantages
* **High-Voltage +24V DC Operating Rail:** Runs on a 24V DC (@ 0.25A min / 6W) power rail. High-gain guitar palm mutes and 7-string low-B transients produce massive crest-factor voltage swings; while 5V USB interfaces and 12V micro-pedals clip and compress, the RNHP reproduces every pick transient cleanly (**+22.8 dBu maximum input headroom** on Input A).
* **Near-Zero Output Impedance (`0.08 Ω` at 1kHz):** Provides a damping factor >1800 into 150Ω–300Ω headphones, ensuring zero frequency-response skewing across everything from 16Ω custom IEMs to 600Ω studio cans.
* **Ultra-Wide Bandwidth (`±0.2 dB` from `10 Hz to 120 kHz`) & Precision Volume Pot:** Preserves natural room-mic air and stereo/mono depth down to whisper-quiet bedroom monitoring levels without left/right channel imbalance.

### RNHP Input Selection & The Mooer Radar "Phase Cancellation" Trap

The RNHP features three selectable rear inputs controlled by the front-panel `A / B / C` pushbuttons:
* **Input A (Dual XLR / 1/4" TRS Combo Jacks):** Calibrated for **+4 dBu Balanced Line Level** (`Zin = 10 kΩ`). Use **Input A** when connecting the **Mesa Mark VII Balanced XLR CabClone Out** or the balanced Left/Right TRS outputs of a professional studio audio interface.
* **Input B (Stereo Unbalanced RCA Jacks):** Calibrated for **-10 dBV Unbalanced Consumer/Pedal Line Level** (`Zin = 10 kΩ`).
* **Input C (3.5mm / 1/8" TRS Stereo Mini-Jack):** Calibrated for smartphones/laptops (`Zin = 6.8 kΩ`).

> **CRITICAL WIRING WARNING (Why You Must Use `Input B` with the Mooer Radar):**
> * The **Mooer Radar's 1/4" Output jack is a TRS Stereo (Dual-Mono) unbalanced output**—it sends the exact same mono guitar signal on both the **Tip (Left)** and **Ring (Right)** contacts so that standard headphones hear sound in both ears.
> * **RNHP Input A (Combo Jack) is a Mono Balanced Differential Receiver.** If you plug a 1/4" TRS cable from the Mooer Radar into **one** RNHP Input A jack, the differential amplifier subtracts the Ring signal from the Tip signal (`Tip - Ring = 0`) to cancel noise—which **cancels out 98% of your guitar signal**, leaving a ghostly, hollow, out-of-phase whisper in only one ear!
> * **The Correct Cable & Connection:** Connect a **1/4" TRS Male to Dual RCA Male Insert ("Y") Cable** (kept under **3 meters / 10 feet** to avoid high-frequency roll-off and EMI hum) from the **Mooer Radar 1/4" Output** into **RNHP Input B (Left & Right RCA)** and press the **`B` button** on the front of the RNHP. This delivers a rock-solid, phase-coherent dual-mono signal to both ears at the exact `-10dBV` gain calibration the Radar outputs.

---

## 3. Mooer Radar Setup & Optimization

The **Mooer Radar** is a dedicated 24-bit / 44.1kHz impulse response loader and power-amp simulator containing **36 user-saveable preset slots**.

### Block-by-Block Configuration for Tube Amps

1. **`POWER` (Power Amp Simulation Block):**
   * **With Mesa Mark VII (`LINE OUT`):** Set to **`OFF`**. Because the Mark VII `LINE OUT` is tapped **post-power-amp** (from the internal reactive load / speaker path), real 6L6 Simul-Class tube compression is already present.
   * **With Marshall JVM 410C (`FX SEND` in Standby Mode) or DSL5C (`FX SEND`):** Set to **`ON`** and select **`EL34`** (for JVM) or **`EL84 / EL34`** (for DSL5C) with `Input Gain: 12:00`, `Presence: 12:30–1:00`, `Output Level: 12:00`. Because the JVM's power section is turned off in Standby mode, this restores the essential British output-transformer sag and smooths out raw preamp fizz.
2. **`CAB` (Cabinet & Microphone Block — Custom IR Behavior):**
   * When you load a third-party `.wav` Impulse Response (like **York Audio**) into a Mooer Radar slot, **the custom IR automatically replaces BOTH the factory Cabinet model AND the factory Microphone/Distance simulation**.
   * You do not need to worry about the Radar's internal mic model or mic position settings once a custom `[U]` user IR is loaded, because York Audio IRs are already mastered, phase-aligned multi-mic captures.
3. **`EQ` (Post-Cabinet Parametric / Graphic EQ Block):**
   * The Radar's `EQ` block remains **100% independent** of the loaded IR.
   * Set `EQ` to **`CUSTOM (P)`** (Parametric Mode) and engage:
     * **HP (High-Pass Filter): `80 Hz – 90 Hz`** (cuts non-musical sub-rumble that muddies headphones).
     * **LP (Low-Pass Filter): `7.5 kHz – 8.5 kHz`** (rolls off ultra-high digital sizzle for an authentic in-the-room speaker feel).

### Connecting Mooer Radar to PC / Mac (USB Procedure)
1. **Power First:** Connect the **12V DC (300mA)** power supply to the Mooer Radar first. **USB bus power alone will NOT power on the Radar.**
2. **USB Cable:** Connect a data-capable **Micro-USB cable** *(not Mini-USB)* from the side of the Radar to your Mac or PC.
3. **Mooer Studio for Radar Software:** Launch the editor, select a preset slot (`1–36`), and click the **`+` (Import)** icon next to the Cabinet name.
4. **Sample Rate Requirement:** Select the **44.1kHz / 24-bit** `.wav` folder from your York Audio download (the Radar converts longer IRs to its native 23.2ms / 1024-sample resolution automatically). Click **Save** inside the software before unplugging.

---

## 4. Cabinet Impulse Responses: York Audio & Bogren Digital

### Why York Audio Outperforms Factory Stock IRs
Factory IRs pre-loaded on the Mooer Radar and Mesa CabClone often sound boxy or one-dimensional because they rely on single static microphones placed flat against the grille. **York Audio** captures cabinets using proprietary phase-aligned multi-mic blends (combining vintage **Shure SM57**, **Shure SM57 Unidyne III**, **Royer R-121 Ribbon**, **Beyerdynamic M160 Ribbon**, **Shure SM7B**, and **Neumann U47 FET**), capturing the full three-dimensional wood resonance and speaker breakup.

### Master IR Pack & Mix Selection Guide

| IR Pack | Physical Cabinet & Speakers | Recommended Specific Mixes | Best Matched Amp, Guitar & Artist Tone |
| :--- | :--- | :--- | :--- |
| **York Audio `MES 412 OS-V2`** | **Mesa/Boogie Rectifier Standard ("Oversized" 4x12)** loaded with 2001 UK-made **Celestion Vintage 30s** | • **`Mix 01` *(57m + 121)*:** Balanced studio gold standard; liquid leads & versatile rhythm.<br>• **`Mix JP` *(Petrucci Spec)*:** Dual SM57s + Royer R-121; ultimate **Dream Theater / Mark IIC+ & IV** mix.<br>• **`Mix FRED` *(Dual Angled/Straight SM57s)*:** Mid-focused Fredman cut; nails **Tool (Adam Jones)** & dense mixes.<br>• **`Mix 07` *(57m + 160)*:** Tighter sub-bass; great for **Linkin Park Drop C#** & **Heafy 7-String**. | **Mesa Mark VII (Ch 2 & 3)**, Majesty 6, Reaper-6, Heafy 7; Dream Theater, Metallica, Tool, Linkin Park, Trivium. |
| **York Audio `MRSH 412 M25`** | **1976 Marshall 1960A/B "Checkerboard" 4x12** loaded with pre-Rola/70s **Celestion G12M-25 Greenbacks** | • **`Mix 08` *(57v + 160)*:** Vintage SM57 + Beyer M160 ribbon; pure 80s NWOBHM **Iron Maiden / Judas Priest** bark.<br>• **`Mix 01` *(57m + 121)*:** Fuller low-end warmth; ideal for **Joe Satriani**, **Rush**, & **Ozzy**.<br>• **`Mix 09` *(SM7 + 121 — Leon Todd Mix)*:** Tightest Greenback mix; tames high-gain **OD2 / 7-String** through the JVM. | **Marshall JVM 410C** & **DSL5C**, Schecter Reaper, Heafy 7 (Voice 2/3); Iron Maiden, Deep Purple, Led Zeppelin, Satriani. |
| **Clean Cabinet IRs** *(For Ch 1 Cleans)* | Open-Back 2x12s with Celestion C90s, Alnico Blues/Golds, or JBL D120F | • **Mark VII Factory Slot 6:** *2x12 Lone Star Open-Back (C90s)* — already built into your Mark VII!<br>• **`York Audio MTCH 212 ESD-V2`:** Matchless 2x12 (G12H30 + G12M25) — glassy, 3D chime.<br>• **`York Audio FTWN 212 D120`:** 1971 Fender Twin Reverb w/ JBL D120F — crystal-clear clean headroom. | **Mesa Mark VII (Ch 1)** & **JVM Clean Green**; *"Pull Me Under"*, *"The Spirit of Radio"*, Majesty Piezo/Split cleans. |
| **Bogren Digital `Downtuned Rhythm IR Pack`** | Custom Jens Bogren cab captures pre-EQ'd specifically for 7/8-string low tunings | • **`Drop Tune` / `Sub-Tight` Mixes:** Pre-sculpted low-mid cleanup that needs zero post-EQ in a mix. | **Epiphone Heafy 7-String (B-Standard & Drop A)** when you want instant mix-ready modern metalcore. |

---

## 5. Mesa/Boogie Mark VII CabClone IR USB Procedure

Unlike the Mooer Radar, the Mesa/Boogie Mark VII **does NOT require any proprietary software application**. When connected via USB, the Mark VII mounts directly on your Mac or PC desktop as a **standard USB Mass Storage Device (external flash drive)**.

### Step-by-Step Drag-and-Drop IR Loading Instructions

1. **Power & Load Setup:** Ensure the Mark VII is either connected to its speaker cabinet **or** has the rear **`SPEAKER OFF`** switch engaged (activating the internal reactive load). Power the amplifier on (it can remain in **Standby**).
2. **USB Connection:** Connect a **USB 2.0 Type-A to Type-B cable** (standard printer-style USB cable) from the Mark VII's rear `USB` port to your computer.
3. **Open the Mounted Drive:** Within a few seconds, a drive named **`CABCLONE IR`** (or `MESA_BOOGIE`) will appear in **macOS Finder** or **Windows File Explorer**.
4. **Understand the 8 Global Folder Slots (`1` through `8`):**
   * Inside the drive, you will see **8 numbered folders (`1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`)** plus a backup/factory folder.
   * These 8 folders are **shared globally across all 3 channels**—each channel's physical 8-position rotary switch on the back of the amp simply points that channel to whichever folder (`1`–`8`) you dial it to!
5. **Backup & Replace Files (`48kHz / 24-bit WAV` Requirement):**
   * Copy the entire contents of the `CABCLONE IR` drive to a folder on your computer hard drive first as a backup.
   * Open your **York Audio `48kHz - 24bit` folder** (*Note: Use the **48kHz** folder for the Mesa Mark VII, and the **44.1kHz** folder for the Mooer Radar!*).
   * To replace an IR (for example, Slot 8), open Folder **`8`**, **delete** the existing factory `.wav` file inside that folder (each folder can only contain **one** `.wav` file at a time!), and drag-and-drop your new York Audio `.wav` file into Folder `8`:
     * **Folder `4`** -> `YA MES 412 OS-V2 Mix 01.wav` *(Singing Lead / All-Rounder)*
     * **Folder `6`** -> *Leave Factory `2x12 Lone Star Open Back` (for Channel 1 Cleans)*
     * **Folder `7`** -> `YA MES 412 OS-V2 Mix FRED.wav` *(Channel 2 Crunch / Tool Rhythm)*
     * **Folder `8`** -> `YA MES 412 OS-V2 Mix JP.wav` *(Channel 3 Mark IIC+ & IV Petrucci Rhythm)*
6. **Safely Eject:** Right-click the `CABCLONE IR` drive and click **Eject** (macOS) or **Safely Remove Hardware** (Windows). The rear CabClone status LED will flash briefly as it indexes the new IRs and return to solid operation.

---

## 6. Transitioning to Digital Modelers & DAWs

When recording directly into a DAW or building a portable digital fly-rig alongside your tube amps:

### Software Amp Modelers & Plugins
* **Neural DSP Archetype: Petrucci X:** Purpose-built around your exact tonal ecosystem. Includes a dedicated **Piezo Acoustic simulator** (for the Majesty), a **Multiband Compressor**, **Mark IIC+ / Mark IV** rhythm and lead amps, a **4-Band Parametric + 9-Band Graphic EQ**, **Room Mic emulation**, a real-time **Transpose (-12 to +12 semitones)** knob, and a **Stereo Doubler** that creates an instant double-tracked wall of sound in headphones.
* **Neural DSP Archetype: Gojira X / Mesa Boogie Mark IIC+ Suite:** Official licensed Mesa/Boogie Mark IIC+ / IIC++ suite and crushing 7-string downtuned metal engines.

### Audio Interface Requirements (Preventing Active Pickup Clipping)
* **High-Headroom JFET Hi-Z Input (`≥ +12 dBu`):** Active pickups like the **Fishman Fluence Voice 1** on the Heafy 7-String output massive peak voltage transients (`~4V peak-to-peak`). Entry-level interfaces (like early Focusrite Scarlett Solo/2i2 Gen 1/2) clip their instrument inputs even with the input gain turned all the way down to zero!
* **Recommended Interfaces:** **Audient iD14 / iD24 MKII** (discrete Class-A JFET DI + ADAT expandability), **MOTU M2 / M4** (ESS Sabre32 Ultra DACs with ultra-low RTL latency), or **Universal Audio Apollo Solo / Twin X**.

### Standalone Hardware Modelers Comparison

| Platform | Modeling / Capture Technology | Strengths | Best Use Case |
| :--- | :--- | :--- | :--- |
| **Fractal Audio (Axe-FX III / FM9 / FM3)** | Component-level SPICE circuit modeling (`Cygnus X-3`) | Deepest Mesa Mark IIC+/IV & Marshall authenticity; studio-grade effects used by **John Petrucci**, **Metallica**, and **Steve Vai** live. | Ultimate studio flagship and deepest progressive metal parameter tweaking. |
| **Neural DSP Quad Cortex** | Hybrid Component Modeling + **Neural Capture V2** + **Plugin Compatibility (`PCOM`)** | 7" multi-touch screen, rotary footswitches, runs **Archetype: Petrucci X** natively on the hardware, and can **Neural Capture your own Mark VII & JVM 410C**! | Cloning your physical tube amps into a backpack-sized floorboard. |
| **Line 6 Helix Floor / LT / Stadium** | HX Dual-DSP Modeling | Fastest, most intuitive scribble-strip workflow and rock-solid MIDI/switching integration with external tube amps. | Seamless 4-Cable Method effects processor + backup modeler. |
