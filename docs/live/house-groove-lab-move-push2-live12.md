# House groove lab: Move, Push 2 and Live 12

> Checked: 18 November 2026. **Original exercises** informed by publicly available Production Music Live (PML) teaching articles, not transcriptions of PML courses or recreated factory patterns. Controls checked against the provided Ableton Move and Live 12 manuals. Push 2 here means **Push 2 controlling Live**, not standalone Push 3.

## Learning path

1. **Foundation:** four-on-the-floor kick, backbeat clap, offbeat hat.
2. **Bounce:** bass syncopation and deliberate note lengths.
3. **Expression:** velocity accents, swing, and restrained note nudges.
4. **Conversation:** toms, shakers and percussion answering (not doubling) the central rhythm.
5. **Arrangement:** small two-bar changes and occasional transitions.

PML's [four-level groove walkthrough](https://www.productionmusiclive.com/blogs/news/how-to-make-a-groove-in-4-levels) provides a useful general progression. Its [humanising drums](https://www.productionmusiclive.com/blogs/news/humanizing-midi-drums) article emphasises swing, velocity and plausible performance. The [bassline patterns](https://www.productionmusiclive.com/blogs/news/bassline-patterns) article highlights sixteenth-note placement and note length. These are **source observations**; patterns below are our own.

## Portable 16-step notation

Each bar has four beats, with four sixteenth steps per beat:

```text
Beat:       1               2               3               4
Step:       01 02 03 04 | 05 06 07 08 | 09 10 11 12 | 13 14 15 16
Kick:        X  .  .  . |  X  .  .  . |  X  .  .  . |  X  .  .  .
Clap:        .  .  .  . |  X  .  .  . |  .  .  .  . |  X  .  .  .
Open hat:    .  .  X  . |  .  .  X  . |  .  .  X  . |  .  .  X  .
Closed hat:  .  x  .  x |  .  x  .  x |  .  x  .  x |  .  x  .  x
Percussion:  .  .  .  x |  .  .  .  . |  .  x  .  . |  .  .  x  .
```

`X` = primary accent; `x` = quieter hit; `.` = rest. The hat/percussion rows are independent **sounds within one Drum Rack**, not separate Move tracks. Try tempo 124 BPM and 4/4, but adjust to taste.

### Bass answer: two bars

Use a short, rounded bass sound; start with A minor. Entries below indicate start positions; note duration is in sixteenth steps. Rest means **no new attack**, not necessarily silence if the previous note sustains.

| Bar | Step | Pitch | Duration | Velocity | Function |
| --- | ---: | --- | ---: | ---: | --- |
| 1 | 2 | A1 | 1 | 96 | After-kick answer |
| 1 | 4 | A1 | 1 | 73 | Pickup |
| 1 | 7 | E2 | 1 | 81 | Offbeat fifth |
| 1 | 10 | A1 | 2 | 99 | Longer low phrase |
| 1 | 15 | G2 | 1 | 69 | Turnaround |
| 2 | 2 | A1 | 1 | 95 | Repeat hook |
| 2 | 4 | A1 | 1 | 72 | Pickup |
| 2 | 7 | E2 | 1 | 80 | Familiar answer |
| 2 | 10 | A1 | 2 | 98 | Sustained weight |
| 2 | 14 | C2 | 1 | 78 | Small variation |
| 2 | 16 | A1 | 1 | 86 | Return pickup |

This **complementary variation** leaves the quarter-note kick attacks at steps 1/5/9/13 predominantly free. Compare it with the older, more downbeat-oriented [bass exercise](../move/groovy-bass-lines.md).

## Translate the same musical experiment

| Operation | Move (standalone) | Push 2 controlling Live 12 | Live 12 mouse/keyboard |
| --- | --- | --- | --- |
| Load drums | Select a Drums Track Preset; 16 left pads are Drum Rack voices | Select a Drum Rack track; enter drum layout | Load Drum Rack on a MIDI track |
| Add drum hits | Choose a sample pad, tap step buttons 1–16; navigate bars using arrows | Tap the drum pad to focus its voice; tap sequencer pads | Add notes in the MIDI Note Editor |
| Add bass | Use a separate melodic track; set key/scale, sequence notes | Use a separate melodic instrument track and melodic step sequencer | Draw MIDI bass notes in a clip |
| Change dynamics | Hold step and turn Volume encoder | Use 16 Velocities mode or note-specific sequencing controls | Edit note velocities |
| Offset timing | Hold step and use left/right arrows; Shift allows finer increments | Note-specific micro-timing controls (see manual §36.14.4) | Nudge notes in MIDI editor |
| Swing | Shift + Step 7 applies a triplet 16th swing **Set-wide** | Apply grooves to clips in Live's Groove Pool (not a Push 2 standalone setting) | Choose and adjust Groove Pool clip grooves |
| Extend groove | Duplicate clip, modify second bar; max four Move tracks | Duplicate clips or build variations in Session | Duplicate/edit clips in either view |

**Move-specific warning:** The Move Groove amount is not a generic percentage of a Live Groove Pool preset. At 0% no groove is applied; 100% corresponds to triplet sixteenth-note swing; values above 100% exaggerate this timing. Groove is applied to the entire Move Set (Move manual §10.2). No independent per-clip Groove Pool controls are assumed on Move.

**Push 2-specific warning:** Push 2 is a controller for Live, so do not confuse its sequencing buttons with Move's dedicated 16 step buttons. Consult the relevant Push 2 layout in the Live manual rather than copying Move key combinations.

## Move exercise (four tracks, not four sounds)

- **Track 1 Drums:** kick, clap, both hats and percussion all in a single 16-pad Drum Rack. Start with the five rows above.
- **Track 2 Bass:** the two-bar A-minor answer above.
- **Track 3 Chords:** sparse offbeat stabs; leave long gaps.
- **Track 4 Hook:** a short melodic call, or leave unused while testing groove.

After entering the notes: turn Groove to 0%, compare against 15%, then 30% as **listening experiments**, not recommended universal values. Adjust closed hats to alternate quieter and stronger notes. For individual timing, hold the relevant step and press left/right; with Shift the nudge is 1% of a step (Move manual §11.4). If the kick and bass collide, shorten bass durations before adding processing.

## Push 2 exercise (Live 12)

1. Load a Drum Rack onto a Live MIDI track and select it from Push 2. Work in the drum step sequencer (Live manual §36.3.5, printed pp. 924–926).
2. Focus each drum voice and enter the first bar's steps. By default drum steps are sixteenths; Scene/Grid changes step size. Keep the kick and clap strong, hats lower.
3. Use **16 Velocities** (Live manual §36.3.2) for expressive replay, or use note-specific parameter editing for programmed steps. Do not assume Move's `hold step + Volume` shortcut exists on Push 2.
4. Add the two-bar bass on another instrument track. Use the melodic sequencer (Live manual §36.6) to input the notes and make duration variations.
5. In Live, assign a groove to the bass or hats (not necessarily to the kick) using Clip Groove / Groove Pool; adjust the chosen groove's settings and compare at identical volume.
6. Make a two-bar clip variation by adding a quiet percussion answer in the second bar. On Push 2 you can copy clips and work with Session View; use the Live interface for advanced groove choices when easier.

**Push 2 pad copying caveat:** the manual's drum-pad Duplicate operation copies the destination sound/device chain but **does not copy its MIDI notes** (Live manual, printed p. 923). Copying a clip or notes is a separate operation.

## Live 12 extension

Experiment in this order so cause and effect remain audible:

1. Straight notes, equal velocity, no groove.
2. Add dynamic accents to hats only.
3. Shorten/extend only the bass notes.
4. Apply a groove to hats/bass, leaving kick straight initially.
5. Fine-adjust selected note positions; try restrained percussive timing differences rather than moving every hit.
6. Add tom or percussion answering gaps rather than filling all sixteenths.
7. Make a second bar with one quiet pickup; compare the repeated one-bar pattern.

For more flexibility, see Live manual **Using Grooves** (chapter 14), **Editing MIDI** (chapter 10), **Using Push 2** (chapter 36), and **Drum Racks** (chapter 25).

## Listening checklist

- Does the groove still work with the kick + bass + clap only?
- Are the quieter hats actually quieter, not simply different samples?
- Does the bass sound tighter when some notes end before the next kick?
- Is the swing helping, or blurring the low-end attacks?
- Do the percussion additions leave breathing room?
- Is the second-bar variation recognisable without becoming a fill every bar?

## Sources and scope

**Free PML resources (read on 18 November 2026):**
- [How to Make a Groove in 4 Levels: Basic to Pro](https://www.productionmusiclive.com/blogs/news/how-to-make-a-groove-in-4-levels)
- [Humanizing MIDI Drums in Ableton (3 Essential Factors)](https://www.productionmusiclive.com/blogs/news/humanizing-midi-drums)
- [We Rebuilt 17 Famous Bassline Patterns](https://www.productionmusiclive.com/blogs/news/bassline-patterns)
- [How to Make Groovy, Banging Drums: 3 Complete Setups](https://www.productionmusiclive.com/blogs/news/how-to-make-groovy-drums)
- [Drum Groove Techniques with Ableton Live](https://www.productionmusiclive.com/blogs/news/groove)

**Official manuals (user-provided copies):**
- Ableton Move manual: §9.5 sequencing, §10.2 groove, §11.1 velocity, §11.4 note nudge, §11.8 copying, §17 Session.
- Ableton Live 12 manual: ch. 10 Editing MIDI, ch. 14 Using Grooves, ch. 25 Drum Racks, ch. 36 Using Push 2 (especially §§36.3.2, 36.3.5, 36.6, 36.14.4).
- [Live manual online](https://www.ableton.com/en/live-manual/12/) · [Move manual online](https://www.ableton.com/en/move/manual/).

**Verification status:** Source pages and manual descriptions reviewed; exercises are *not yet audition-tested* on physical Move or Push 2. Record Live version, Move firmware, actual pad layout and sound preset after testing. No paid PML content accessed or copied.
