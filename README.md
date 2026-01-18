# Nishizumi IBT Overlay

Nishizumi IBT is a single-file Tkinter overlay that compares live iRacing telemetry to a
reference lap extracted from a local IBT file. It highlights throttle, brake, and speed
traces along with reference brake/lift/power cues to help you benchmark your driving.

> **Status:** This project is still **experimental**. Expect rough edges and evolving
> behavior as the overlay is refined.

## Features

- Live throttle/brake/speed traces against a reference lap.
- Reference event cues (brake, lift, power) derived from the IBT data.
- Configurable thresholds, colors, and overlay layout.
- Optional audible cue support on Windows.

## Requirements

- Windows with Python 3 installed.
- iRacing running with telemetry enabled.
- A local `.ibt` file containing a clean reference lap.
- Python packages:
  - `irsdk` (`pip install irsdk`)

## Usage

```bash
python nishizumi_ibt_overlay.py
```

When prompted, select a reference IBT file and start driving to see live comparisons.

## Project Layout

- `nishizumi_ibt_overlay.py` — The full overlay application.

## Notes

- The overlay assumes a reasonable track length from the IBT data; laps with missing
  telemetry may display incomplete reference traces.
- Because this is experimental, settings and UI layout may change.
