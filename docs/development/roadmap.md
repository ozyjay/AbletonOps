# Development roadmap

Checked 1 November 2026. This is a plan; no SDK or runnable project has been installed.

## Development routes

| Route | Intended work | Boundary |
| --- | --- | --- |
| Live Extensions SDK | Generate or transform MIDI clips and automate Set edits | Live 12 Suite Beta 12.4.5+ per Ableton; not Standard, Intro or Lite |
| Max for Live | Explore sequencers and continuous MIDI/audio devices | Separate from the Extensions SDK; confirm installed Live/Max licensing before work |
| Control surfaces | Investigate controller mapping and MIDI Remote Script integration | Research current supported interfaces before choosing an implementation |
| Move integrations | External MIDI and supported preset/Set transfer | Do not assume Live SDKs execute on Move |

The official [Extensions page](https://www.ableton.com/en/live/extensions/) and [FAQ](https://help.ableton.com/hc/en-us/articles/27303428331420-Ableton-Extensions-FAQ) currently require Suite Beta 12.4.5 or later. The FAQ lists Node.js 24.16.0 LTS or higher for development. Recheck these changing requirements when starting. The [SDK entry page](https://ableton.github.io/extensions-sdk/) directs users to the beta program for the SDK and documentation.

Extensions perform discrete operations on a Set; the FAQ excludes continuous real-time audio/MIDI processing, device-chain instruments and timing-critical playback work. It points to Max for Live for performance-oriented devices. This distinction matters when choosing where a groove generator belongs.

## Milestones

1. **Knowledge foundation:** complete an on-device kit inventory, pad maps and repeatable listening comparisons. Keep source dates with every version-sensitive claim.
2. **Standalone groove model:** design a deterministic two-bar pattern representation with tempo, pad mapping, velocity, swing and a reproducible random seed. Prototype under `sdk/experiments/`; keep demonstration patterns under `examples/`.
3. **MIDI export experiment:** generate a standard MIDI file for Live and verify duration, note mapping and velocity by importing it. Test timing bounds, reproducibility and malformed input. Do not claim direct Move MIDI-file import without a separately verified supported route.
4. **Live Extension:** after checking Suite Beta access and SDK terms, adapt the pattern model to create or modify a selected clip. Work in a disposable Set and verify musical output, undo behavior and clip boundaries.
5. **Interactive device or controller:** choose Max for Live for continuous processing, or research controller integration under `sdk/control-surface/`. Document version dependencies before implementation.
6. **Move handoff:** audition the musical idea on Move through supported MIDI or compatible content transfer. Validate the actual route and hardware behavior before documenting it as supported.

Move's [manual](https://www.ableton.com/en/move/manual/) documents MIDI and Control Live Mode. Neither it nor the linked Live SDK documentation establishes a public native Move SDK. Community modifications should be documented separately from Ableton-supported interfaces.
