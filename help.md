![MIDEO logo](og-image.jpg)

# MIDEO

**Video-driven MIDI automation for creative sound design.**

Turn any video into a MIDI controller. MIDEO extracts color data from video frames and translates RGB values into MIDI CC messages in real-time. Perfect for automating parameters in your DAW with visual content.

## <i class="bi bi-palette"></i> What It Does

Place cursors anywhere on a playing video. Each cursor samples the color beneath it and outputs three MIDI CC values (RGB channels, 0-127). Connect to Ableton, Logic, Bitwig, or any MIDI-capable software to automate filters, effects, or any parameter you can imagine.

**Core features:**
- Real-time color sampling with multiple cursor positioning
- Standard MIDI CC output (compatible with all DAWs)
- DAW-style controls: mute, solo, enable per channel
- Touch and desktop support with drag positioning
- 100% offline processing

---

## <i class="bi bi-gear-fill"></i> Setup

### MIDI Bus Configuration

Before anything else, you need a virtual MIDI bus so your DAW can receive MIDEO's output.

**macOS**  
Open Audio MIDI Setup → Window → Show MIDI Studio → Double-click IAC Driver → Check "Device is online"

**Windows**  
Download [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html), create a virtual port

**Linux**  
Use ALSA (`modprobe snd-virmidi`) or JACK MIDI

### Getting Started

1. **Load your video** - Drag & drop or click to browse (MP4, WebM, MOV, AVI, MKV)
2. **Enable cursor overlay** - Click the three dots button in the control bar
3. **Place cursors** - Click anywhere on the video to start sampling
4. **Configure channels** - Adjust CC assignments, channels, and controls
5. **Connect your DAW** - Select the virtual MIDI bus as input
6. **Map parameters** - Use your DAW's MIDI learn to connect color data to sound

---

## <i class="bi bi-sliders"></i> Usage

### <i class="bi bi-cursor"></i> Working with Cursors

**Creating:** Click anywhere on the video to place a sampling cursor  
**Moving:** Hover briefly to enable drag mode, then reposition as needed  
**Layering:** Long hover makes a cursor transparent for placing others behind it  
**Touch:** Works natively on touch devices with immediate drag capability

### <i class="bi bi-music-note"></i> MIDI Mapping Workflow

For precise parameter mapping in your DAW:

1. **Solo the target CC** - Isolates that signal for clean mapping
2. **Enter MIDI learn mode** - In your DAW, select the parameter to control  
3. **Start video playback** - Color changes trigger MIDI CC output
4. **Confirm mapping** - Your DAW establishes the connection
5. **Set parameter range** - Adjust min/max values to taste
6. **Repeat or finish** - Map more CCs or exit learn mode

Pro tip: Choose high-contrast video areas for more dramatic automation curves.

### <i class="bi bi-sliders2"></i> Channel Controls

Each cursor outputs three channels (RGB) with individual controls:

| Control | Function |
|---------|----------|
| **CC Number** | MIDI controller assignment (auto-assigned, manually adjustable) |
| **MIDI Channel** | Output channel (1-16) |
| **Mute/Solo** | DAW-style channel isolation |
| **Enable** | Master on/off per channel |
| **Root Point** | Progress bar direction (left-to-right or right-to-left) |

---

## <i class="bi bi-lightbulb"></i> Creative Applications

**Music Videos**  
Sample beat-synchronized color changes for rhythmic filter automation

**Abstract Visuals**  
Use smooth color gradients for evolving ambient textures and pads

**Performance Content**  
Map stage lighting changes to reverb, delay, or spatial effects

**Motion Graphics**  
Turn animated elements into precise automation curves for synthesis parameters

### Example Session

Load a music video with strong visual elements, then place cursors strategically:
- **Lead visuals** → Filter cutoff frequency
- **Background colors** → Reverb send amount
- **Text/graphics** → Distortion drive level
- **Lighting changes** → Delay feedback

Record the MIDI output while the video plays to capture your automation as editable CC data.

---

## <i class="bi bi-question-circle"></i> Troubleshooting

**No MIDI output detected?**  
Verify your virtual MIDI bus is active and selected as input in your DAW.

**Cursor dragging not working?**  
Desktop: Hover briefly to enable drag mode. Touch: Should work immediately.

**Video won't load?**  
Check format compatibility. MP4 works best across all platforms.

**Performance issues?**  
Reduce the number of active cursors or lower video resolution.

---

*Berlin 2026 | [cafe del cadence](https://cafedelcadence.bandcamp.com)*
