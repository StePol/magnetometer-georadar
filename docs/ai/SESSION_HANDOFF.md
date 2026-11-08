# Session handoff — Magnetometer / Georadar

Updated: 2026-11-08

## Where it started
Separate low-cost geophysical magnetometer/georadar project, with GitHub, KiCad, mechanical CAD, smartphone UI and expandable magnetic sensor array.

## Decisions locked
- Repository: `StePol/magnetometer-georadar`.
- Canonical project notes and AI handoff: `docs/ai/` in GitHub.
- Start by characterizing one K49E channel.
- Plan more than seven channels and two reference sensors, but do not freeze the array layout yet.
- Use an external ADC for serious analog measurements; selection remains open.
- Phone as monitoring/control UI; local storage of raw data.

## Measurements completed
K49E marked `K49E / 6Y071L`.
VCC 4.972 V; VOUT without nearby test magnet 2.450 V; pole 1 4.300 V; pole 2 0.835 V. Offset relative to VCC/2: -36 mV. Magnetic sensitivity, noise and long-term drift have not been calibrated.

## Unknowns and blockers
- Local technical file: `/home/stepol/Dokumenty/projekty/MultiChannel_datalogger/docs/AI_PODKLAD_DATALOGGER.md` needs to be read by a local agent or uploaded.
- K49E manufacturer and guaranteed characteristics unknown.
- ADC design and reference sensors not finalized.

## Exact next steps
1. Read `PROJECT_CONTEXT.md`, `CURRENT_STATUS.md` and this handoff.
2. Examine the MultiChannel_datalogger technical note and available ADS1256 hardware.
3. Measure K49E output and supply stability over time.
4. Update current status and decisions with verified results.
5. Commit and push; on another computer, pull before editing.

## Session handoff convention
Summarize starting context, locked decisions, completed tests, outstanding issues and the next concrete action. Separate verified measurements from proposals.
