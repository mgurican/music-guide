# 🔌 Hardware, Routing & Power Engineering

Return to [[Home]] | [[Tone Presets]]

---

## 🎧 1. Silent Headphone Signal Chain (Studio Grade)

```
[Guitar] -> [Pedalboard: TS808 / SD-1 / Spark / HyperGravity]
         -> [Amplifier Preamp Line Out (Mesa Mark VII Dry / JVM Silent Rec)]
         -> [Mooer Radar (Power Amp Sim OFF, York Audio IR ON)]
         -> [Rupert Neve Designs RNHP (TRS Balanced Line Input)]
         -> [Headphones]
```

### Key Engineering Notes:
* **Mesa Boogie Mark VII Dry Line Out:** Tapped directly after preamp before power tubes.
* **Marshall JVM 410C Silent Recording:** Disengages power section output while leaving Preamp and FX Loop fully operational.
* **Rupert Neve RNHP:** Discrete reference headphone amplifier providing maximum dynamic range and zero transient compression compared to built-in headphone jacks.

---

## 🎛️ 2. Boss EQ-200 Dual Signal Routing

* **Pre-Amp Routing (Channel A):** Placed before amp input. Use to cut frequencies below 160Hz before hitting high gain stages.
* **FX Loop Routing (Channel B):** Placed in Marshall JVM410C FX Loop. Use to shape post-distortion tone (boost 1.6kHz - 3.2kHz for lead cut).
* **Preset Control:** Connect Boss FS-6 / FS-7 foot switches to switch channels or step through presets.

---

## ⚡ 3. Power Supply Isolation & Safety

* **Ground Loops & Floating Potential:** Running analog drives (TS808, SD-1) on the same daisy chain as digital DSP units (Dreamscape, Mooer Radar) produces high-frequency ground noise and stray current on cable jacks.
* **Isolation Solution:** Use **Harley Benton PowerPlant ISO-12 Pro** with individually isolated transformer outputs.
* **18V Headroom:** TC Spark Mini strictly requires 9V. Supplying 18V will destroy it. Never supply 18V to 9V-only digital units.
