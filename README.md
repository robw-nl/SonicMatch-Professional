# SonicMatch Professional

A localized, hardware-agnostic psychoacoustic match engine designed to align the perceived loudness and tonal balance of modeler patches (Quad Cortex, Helix, Fractal, Kemper, etc) or software plugins. Or any other audio file for that matter.

Unlike standard LUFS meters, SonicMatch uses a 24 Bark-band critical hearing model to analyze why dense distortion presets push harder than dynamic clean tones at the same measured volume, outputting exact 1:1 physical dB corrections and parametric EQ match suggestions.

*This program is completely free to use, modify and distribute; but NOT if you intend to use my code for commercial gain.*

---

## SonicMatch Workflow

To guarantee perfect 1:1 matching without performance or input dynamics variance, use your modeler's built-in multi-channel USB interface:

1. **Capture the Dry Signal:** Connect your modeler to your DAW or recording application (e.g., Audacity, Reaper). Note: Ensure you use the exact same input connection and hardware gain settings for both recordings to guarantee an accurate match.
2. **Re-Amp Cleanly:** Route that exact same dry DI track back into the modeler simultaneously through:
   * **Preset A (Reference):** Your baseline target tone in the mix.
   * **Preset B (Target):** The tone you want to correct.
3. **Export:** Bounce both processed takes to your computer. Ensure **no normalization** is applied during DAW export.
4. **Analyze:** Drop the files into the interface, select your preferred target EQ block layout, and hit analyze.
5. **Correct:** Apply the calculated **Volume Correction** directly to the output block of Preset B, and dial the target EQ deviations into a Parametric EQ block.

---

## Architecture & Privacy
* **Zero Installation:** Runs natively inside any modern browser supporting the Web Audio API.
* **100% Local & Private:** Your audio files never leave your computer. All Fast Fourier Transforms (FFT) and psychoacoustic sorting are handled on your local CPU threads. No servers, no tracking, no analytics.

* ## Cost
* **No cost:** Sharing is caring, especially among musicians.
