# what do you recommend as midi controller
**URL:** [https://gemini.google.com/app/e175eb546bc13462](https://gemini.google.com/app/e175eb546bc13462)  
**Date:** Mar 24, 2026, 2:02:29 PM CEST  
**Total Prompts:** 1  
**Tags:** #session #music_guide #gemini

---
## Overview Links
* Return to [[Home]] | [[Tone Presets]] | [[Hardware & Routing]] | [[Guitars & Pickups]]

---
## Conversation History

### 1. [Mar 24, 2026, 2:02:29 PM CEST] Prompt
> **what do you recommend as midi controller for my rig? and, please explain why?**

#### Gem Response
Managing a rig with a **Mesa Boogie Mark VII** and a **Marshall JVM410C**—especially with your collection of progressive and shred-oriented guitars—requires a controller that can handle multi-device mapping without a "pedal dance." You aren't just switching channels; you are coordinating two distinct amp architectures and a deep effects chain.

### The Recommendation: Morningstar MC8 Pro

For your specific gear and musical tastes (Petrucci-style complexity, Satriani fluidity, and Tool-esque atmospheric shifts), the **Morningstar MC8 Pro** is the superior choice over industry standards like the Voodoo Lab Ground Control or the Boss ES series.

#### Why the MC8 Pro fits your rig:

* **Dual Amp Management:** The Mark VII is fully MIDI-capable (Channels 1-3, EQ, Reverb, FX Loop), while the JVM410C is a "MIDI Learn" machine. The MC8 Pro allows you to send unique MIDI Program Changes (PC) and Control Changes (CC) to both amps simultaneously. You can engage the Mark VII’s Graphic EQ for a *Dream Theater* lead and simultaneously switch the JVM to a dry Crunch mode for a *Deep Purple* rhythm layer.
* **Omniports for Non-MIDI Integration:** Your pedalboard has several "standard" pedals. The MC8 Pro’s **Omniports** can act as TRS MIDI outputs, expression inputs, or—crucially—**Relay Switches**. If you ever want to switch a non-MIDI function on an older piece of gear, the MC8 handles it without an external switcher.
**Action-Based Programming:** Unlike older controllers, the MC8 allows "Press," "Release," "Long Press," and "Double Tap" actions on a single switch.

* *Example:* Tap for a *Rush* "Tom Sawyer" clean (JVM Clean Green + Chorus); Long Press to kick in the Mark VII's Mark IV mode for the solo.

* **The Desktop Editor:** Programming a JVM and a Mark VII via a tiny LED screen is a nightmare. Morningstar’s web editor allows you to drag-and-drop commands, name your presets (e.g., "7-String Heavy," "Satriani Lead"), and visualize your entire MIDI map.

### Analysis: Pros & Cons in Your Setup

| Feature | Morningstar MC8 Pro (Pros) | Cons / Trade-offs |
| --- | --- | --- |
| **Logic** | 16 MIDI channels; can control your amps and the Triple Delay/Dreamscape at once. | No built-in audio loops (you'll keep using your pedals as-is unless you add a Loop Switcher). |
| **Visuals** | Dual large LCD screens with customizable names for every switch. | The sleek, compact footprint might feel "small" if you prefer the massive stage presence of a Ground Control Pro. |
| **Connectivity** | USB-C, 5-Pin DIN, and 4 Omniports. | High technical ceiling; requires a solid understanding of CC/PC mapping to maximize. |

### Integration Strategy: Mesa VII + JVM410C

To get the most out of this, I suggest the following MIDI architecture:

* **Channel Mapping:** Set the Mark VII to MIDI Channel 1 and the JVM to Channel 2.
* **The "Lead" Preset:** Program one switch to send PC # for Mark VII Channel 3 (IIC+ mode) + CC for Graphic EQ "On" + PC # for your Marshall Delay.
* **The "Classical" Clean:** Even though you don't play Beethoven, your ear for that dynamic range means you'll appreciate the Mark VII's "Clean" mode on 90W for headroom. Program a "Scene" that engages the Dreamscape (in the loop) and switches both amps to their cleanest respective modes for a massive, wide-stereo spread.

### Critical Correction

While the JVM410C is a MIDI powerhouse, remember it **only accepts Program Change (PC) messages** for its 12 modes and master volumes/loop states. It does **not** respond to individual CC messages for "FX Loop On/Off" in real-time like the Mark VII does. You must save the JVM's state into a preset on the amp itself, then call that preset number from the MC8.
**Would you like me to detail the specific MIDI PC/CC mapping values for the Mark VII functions to help you start your template?**

---
