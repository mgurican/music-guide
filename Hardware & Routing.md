# 🔌 Hardware, Routing & Power Engineering

Return to [[Home]] | [[Amplifiers & Cabinets]] | [[EQ Guide]] | [[Silent Practice & Studio Audio]] | [[Tone Presets]]

---

## 1. Front-of-Amp Pedals (Input Chain) & Drive Gain Staging

Your front-of-amp pedalboard chain conditions dynamics, acoustic piezo resonance, and pre-distortion frequency curves before hitting the amplifier's V1 input tube:

```
[Guitar] ──> [TC HyperGravity] ──> [Boss SD-1] ──> [Ibanez TS808] ──> [TC Spark Mini] ──> [Boss EQ-200 Ch A] ──> [Amp Input]
(Dedicated Majesty Piezo Out) ──> [TC BodyRez] ──> [Clean Amp / Acoustic Input]
```

### Drive & Boost Pedals Technical Comparison

| Pedal | Clipping Circuit | Harmonic Profile | Frequency Curve | Primary Use Case |
| :--- | :--- | :--- | :--- | :--- |
| **Boss SD-1** (Super OverDrive) | **Asymmetrical** (3 silicon diodes: 2 one way, 1 the other) | **Even-order** harmonics (raw, jagged, tube-like grit & aggressive upper-mid bite) | Low cut below ~400Hz with a wider, grittier ~1kHz upper-mid peak | Pushing **Marshall JVM 410C** (Iron Maiden, Judas Priest, Ozzy), raw garage rock (Jack White), or boosting **Heafy 7 (Voice 2 Passive)** |
| **Ibanez TS808** (Tube Screamer) | **Symmetrical** (2 back-to-back silicon diodes in feedback loop) | **Odd-order** harmonics (smooth, compressed, vocal sustain) | Steep sub-bass cut (<720Hz, -6dB/oct) + focused ~720Hz mid hump + treble roll-off | Tightening **Mesa Mark VII** / **Schecter Drop C#** / **7-String** high-gain rhythm, and liquid Petrucci/Satriani solo sustain |
| **TC Electronic Spark Mini** | **Discrete Analog Transistor** (Zero clipping diodes; PrimeTime momentary/latching switch) | Pure linear gain (**up to +20dB**) with zero added diode distortion | 100% flat across the entire spectrum | Compensating coil-split volume drops (Heafy Voice 3), driving JVM Crunch cleanly, or adding front-end saturation |

### Gain Staging Strategies: Front-End Tightener vs. Standalone Drive vs. Stacked Fuzz

1. **Tightening High-Gain Tube Channels (The Modern Metal Formula):**
   * **Pedal Settings:** **`LEVEL` at 9–10 (Max), `DRIVE` at 0–1 (Min), `TONE` at 5–6 (12:00–1:00)**.
   * **Amp Settings:** Lower amplifier channel gain slightly (e.g., Mark VII Gain at `5.0–6.0` or JVM OD1 Gain at `4.0–4.5`).
   * **Physics:** The overdrive acts as a **passive high-pass filter (<720Hz) and clean voltage booster**. It strips away bloated sub-bass *before* the first preamp tube (`V1`) so the low strings cannot cause blocking distortion, while slamming the midrange with high voltage for instant palm-mute recovery and surgical note separation.
2. **When to Use Overdrives Into a Clean Channel (Standalone Drive Mode):**
   * Even when you own multi-channel monsters like the Mark VII and JVM 410C, running the **TS808 or SD-1 with high `DRIVE` (`5–8`) into a Clean or Edge-of-Breakup Channel** unlocks distinct textures that cascading tube channels cannot replicate on their own:
     * **Vintage Op-Amp Diode Compression (Blues / Indie / 70s Rock):** Cascading tube channels have massive dynamic transient swings. Turning the TS808 or SD-1 `DRIVE` up to `6–8` (`LEVEL: 5`, `TONE: 5`) into **Mark VII Channel 1 (Clean/Fat)** or **JVM Clean (Green/Orange)** locks the signal into a tight, spongy diode-clipped ceiling—perfect for SRV/Mayer blues-rock, Rush (*"The Spirit of Radio"* early crunch), or rolling your guitar volume knob from crystal clean to singing crunch without tap-dancing amp channels.
     * **Pedal Stacking into Edge-of-Breakup (80s Hard Rock):** Setting **Mark VII Ch 1 (Crunch)** or **JVM Crunch (Green)** just at the threshold of tube breakup and hitting it with the **Boss SD-1 (`DRIVE: 4`, `LEVEL: 7`)** creates a harmonically complex hybrid of silicon asymmetrical diode clipping and 12AX7 tube saturation.
3. **Stacked Overdrives (`TS808 -> SD-1`) for Raw Garage Rock / Square-Wave Fuzz:**
   * Since the rig does not include a dedicated Big Muff or Fuzz Face, turning **BOTH** the **Ibanez TS808 (`DRIVE: 8`, `LEVEL: 8`, `TONE: 6`)** and **Boss SD-1 (`DRIVE: 8`, `LEVEL: 7`, `TONE: 7`)** ON simultaneously into a dirty Crunch channel cascades symmetrical clipping directly into asymmetrical clipping.
   * This chops the peaks of the guitar waveform into a **splatty, Velcro-like square wave** that nails **Jack White (*Frozen Charlotte* — *"You'll Never Fix Me"* / *"Thick as Thieves"*)** and lo-fi garage punk.

---

## 2. Effects Loop Pedals (Post-Preamp Chain)

Placing modulation and time-based effects in the amplifier's **FX Loop** (after the preamp distortion tubes and after **Boss EQ-200 Channel B**) keeps chorus swirls and delay repeats pristine, wide, and un-smeared:

* **TC Electronic The Dreamscape (John Petrucci Signature Modulation):**
  * Contains 6 custom Petrucci modulation engines (**2x Chorus [Corona], 2x Flanger [Vortex], 2x Vibrato [Shaker]**) plus 1 TonePrint slot, controlled by `SPEED`, `DEPTH`, `FX LEVEL`, and a 3-way `BRIGHT / NORMAL / DARK` voicing toggle.
  * *Petrucci Lush Clean Chorus:* **`CHORUS 1`**, `Speed: 10:00`, `Depth: 2:00`, `FX Level: 1:00`, Switch: `Normal` or `Dark`.
  * *70s Swirling Phaser / Kashmir Texture:* **`FLANGER 2`** (or loaded **Blood Moon Phaser TonePrint**), `Speed: 9:30`, `Depth: 1:30`, `FX Level: 12:00`.
* **TC Electronic Flashback Triple Delay & Marshall Echohead EH-1:**
  * **Flashback Triple Delay:** Runs up to **3 independent delay engines simultaneously** in Series or Parallel with dedicated subdivision control (Quarter, Dotted Eighth, Dual, Ping-Pong) and Tap Tempo. Essential for **John Petrucci (`2290 Dynamic` or `Analog` at 450–550ms)** and **Joe Satriani (Dual Dotted-Eighth + Quarter)**.
  * **Marshall Echohead EH-1:** Compact 6-mode stereo delay (`Hi-Fi, Analogue, Tape Echo, Multi-Tap, Reverse, Mod Filter`). Best set to **`Analogue`** or **`Tape Echo`** for warm rhythmic slapback (`Time: 110–130ms`, `Feedback: 1–2 repeats`) that melts beneath the mix without cluttering fast picking.

---

## 3. Studio Compression: TC Electronic HyperGravity

The **TC Electronic HyperGravity** is a studio-grade digital compressor running the **MD3 multiband dynamics algorithm** ported directly from TC Electronic's flagship **System 6000** mastering processor.

### Hardware Controls & 3-Way Voicing Switch
* **4 Rotary Controls:**
  1. **`SUSTAIN`:** Controls compression ratio and threshold (how much squash and tail sustain is applied).
  2. **`ATTACK`:** Controls transient response time (Counter-clockwise = fast attack that clamps down on initial pick click for smooth legato/cleans; Clockwise = slow attack that lets the raw pick snap punch through before compressing the sustain tail).
  3. **`LEVEL`:** Output makeup gain.
  4. **`BLEND`:** Parallel "New York" compression mix (`Counter-Clockwise = 100% Dry`, `12:00 = 50/50`, `Clockwise = 100% Compressed`). *(Note: There is NO "Tone" knob on the physical pedal; EQ/Spectral tilt is handled internally via the 3-way switch or TonePrint app).*
* **3-Way Mode Toggle Switch:**
  * **`SPECTRA` (Up — Multiband):** Splits the guitar signal into 3 independent frequency bands (Low, Mid, High) and compresses each separately. Low-E/Low-B string palm mutes or bass notes will **never** cause the high strings to "duck" or pump, keeping extended prog chords glassy and surgical.
  * **`TONEPRINT` (Center):** Loads custom artist configurations via the TonePrint app—specifically **John Petrucci's two official signature TonePrints**:
    * **"TransComp" (John Petrucci):** Transparent studio multiband compression tailored for acoustic-like electric cleans and liquid lead sustain.
    * **"EverComp" (John Petrucci):** Higher-ratio sustain compressor designed for endless singing lead lines and shimmering 90s rack cleans.
  * **`VINTAGE` (Down — Single-Band VCA):** Emulates classic analog stompboxes (Ross / MXR Dyna Comp) with warm high-end roll-off and a pronounced percussive "squish" (ideal for 70s/80s Rush, funk, and classic rock).

### Honest Pros & Cons Assessment
* **Pros:** Zero bass-triggered pumping in `Spectra` mode; onboard `Blend` knob preserves natural right-hand pick dynamics; Petrucci's official TonePrints are free and purpose-built for this exact rig.
* **Cons:** Requires **100mA isolated 9V power** (digital DSP); raises the noise floor if left ON in front of high-gain rhythm channels (should be **OFF** for heavy metal rhythm chugging, and engaged **only** for cleans, ambient tapping, or smooth low/mid-gain legato solos).

### Master Compressor Song Dial-In Matrix

| Song / Artist | Mode Switch | Sustain | Attack | Level | Blend | Musical Purpose |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **Dream Theater — *"Pull Me Under"* / *"Take The Time"* (Clean Intro)** | `SPECTRA` (or *EverComp*) | `1:30` | `10:00` (Fast) | `12:30` | `2:00` (70%) | Evens out every cross-picked note across all 6 strings for glossy 90s studio rack shimmer. |
| **Rush — *"The Spirit of Radio"* (Intro & Reggio Clean)** | `VINTAGE` | `1:00` | `1:30` (Slow) | `12:30` | `2:30` (75%) | Classic 1980 analog Ross/Dyna Comp percussive snap and sustained pull-off flurries. |
| **Iron Maiden — *"Wasted Years"* (Intro & Clean Verses)** | `SPECTRA` | `12:30` | `12:00` | `12:00` | `1:30` (65%) | Keeps Adrian Smith's rapid high-E open-string pedal-point intro laser-consistent. |
| **Tool — *"Schism"* / *"Lateralus"* (Clean Bass/Guitar Interludes)** | `SPECTRA` | `12:00` | `2:00` (Slow) | `12:00` | `12:30` (55%) | Preserves woody hammer-on percussive thump while sustaining modal D-drone decay. |
| **Joe Satriani — *"Always With Me, Always With You"* (Clean & Lead)** | `TONEPRINT` (*TransComp*) | `1:00` | `11:00` | `12:30` | `12:00` (50%) | Cushions clean chord arpeggios and adds subtle infinite sustain to singing legato leads. |
| **High-Gain Metal Rhythm (*"One Step Closer"*, *"Master of Puppets"*)** | **BYPASS (OFF)** | — | — | — | — | Tube saturation already compresses 10:1; adding front-end compression causes feedback hiss. |

---

## 4. Master 4-Cable Method (4CM) Signal Routing

To place pre-gain filters/drives in front of the amplifier while routing post-gain EQ sculpting, modulation, and delays inside the amplifier's effects loop, the rig uses the **4-Cable Method (4CM)**:

```
[GUITAR]
   │
   ▼  (Cable 1: Guitar -> Pedalboard Input)
[Pedalboard Front Section]
   ├── TC Electronic HyperGravity Compressor
   ├── Boss SD-1 Super OverDrive
   ├── Ibanez TS808 Tube Screamer
   ├── TC Electronic Spark Mini Booster
   └── Boss EQ-200 [INPUT A ──> OUTPUT A] (Pre-Amp Tightening / Pickup Voicing)
   │
   ▼  (Cable 2: EQ-200 Out A -> Amplifier Front Input)
[AMPLIFIER INPUT (Mesa Mark VII / Marshall JVM 410C)]
   │
   [PREAMP GAIN STAGES & PRE-DISTORTION TONE STACK]
   │
[AMPLIFIER FX LOOP SEND]
   │
   ▼  (Cable 3: Amp FX Send -> EQ-200 Input B)
[Pedalboard Effects Loop Section]
   ├── Boss EQ-200 [INPUT B ──> OUTPUT B] (Post-Preamp Console Sculpt & +3.5dB Solo Boost)
   ├── TC Electronic The Dreamscape (Chorus / Flanger / Vibrato)
   └── TC Flashback Triple Delay / Marshall Echohead
   │
   ▼  (Cable 4: Delay Out -> Amplifier FX Loop Return)
[AMPLIFIER FX LOOP RETURN]
   │
   [POST-LOOP GRAPHIC EQ (Mark VII) & TUBE POWER AMPLIFIER]
   │
   ▼
[SPEAKER CABINET / INTERNAL REACTIVE LOAD / SILENT PRACTICE CHAIN]
```

---

## 5. Power Supply Engineering & Electrical Safety

### Why Daisy Chains Hum & Cause the "Electric Tingle" (Leakage Current Physics)

1. **Ground Loops & Digital Clock Bleed:**
   * When analog drive pedals (TS808, SD-1) and high-current digital DSP pedals (Boss EQ-200, TC Dreamscape, TC Triple Delay, Mooer Radar) share a single daisy-chain wire, they share a **common ground return path**.
   * Digital DSP chips dump high-frequency switching noise (PWM clock pulses at 16–48kHz) onto the ground wire. Because your guitar amplifier is also grounded to the wall outlet, a **ground loop antenna** is formed between the pedalboard and the amp, amplifying a constant 50/60Hz hum and a high-pitched digital whine into your high-gain channel.
2. **The "Electric Tingle" on Unplugged Guitar Cables (`Y-Capacitor` Leakage Current):**
   * Most cheap 2-prong (Class II ungrounded) switch-mode wall-warts use an internal EMI suppression capacitor (**Y-Capacitor**) bridged between the high-voltage AC primary side and the low-voltage DC ground side to pass FCC emissions tests.
   * When your pedalboard is powered on **without being plugged into a grounded amplifier** (so the ground is "floating"), this Y-capacitor leaks a tiny AC current (~0.1mA – 0.25mA at ~90V–110V AC phantom voltage) onto the sleeves of your guitar cables and metal pedal enclosures. Touching the cable sleeve or strings with bare skin completes the path to earth, creating a harmless but annoying **60Hz buzzing/tingling sensation**.
   * **How to Eliminate It:** Always keep the pedalboard connected to an amplifier with a **grounded 3-prong IEC power cord** (even if the amp is in Standby), which immediately drains the floating leakage voltage to earth ground, **AND** power the board with a transformer-isolated supply.

### Harley Benton PowerPlant ISO-12 Pro Port Mapping & Voltage Safety

The **Harley Benton PowerPlant ISO-12 Pro** uses **12 individually transformer-isolated, filtered outputs** (powered by an external 12V DC @ 3A adapter, 27W max total continuous output), completely breaking ground loops between every pedal:

* **Outputs 1 – 9:** Fixed **9V DC @ 300mA** each (isolated).
* **Outputs A, B, C:** Switchable **9V / 12V / 18V DC @ 500mA** each (isolated).

| Pedal | Required Voltage | Current Draw | Assigned ISO-12 Pro Port | Voltage Safety Warning |
| :--- | :---: | :---: | :--- | :--- |
| **TC HyperGravity Compressor** | **9V DC** (Center Negative) | ~100 mA | **Port 1** (9V @ 300mA) | **Strictly 9V ONLY.** Digital TonePrint DSP will burn out at 12V/18V. |
| **TC Electronic BodyRez** | **9V DC** (Center Negative) | ~100 mA | **Port 2** (9V @ 300mA) | **Strictly 9V ONLY.** |
| **Boss SD-1 Super OverDrive** | **9V DC** (Center Negative) | ~10 mA | **Port 3** (9V @ 300mA) | **Keep at 9V.** |
| **Ibanez TS808 Tube Screamer** | **9V DC** (Center Negative) | ~8 mA | **Port 4** (9V @ 300mA) | **Strictly 9V ONLY.** Requires 3.5mm positive-tip mini-plug adapter if using vintage jack, or standard 2.1mm on newer reissues. |
| **TC Electronic Spark Mini** | **9V DC** (Center Negative) | ~40 mA | **Port 5** (9V @ 300mA) | **Strictly 9V ONLY.** Has an internal voltage doubler; 18V will destroy it. |
| **Marshall Echohead EH-1** | **9V DC** (Center Negative) | ~70 mA | **Port 6** (9V @ 300mA) | **Strictly 9V ONLY.** |
| **TC Electronic The Dreamscape** | **9V DC** (Center Negative) | ~100 mA | **Port 7** (9V @ 300mA) | **Strictly 9V ONLY.** |
| **Boss EQ-200 Graphic EQ** | **9V DC** (Center Negative) | **170 mA** | **Port 8** (9V @ 300mA) | **Strictly 9V ONLY.** High-current DSP easily handled by the 300mA port. |
| **TC Flashback Triple Delay** | **9V DC** (Center Negative) | **300 mA** | **Port A (set to 9V @ 500mA)** | **Strictly 9V ONLY.** Use a 500mA port so startup inrush current never browns out. |
| **Mooer Radar IR Loader** | **12V DC** (Center Negative) | **300 mA** | **Port B (set to 12V @ 500mA)** | **REQUIRES 12V DC.** Set Port B dip-switch to **12V** (mark cable with red tape so it is never plugged into a 9V pedal!). |

---

## 6. Pedalboard Platforms, Mounting & Loop Switchers

### Pedalboard Platform Comparison (For 9–10 Pedals + ISO-12 Pro Underneath)

| Pedalboard Model | Dimensions | Mounting System | Underneath PSU Clearance | Verdict |
| :--- | :--- | :--- | :--- | :--- |
| **Harley Benton Spaceship 60 (or 80)** | `600 x 305 mm` | Standard Velcro / 3M Dual Lock on aluminum rails | **Direct bolt-on elastic/bracket mount** specifically designed for the ISO-12 Pro | **Best Value & Native Fit.** Lightweight, adjustable height feet, zero compatibility headaches. |
| **Pedaltrain Classic 2** | `610 x 317 mm` | **3M Dual Lock (SJ3550)** on open 4-rail frame | Spacious open underside (mounts PSU via Dual Lock or Truetone brackets) | **Industry Standard.** Indestructible touring frame and easiest 4CM cable routing. |
| **RockBoard Quad 4.1 (with MOD 1/2/3)** | `470 x 330 mm` | Slotted grid + QuickMount plates | Fits ISO-12 Pro + integrates a **front-panel patchbay (MOD)** for the 4CM cables | **Cleanest 4-Cable Method Setup.** Plug your 4 amp cables into one central patchbay box. |
| **Temple Audio Duo 24** | `610 x 318 mm` | Proprietary adhesive Quick-Release plates (or Dual Lock) | High clearance + modular side micro-punch plates | Sleekest modular design, though adhesive plates cost extra per pedal. |

* **Mounting Hardware Tip:** Avoid cheap fuzzy hook-and-loop Velcro on heavy pedals like the Triple Delay and EQ-200. Use **3M Dual Lock (SJ3550 250-stem)** applied in `1" x 1"` squares at the 4 corners of each pedal for a rock-solid, rattle-free snap lock.

### Eliminating "Tap Dancing": Programmable Loop Switchers
If you want to press **one single footswitch** to simultaneously switch from a *Pristine Compressed Chorused Clean* to a *TS808-Boosted High-Gain Rhythm* without physically stepping on 4 pedals:
1. **Boss ES-8 / ES-5 Effects Switching System:** Places every analog/digital pedal in its own true-bypass relay loop, supports full 4-Cable Method routing (with a movable preamp insert loop), and simultaneously fires **MIDI PC/CC messages** to the Mesa Mark VII, Marshall JVM 410C, and Boss EQ-200.
2. **Joyo PXL-Live (Budget 8-Loop + Dual MIDI + Amp Trigger Switcher):** Features 2x4 separable loop banks (ideal for splitting Front-of-Amp pedals and FX Loop pedals) plus built-in MIDI Out and 1/4" Relay Triggers for amp channel switching at a fraction of the price.

---

## 7. MIDI Rig Control Architecture

Managing channels, modes, and EQ presets across the **Mesa Mark VII**, **Marshall JVM 410C**, and **Boss EQ-200** simultaneously is achieved by linking them in a single MIDI chain (`Controller 5-Pin MIDI Out -> Amp MIDI In/Thru -> EQ-200 3.5mm TRS MIDI In`).

### How Your Gear Responds to MIDI

| Device | MIDI Connector | Supported Messages | What MIDI Controls |
| :--- | :--- | :--- | :--- |
| **Mesa/Boogie Mark VII** | 5-Pin DIN (`MIDI IN` & `MIDI THRU/OUT`) | **PC (1–128)** & **CC** | Stores and recalls **Channel (1/2/3)**, **5-Band Graphic EQ (On/Off)**, **Reverb (On/Off)**, **FX Loop (On/Off)**, and **CabClone IR / Solo features**. |
| **Marshall JVM 410C** | 5-Pin DIN (`MIDI IN` & `MIDI THRU`) | **PC Only (1–128)** | Recalls 128 user snapshots storing **Channel (Clean/Crunch/OD1/OD2)**, **Mode (Green/Orange/Red)**, **Master 1 vs Master 2**, **Reverb On/Off**, and **FX Loop On/Off**. *(Set JVM setting via front panel, double-press `FOOTSWITCH/MIDI PROGRAM` so LED flashes, then send a PC number from controller to save).* |
| **Boss EQ-200** | **3.5mm TRS MIDI (`Type A`)** (`MIDI IN` & `MIDI OUT`) | **PC (1–128)** & **CC** | Recalls any of the **128 Dual-Channel EQ Presets**, toggles Channel A / Channel B bypass independently, and controls Output Level via CC. |

### Recommended MIDI Foot Controllers

1. **Morningstar MC8 Pro / MC6 Pro (Gold Standard Recommendation):**
   * **Display:** High-contrast color LCD scribble strips above every switch showing exact song/preset names (e.g., *"Pull Me Under Clean"*, *"JP IIC+ Rhythm"*, *"Lead +3.5dB"*).
   * **Connectivity:** 5-Pin DIN MIDI In/Out, USB-C Host/Device, Bluetooth wireless editor, **4x configurable 1/4" Omniports** (each independently assignable as TRS MIDI Out [Type A or B], Expression Pedal In, or Aux Switch In), **PLUS dedicated 3.5mm TRS Relay Switching Ports** (2 ports / 4 relays on MC6 Pro; 4 ports / 8 relays on MC8 Pro) for switching non-MIDI amps like the **Marshall DSL5C** or pedals with external trigger jacks! *(Note: The older non-Pro MC8 requires an external Morningstar Relay Interface box to switch analog amp relays, whereas the **MC6 Pro and MC8 Pro have relay switching built directly inside**).*
   * **Action Engine:** A single switch can fire up to 32 simultaneous MIDI messages across different channels and differently responding actions (`Press`, `Release`, `Double Tap`, `Long Press`).
2. **Disaster Area Designs (DMC.micro Gen4 / MIDI Baby 3):**
   * Ultra-compact footprint if you only want to step through presets on the Boss EQ-200 and one amplifier without taking up pedalboard space.
3. **Behringer FCB1010 (with UnO2 Firmware Chip):**
   * Full-size 10-footswitch floorboard with **2 built-in expression pedals** and **2 built-in 1/4" analog relay jacks**; very affordable and indestructible, though physically massive (`687 x 221 mm`) compared to Morningstar units.
