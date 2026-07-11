# Sketch Recorder — hand-drawing data collection

A single-page drawing tool for collecting **part-labelled, stroke-order, pressure-recorded**
sketches of single still-life objects (apple / pear / ceramic jar) for a master's thesis on
a painter-like layered sketch-generation pipeline.

**Use it here:** open the GitHub Pages site for this repo in Safari/Chrome (iPad + Apple Pencil
recommended — pressure is recorded as stroke width). Fingers don't draw (palm rejection);
only the pencil (or mouse via the test toggle).

## How to draw (please follow — data is only comparable if we all do the same)

1. **Enter your name** in the *artist* box (top left) — once; it's remembered.
2. **One object per canvas**, upright, roughly centred, filling most of the canvas.
   - Viewpoint: classic still-life view — eye level or slightly above (a jar's mouth is a gently open ellipse).
   - Poses: straight or *mildly* leaning (up to ~20–30°). No lying-down or top views.
   - Vary shapes between drawings: fat / round / tall; simple (2 strokes) to detailed (6+).
3. Draw naturally, **vary your pen pressure** — it's recorded as line width.
4. **Tag your strokes**: after a few strokes, tap **Tag** → pick a chip (body / stem / mouth / neck / base…)
   or type your own words → optionally set the stroke kind:
   - `contour` = a final, correct line
   - `construction` = a guideline / scaffold line
   - `discard` = a line that came out wrong — **do not avoid these; never wish for an eraser.**
     Wrong lines and guidelines are part of the data. Use Undo only for real accidents (palm blips).
5. **Export** (top right) → *Download .json* (or *Copy to clipboard*) → send the file back to the
   dataset owner (WeChat / email). One file per drawing. Then tap **New** and draw the next one.

Rough target: ~20 drawings per object type per person.

## What gets recorded

Per stroke: drawing order, your label (free text), role (contour/construction/discard),
the full pen trajectory with per-point pressure (=width) and timestamps. Per file: object type,
artist name, canvas size. **Nothing is uploaded anywhere by the tool** — data stays on your
device until you send the exported file yourself.

## Files

- `index.html` — the whole tool (self-contained, no dependencies, works offline once loaded).
