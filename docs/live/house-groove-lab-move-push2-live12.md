# House groove lab: Move, Push 2 and Live 12

> Checked: 18 November 2026. **Original exercises** informed by publicly available Production Music Live (PML) teaching articles, not transcriptions of PML courses or recreated factory patterns. Controls checked against the provided Ableton Move and Live 12 manuals. Push 2 here means **Push 2 controlling Live**, not standalone Push 3.

## Learning path

1. **Foundation:** four-on-the-floor kick, backbeat clap, offbeat hat.
2. **Bounce:** bass syncopation and deliberate note lengths.
3. **Expression:** velocity accents, swing, and restrained note nudges.
4. **Conversation:** toms, shakers and percussion answering (not doubling) the central rhythm.
5. **Arrangement:** small two-bar changes and occasional transitions.

PML's [four-level groove walkthrough](https://www.productionmusiclive.com/blogs/news/how-to-make-a-groove-in-4-levels) provides a useful general progression. Its [humanising drums](https://www.productionmusiclive.com/blogs/news/humanizing-midi-drums) article emphasises swing, velocity and plausible performance. The [bassline patterns](https://www.productionmusiclive.com/blogs/news/bassline-patterns) article highlights sixteenth-note placement and note length. PML's [three groove setups](https://www.productionmusiclive.com/blogs/news/how-to-make-groovy-drums) additionally illustrate bell-led, tom-led and clap-led arrangements, with deliberate space between complementary parts. These are **source observations**; patterns below are our own. PML examples and equipment-specific settings are not requirements for these exercises.

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

`X` = primary accent; `x` = quieter hit; `.` = rest. The hat/percussion rows are independent **sounds within one Drum Rack**, not separate Move tracks. The table represents MIDI trigger positions, not the durations of the resulting audio tails. If the open and closed hats overlap awkwardly, shorten the open-hat sample or use a choke group where available. Try 124 BPM in 4/4, but adjust to taste. For variation, omit a percussion hit in bar 2 and place a quiet pickup on step 16.

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

This **complementary variation** avoids *new* bass attacks on the kick's steps 1/5/9/13; some bass notes may still sustain across those steps (for example bar 1 step 4 into beat 2 if a sound has a long release). Adjust instrument release and note length by ear. Compare it with the older, more downbeat-oriented [bass exercise](../move/groovy-bass-lines.md).

## Translate the same musical experiment

| Operation | Move (standalone) | Push 2 controlling Live 12 | Live 12 mouse/keyboard |
| --- | --- | --- | --- |
| Load drums | Select a Drums Track Preset; 16 left pads are Drum Rack voices | Select a Drum Rack track; enter drum layout | Load Drum Rack on a MIDI track |
| Add drum hits | Choose a sample pad, tap step buttons 1–16; navigate bars using arrows | Tap the drum pad to focus its voice; tap sequencer pads | Add notes in the MIDI Note Editor |
| Add bass | Use a separate melodic track; set key/scale, sequence notes | Use a separate melodic instrument track and melodic step sequencer | Draw MIDI bass notes in a clip |
| Change dynamics | Hold step and turn Volume encoder | 16 Velocities mode sets the velocity of newly entered/played drum hits; hold an existing sequencer step to edit its velocity with an encoder | Edit MIDI note velocities |
| Offset timing | Hold step and use left/right arrows; Shift allows finer increments | Note-specific micro-timing controls (see manual §36.14.4) | Nudge notes in MIDI editor |
| Swing | Shift + Step 7 opens **Set-wide** triplet-sixteenth swing amount | Set clip grooves in Live's Groove Pool (via Live's interface), not a standalone Push 2 groove knob | Choose and adjust Live clip groove settings |
| Extend groove | Duplicate clip, modify second bar; max four Move tracks | Duplicate clips or build variations in Session | Duplicate/edit clips in either view |

**Move-specific warning:** The Move Groove amount is not a generic percentage of a Live Groove Pool preset. At 0% no groove is applied; 100% corresponds to triplet sixteenth-note swing; values above 100% exaggerate this timing. Groove is applied to the entire Move Set (Move manual §10.2). No independent per-clip Groove Pool controls are assumed on Move.

**Push 2-specific warning:** Push 2 is a controller for Live, so do not confuse its sequencing buttons with Move's dedicated 16 step buttons. In its drum sequencing layout, the 8×8 pad grid includes dedicated drum voice, step and loop controls; the assignment depends on layout. Consult Live manual §36.3 rather than copying Move key combinations.

**Clip-groove scope:** In Live a groove assigned to a MIDI clip affects the clip's MIDI notes, including all voices in a single Drum Rack clip. You cannot independently groove just the hats *within that same clip* using a separate Groove Pool assignment. To leave the kick straight, split hats/percussion onto another clip/track, use manual per-note timing edits, or keep all voices under one shared groove and evaluate the result. Move has only the Set-wide Groove control, but individual notes can be nudged.

## Move exercise (four tracks, not four sounds)

- **Track 1 Drums:** kick, clap, both hats and percussion all in a single 16-pad Drum Rack. Start with the five rows above.
- **Track 2 Bass:** the two-bar A-minor answer above.
- **Track 3 Chords:** sparse offbeat stabs; leave long gaps.
- **Track 4 Hook:** a short melodic call, or leave unused while testing groove.

After entering the notes: turn Groove to 0%, compare against 15%, then 30% as **listening experiments**, not recommended universal values. Adjust closed hats to alternate quieter and stronger notes. For individual timing, hold the relevant step and press left/right; with Shift the nudge increment is 1% of a step (Move manual §11.4). At a 1/16 grid and 124 BPM, a step lasts about 121 ms, so the fine increment is roughly 1.2 ms. Avoid confusing 1% of a step with 1% of a bar. If the kick and bass collide, shorten bass durations before adding processing.

## Push 2 exercise (Live 12)

1. Load a Drum Rack onto a Live MIDI track and select it from Push 2. Work in the drum step sequencer (Live manual §36.3.5, printed pp. 924–926).
2. Focus each drum voice and enter the first bar's steps. By default drum steps are sixteenths; Scene/Grid changes step size. Keep the kick and clap strong, hats lower.
3. Use **16 Velocities** (Live manual §36.3.2) to enter or play drum hits at selected velocities. For existing steps, **hold a sequencer step and adjust the corresponding velocity encoder** (see §36.14.4). You can also adjust note nudge and length from this step view. Do not assume Move's `hold step + Volume` shortcut exists on Push 2.
4. Add the two-bar bass on another instrument track. Use the melodic sequencer (Live manual §36.6) to input the notes and make duration variations.
5. In Live, try a groove on the **bass clip** first. To groove hats without the kick, separate hats into a different MIDI clip/track or manually nudge individual hat notes in the existing Drum Rack clip. Adjust the groove settings in Live's interface and compare at similar loudness.
6. Make a two-bar clip variation by adding a quiet percussion answer in the second bar. On Push 2 you can copy clips and work with Session View; use the Live interface for advanced groove choices when easier.

**Push 2 pad copying caveat:** the manual's drum-pad Duplicate operation **replaces the destination pad's devices/sound, while preserving any existing MIDI notes for that destination pad** (Live manual §36.3.4.1, printed pp. 922–923). This does not duplicate the source pad's MIDI pattern. Copying a clip or its notes is a separate operation.

## Live 12 extension

Experiment in this order so cause and effect remain audible:

1. Straight notes, equal velocity, no groove.
2. Add dynamic accents to hats only.
3. Shorten/extend only the bass notes.
4. Apply a groove to the bass clip first. If you want separately grooved hats with a straight kick, separate the hat notes onto another track or manually adjust their timing inside the Drum Rack clip.
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

**Free PML resources (web-verified on 18 November 2026; first three links below were located through indexed search content where direct page fetching failed):**
- [How to Make a Groove in 4 Levels: Basic to Pro](https://www.productionmusiclive.com/blogs/news/how-to-make-a-groove-in-4-levels)
- [Humanizing MIDI Drums in Ableton (3 Essential Factors)](https://www.productionmusiclive.com/blogs/news/humanizing-midi-drums)
- [We Rebuilt 17 Famous Bassline Patterns](https://www.productionmusiclive.com/blogs/news/bassline-patterns)
- [How to Make Groovy, Banging Drums: 3 Complete Setups](https://www.productionmusiclive.com/blogs/news/how-to-make-groovy-drums)
- [Drum Groove Techniques with Ableton Live](https://www.productionmusiclive.com/blogs/news/groove)

**Official manuals (user-provided copies):**
- Ableton Move manual: §9.5 sequencing, §10.2 groove, §11.1 velocity, §11.4 note nudge, §11.8 copying, §17 Session.
- Ableton Live 12 manual: ch. 10 Editing MIDI, ch. 14 Using Grooves, ch. 25 Drum Racks, ch. 36 Using Push 2 (especially §§36.3.2, 36.3.5, 36.6, 36.14.4).
- [Live manual online](https://www.ableton.com/en/live-manual/12/) · [Move manual online](https://www.ableton.com/en/move/manual/).

**Verification status:** Manual control behaviour was checked against the provided Move and Live 12 PDF manuals (including Push 2 §§36.3.2, 36.3.4.1, 36.3.5 and 36.14.4). PML's 4-level, bassline and 3-setup articles were checked via indexed public page content; humanising-drums and Drum Groove Techniques pages were directly inspected. No paid PML material was accessed or copied. Exercises remain **musical proposals, not audition-tested** on physical Move or Push 2. Record Live version, Move firmware, actual pad layout, instrument/sound preset and subjective listening notes after testing.
