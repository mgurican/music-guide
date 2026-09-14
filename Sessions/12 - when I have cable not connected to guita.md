# when I have cable not connected to guita
**URL:** [https://gemini.google.com/app/fffe3a9cf3ba22c7](https://gemini.google.com/app/fffe3a9cf3ba22c7)  
**Date:** Apr 19, 2026, 8:50:15 PM CEST  
**Total Prompts:** 7  
**Tags:** #session #music_guide #gemini

---
## Overview Links
* Return to [[Home]] | [[Tone Presets]] | [[Hardware & Routing]] | [[Guitars & Pickups]]

---
## Conversation History

### 1. [Apr 19, 2026, 8:50:15 PM CEST] Prompt
> **when I have cable not connected to guitar and i touch jack on end of my pre-amp loop i feel electric energy, is that ok, or I have to worry about something?**

#### Gem Response
Feeling "electric energy" or a tingling sensation when touching the jack of an active instrument cable is **not normal and is a serious safety hazard.** You must address this immediately before continuing to play.
This sensation indicates that stray AC voltage is traveling through the audio path and using your body as a path to earth ground. Given that you are running high-voltage tube amplifiers (the Mesa Boogie Mark VII and Marshall JVM410c operate with internal plate voltages exceeding 450V DC), any grounding failure can be lethal.
Here is a technical breakdown of the potential causes in your specific rig and how to diagnose them:

### 1. Wall Outlet Grounding Failure

* **The Issue:** The most common cause of stray voltage on a guitar chassis (and by extension, the cable sleeve/jack) is a missing or faulty earth ground at the wall receptacle. If the amp cannot dump stray current to earth, it sends it through the chassis and down the guitar cable.
* **Action:** Purchase a standard AC receptacle tester. Plug it into the wall outlets powering your Mesa, Marshall, and pedalboard. If it indicates "Open Ground," do not use that outlet.

### 2. Multi-Amp Ground Potential Differences

* **The Issue:** You own both a Mark VII and a JVM410c. If you are running them simultaneously in a stereo or wet/dry configuration using your TC Electronic delays, you may have created a massive ground loop. If the amps are plugged into different circuits with slightly different ground potentials, AC voltage will travel across the shield of your patch cables to equalize, resulting in a shock when you become the bridge.
* **Action:** If running a multi-amp rig, you must use a high-quality, transformer-isolated ABY splitter (like a Radial Tonebone or Lehle) to lift the ground on one of the amplifiers and isolate the signal paths safely.

### 3. Pedalboard Power Supply Leakage

* **The Issue:** If you are using a cheap, daisy-chained, or non-isolated power supply for your pedals (especially high-draw digital units like the TC Triple Delay or Dreamscape), switch-mode leakage current can enter the audio ground path.
* **Action:** Ensure you are using a professional-grade, fully isolated toroidal power supply (e.g., Voodoo Lab Pedal Power 3, Strymon Zuma). To test if the pedalboard is the culprit, plug your guitar directly into the front of the Mesa Mark VII with no pedals connected. If the shock disappears, your pedal power supply or a specific pedal is leaking voltage.

### 4. Amplifier Component Failure

* **The Issue:** While both the Mark VII and JVM410c are modern amps with robust safety standards, a failing filter capacitor, a shorted power tube, or a compromised power transformer can leak mains voltage directly to the chassis.
* **Action:** If your wall outlets test perfectly, and bypassing the pedalboard does not solve the issue, immediately power down the amplifier, unplug it from the wall, and take it to a certified tube amp technician. Do not attempt to open the chassis yourself; filter capacitors hold lethal charges long after the amp is powered off.

Safety must be the absolute priority when managing an advanced, multi-stage gain rig.
Are you currently running the Mesa Mark VII and the Marshall JVM410c at the same time in a stereo/split configuration, or does this issue occur when playing through just one isolated amplifier?

---

### 2. [Apr 19, 2026, 8:55:14 PM CEST] Prompt
> **I have daisy chained power suplies powering wah, and other one rest of pre-amp pedals - ts, sd1 and spark, and last one powering dreamscape and marshal delay should. Is Harley Benton PowerPlant ISO-12 Pro good solution ?**

#### Gem Response
Yes, switching to the **Harley Benton PowerPlant ISO-12 Pro** is an excellent and highly recommended move for your specific rig.
Daisy-chaining power, especially when mixing analog drives (TS808, SD-1) with high-draw digital modulation and time-based effects (TC Triple Delay, Dreamscape), is a recipe for disaster. It introduces ground loops, digital clock noise bleed into the audio path, and, as you've experienced, potential stray leakage current.
Here is an honest breakdown of the ISO-12 Pro and how it impacts your signal chain:

### Pluses (The Good)

* **True Output Isolation:** All 12 outputs are individually isolated and filtered. This instantly breaks the ground loops between your front-of-amp pedals and your FX loop pedals, completely eliminating the stray voltage bridge that is likely causing your shocks.
* **High Current Headroom:** Digital pedals are power-hungry. Your TC Triple Delay requires around 300mA. The ISO-12 Pro offers nine outputs at 300mA and three outputs at 500mA. This guarantees your digital units will never be starved for current, which prevents digital clipping and artifacting.
**Switchable Voltages:** The three 500mA outputs can be switched between 9V, 12V, and 18V.

* *Pro-Tip:* You can run your Boss SD-1 or TC Spark Mini at 18V (always check your specific pedal's manual first) to drastically increase their dynamic headroom. Running drives at 18V into your Marshall JVM410c will give you a less compressed, more articulate pick attack perfectly suited for classic Rush and Deep Purple tones.

* **Cost-to-Performance Ratio:** It performs exceptionally well for the price, rivaling units from Strymon and Voodoo Lab that cost two to three times as much.

### Minuses (The Drawbacks)

* **Wall-Wart Power Supply:** Unlike higher-end units (like the Voodoo Lab Pedal Power 3 or Truetone CS12) which use a heavy-duty internal transformer and plug directly into the wall via a standard IEC cable, the ISO-12 Pro relies on an external 12V/3A wall-wart adapter to power the brick. Wall-warts can be flimsy and take up awkward space on a power strip.
* **Cable Lengths:** The included DC patch cables are 60cm. If your pedalboard is exceptionally wide, you might find these cables slightly short to reach the furthest routing points cleanly.
* **Total Wattage Limit:** The total output load cannot exceed 27 Watts. While your current pedals won't hit this ceiling, if you were to add multiple massive multi-effects units later (like a Quad Cortex or Line 6 HX Stomp), you would max out the adapter's capability.

### The Verdict for Your Rig

The Harley Benton ISO-12 Pro will immediately lower the noise floor of your high-gain Mesa and Marshall channels, eliminate the digital whining from the Dreamscape/Delays, and resolve your grounding hazard. It is a highly practical, budget-conscious, and effective solution.
Before you map out your new pedalboard routing, are you planning on running any of your drive pedals (like the Spark or SD-1) at 18V to maximize their headroom, or do you prefer the compressed feel of standard 9V operation?

---

### 3. [Apr 19, 2026, 9:03:34 PM CEST] Prompt
> **is it safe to run them at 18v?**

#### Gem Response
No, it is **not safe** to run your specific drive pedals (Ibanez TS808, Boss SD-1, and TC Spark Mini) at 18V. Doing so will permanently damage them.
While some boutique pedals feature internal charge pumps or higher-rated components to handle 18V for increased headroom, standard mass-produced classics are strictly designed for 9V DC.
Here is the technical breakdown of why feeding 18V to your current front-of-amp board is a critical error:

* **Ibanez TS808 Tube Screamer:** The standard TS808 circuit utilizes electrolytic capacitors in the power filtering section that are typically rated for a maximum of 16V DC. Hitting them with an 18V supply will cause the dielectric to fail, resulting in capacitor rupture and a dead pedal.
* **Boss SD-1 Super Overdrive:** Modern PSA-style and SMD (Surface Mount Device) versions of the SD-1 are strictly 9V. Like the TS808, the internal filter capacitors and the specific operational amplifiers used are not spec'd to handle an 18V load. Overvoltaging will fry the circuit. *(Note: Vintage Japanese ACA-powered SD-1s required 12V isolated power to drop down to 9V internally, but they still cannot handle 18V).*
* **TC Electronic Spark Mini:** TC Electronic strictly specifies 9V DC (center negative) for this unit. Supplying 18V will instantly destroy the internal components.

### The Sonic Reality for Your Rig

Since your goal is to tighten up the Mesa Boogie Mark VII and Marshall JVM410c for articulately defined gain (Tool, Dream Theater, Deep Purple), running your TS808 and SD-1 at 9V is actually the optimal, standard practice for your setup.

* **Compression is Key Here:** At 9V, the TS808 provides the exact amount of symmetrical clipping, compression, and low-end roll-off (~720Hz) needed to focus the low B of your 7-string Epiphone and the crunch of your Schecter Reaper into the Mesa. If it had 18V headroom, it would let too much uncompressed transient bass through, defeating its purpose as a surgical tightening tool.
* **Marshall Synergy:** The SD-1 at 9V provides the aggressive, squashed asymmetrical bite necessary to push the Marshall JVM410c into authentic, saturated 80s Iron Maiden and Judas Priest territory.

Keep the Harley Benton ISO-12 Pro outputs strictly set to **9V** for your entire current pedalboard to ensure safe, noiseless operation.
If you want to experiment with the uncompressed, massive transient headroom of 18V operation in the future, you must invest in overdrives specifically engineered for variable voltage. For your specific tastes, the **Horizon Devices Precision Drive** (built with modern prog/Dream Theater in mind) or the **Fulltone OCD** are excellent 18V-capable additions.

---

### 4. [Apr 19, 2026, 9:18:52 PM CEST] Prompt
> **are there any other devices that also resolves this issue, but have some additional benefits like being able to turn on multiple pedals at once?**

#### Gem Response
To give it to you straight: combining a high-current isolated power supply and a programmable loop switcher into a single chassis is incredibly rare in the professional tier.
While there are budget all-in-one units on the market (like the Vitoos VMPS-4), they are severely underpowered. They usually max out at 100mA per output, which will instantly starve your TC Electronic Triple Delay and introduce massive digital clock noise. Furthermore, cramming power transformers into the same chassis as mechanical audio relays often raises the noise floor—exactly what we are trying to avoid for your high-dynamic-range tones.
For a rig boasting a Mesa Mark VII and Marshall JVM410c, you need to use the industry-standard approach: **Separate the power from the brain.** You run a dedicated isolated power supply (like the Harley Benton ISO-12 Pro or a Strymon Zuma) and feed that power into a **Programmable Loop Switcher**.
A programmable loop switcher (like the **Boss ES-5**, **Boss ES-8**, or the budget-friendly **Joyo PXL-Live**) acts as the central command station for your pedalboard. You plug every pedal into its own individual effects loop on the switcher.
Here is the honest breakdown of integrating a programmable switcher into your specific setup:

### Pluses (The Good)

* **Single-Stomp Scene Changes:** This is exactly what you are asking for. You can program "Patches." Patch 1 could be your heavy Dream Theater rhythm (TS808 engaged, everything else bypassed). Patch 2 could be your John Petrucci solo tone (Spark Mini, Dreamscape, and TC Delay engaged). One stomp switches all four pedals simultaneously.
* **Ultimate Tone Preservation:** When a pedal is not engaged on a loop switcher, it is physically removed from the signal chain via true bypass relays. This prevents the buffers of your Boss SD-1 or Ibanez TS808 from coloring your clean tone, ensuring the Rachmaninov-esque acoustic clarity you value remains pristine.
* **MIDI Amp Integration (The Game Changer):** Both your Mesa Mark VII and Marshall JVM410c are MIDI-capable. A switcher like the Boss ES-5 or Joyo PXL-Live can send MIDI commands. One stomp can simultaneously turn on your overdrive, kick on your delays, *and* switch the Mark VII from the Clean channel to the Mark IIC+ mode.

### Minuses (The Drawbacks)

* **Pedalboard Real Estate:** Loop switchers are large. A Boss ES-8 takes up massive space on the front row of your board, meaning you may need to upgrade to a larger pedalboard strictly to accommodate the brain.
* **Cable Nightmare:** Because every pedal needs a "Send" and a "Return" cable, you are instantly doubling the amount of patch cables on your board. This requires a significant investment in custom-length, high-quality patch cables (like Evidence Audio or George L's) to keep things tidy and reliable.
* **The Learning Curve:** You are transitioning from a plug-and-play setup to an IT project. Programming the patches, assigning MIDI PC/CC messages to your amps, and organizing the routing takes time and patience.

If you want the ultimate, tap-dancing-free control over your Iron Maiden and Tool tones, pairing an isolated power supply with a programmable switcher is the only professional way forward.
Since your pedalboard is currently split between the front-of-amp (drives) and the FX Loop (delays/modulation), would you want a switcher capable of managing the 4-cable method to route pedals to both locations, or do you prefer keeping the FX loop pedals on their own separate, manually controlled board?

---

### 5. [Apr 20, 2026, 5:53:42 AM CEST] Prompt
> **Why chaining causes me to feel electricity at cable?**

#### Gem Response
To give it to you straight: the daisy chain itself isn't generating the electricity, but it is acting as a massive highway for a phenomenon known as **Leakage Current**.
The tingle you feel is the result of using ungrounded power supplies paired with the physical nature of how guitar pedal circuits share audio and power grounds.
Here is the exact technical breakdown of why this happens when you touch the end of your unplugged cable:

### 1. The Source: Switch-Mode Power Supplies (SMPS)

The wall adapters (wall warts) typically used to power daisy chains are almost always 2-prong, Class II power supplies. This means they do not have a dedicated connection to Earth ground. To pass strict electromagnetic interference (EMI) regulations, these cheap adapters use internal components called **"Y-Capacitors."** * These capacitors bridge the high-voltage AC mains side of the adapter to the low-voltage DC side (the 9V side that goes to your pedals) to filter out digital noise.

* The byproduct of this design is that it intentionally leaks a tiny, usually non-lethal amount of AC mains voltage (often around half your wall voltage, which is roughly 115V AC in Czechia) onto the DC negative wire.

### 2. The Daisy Chain Highway

In a standard guitar pedal, the DC negative (power ground) is physically soldered to the audio jack sleeves (audio ground) and the metal chassis of the pedal.

* When you use a daisy chain, you are linking the DC negative of every single pedal together.
* This means that the AC leakage current from that cheap wall adapter floods the metal casings, the patch cables, and the audio ground of every pedal on your board simultaneously.

### 3. You Become the Earth Ground

Electricity always seeks the path of least resistance to the earth.

* Normally, when your pedalboard is plugged into your Mesa Mark VII or Marshall JVM410c, and those amps are plugged into a properly grounded 3-prong wall outlet, that AC leakage current travels safely down your guitar cable, into the amplifier's chassis, and straight into the wall's earth ground. You never feel a thing.
* However, you mentioned you feel the electricity when the cable is **not connected to the guitar**. If the amp happens to be off, or if the pedals are physically disconnected from the amp at that moment, that floating AC leakage has nowhere to go.
* When your hand touches the metal jack of the cable, **you become the earth ground**. The AC current travels out of the Y-capacitor, through the daisy chain, down the audio cable, into your fingers, through your body, and into the floor.

### The Resolution

This specific "tingle" from an SMPS adapter is usually measured in harmless micro-amps, but it is incredibly annoying and points to a noisy, ungrounded power foundation. Upgrading to an isolated power supply prevents power ground sharing, heavily filtering this noise. *(Note: Even with high-end gear, always ensure your amplifiers are plugged into properly earthed wall outlets to dump any stray current safely).*
To pinpoint the exact source of the leakage on your current board: Are the power adapters you are currently using for those daisy chains standard 2-prong plastic wall warts, or do they feature a 3-prong grounded plug?

---

### 6. [Apr 20, 2026, 5:56:44 AM CEST] Prompt
> **How does Harley powerstation help with this? It doesn't have 2 pole power supply as well?**

#### Gem Response
That is an incredibly sharp observation. You are absolutely correct: the Harley Benton ISO-12 Pro uses a 2-prong power adapter, which means the adapter itself is still generating that exact same AC leakage current.
So, how does it solve the problem? The answer comes down to a crucial piece of internal engineering called **Galvanic Isolation**.
Here is exactly how the ISO-12 Pro traps the leakage current before it can reach your fingers:

### The Magic of Galvanic Isolation

While the 2-prong wall adapter sends leakage current into the main input of the Harley Benton brick, the outputs that connect to your pedals are fundamentally separated from that input.

* **Inside the Brick:** The ISO-12 Pro uses individual **DC-to-DC isolation transformers** for each of its 12 outputs.
* **Magnetic Transfer, Not Direct Wire:** A transformer works by transferring electrical energy across a gap using a *magnetic field*. There is literally no continuous, physical copper wire connecting the power input of the brick to the power outputs going to your pedals.
* **The Blockade:** Because the physical electrical path is broken by these transformers, the AC leakage current from the 2-prong wall adapter is trapped at the input stage. It cannot physically cross the magnetic gap to enter your pedals, your patch cables, or your guitar jack.

### Daisy Chain vs. Galvanic Isolation (The Summary)

* **Your Current Daisy Chain:** A daisy chain is just one continuous strip of copper wire. The leakage current from the wall wart travels unimpeded down the wire, floods your pedals' metal chassis, and waits at your guitar cable for you to touch it and complete the circuit to earth ground.
* **The Harley Benton ISO-12 Pro:** The leakage current enters the brick, hits the isolation transformers, and stops. Your pedals receive clean DC power transferred magnetically, completely free of the stray AC voltage.

This is also exactly why true isolated power supplies eliminate digital clock noise and ground loop hum. By breaking the continuous physical connection between every pedal, you prevent them from sharing a noisy ground path.
Since you are running highly sensitive pedals in both the front of the amp and in the FX loop of the JVM410c and Mark VII, eliminating these ground loops will drastically improve the noise floor of your high-gain Iron Maiden and Tool tones.
Are you currently noticing a loud hum or squeal when you engage the TC Triple Delay and Dreamscape in your amp's FX loop alongside your front-of-amp overdrives?

---

### 7. [Apr 20, 2026, 6:38:20 AM CEST] Prompt
> **No they are on separate daisy chains**

#### Gem Response
That is actually a very smart, classic routing strategy. By separating the power supplies for your front-of-amp analog drives from your high-draw digital FX loop pedals, you have successfully prevented the digital clock noise of the TC Triple Delay from directly polluting the power rail of your TS808.
However, from a technical routing perspective, running three separate daisy chains still leaves your rig vulnerable to the exact leakage current and noise issues you are experiencing.
Here is the honest breakdown of why those separate daisy chains are still holding your tone back:

### 1. The Audio Ground Loop Trap

Even though your three power supplies are physically separated, **your audio patch cables connect everything together.** * Your TS808 goes into the front of the Mesa Mark VII.

* Your TC Triple Delay connects to the Mesa's FX Loop.
Inside the Mesa, the front input ground and the FX loop ground are tied to the exact same metal chassis.
Therefore, if *any* of those three wall adapters leaks AC current, that current travels down the audio cable shield, hits the amp chassis, and connects the entire rig together. You still have a massive ground loop bridging the front of the amp to the back of the amp.

### 2. Digital-to-Digital Pollution

Your FX loop daisy chain is powering both the TC Electronic Triple Delay and the TC Dreamscape. Both are highly complex digital processors.

* Digital pedals inherently dump high-frequency "garbage" (clock noise and processor whine) back into their negative power ground.
* Because they are on the same daisy chain, the Dreamscape is forcing its digital exhaust directly into the Triple Delay, and vice versa. This artificially raises the noise floor of your delays, masking the high-fidelity acoustic clarity you want for those pristine, Rachmaninov-inspired clean passages.

### The Harley Benton ISO-12 Pro Advantage

Switching to the ISO-12 Pro completely eliminates both of these blind spots.
By powering your TS808, your SD-1, your delays, and your modulation from a single, galvanically isolated brick, you cut the audio ground loops dead in their tracks. The Dreamscape and the Triple Delay will no longer share a power ground, resulting in absolute silence when bypassed and pristine repeats when engaged.
To ensure this power upgrade integrates seamlessly with your physical setup: What specific model of pedalboard are you currently using, and does it have the physical clearance underneath to mount an isolated power brick, or will it need to sit on top next to your pedals?

---
