# Current status — Magnetometer / Georadar

Updated: 2026-11-08

## K49E measurements
Sensor marking: K49E / 6Y071L; manufacturer not confirmed.

| Measurement | Result |
|---|---:|
| Supply voltage | 4.972 V |
| Output without nearby test magnet | 2.450 V |
| Output with magnet pole 1 | 4.300 V |
| Output with magnet pole 2 | 0.835 V |

Half-supply: 2.486 V. Difference from half-supply: -36 mV.
Changes relative to baseline: +1.850 V and -1.615 V. The response confirms functionality, not calibrated field sensitivity or geomagnetic measurement accuracy. “Without magnet” is not zero field.

## Current workflow
GitHub is the canonical location for project documentation. Local Linux/Windows work uses Git; mobile access can use GitHub or a configured Obsidian Git copy. AI tools do not necessarily share chat histories, so docs/AI is the handoff point.

## Next actions
1. Review MultiChannel_datalogger technical note `docs/AI_PODKLAD_DATALOGGER.md` from the separate local project; contents have not yet been supplied to this chat.
2. Measure K49E output drift for 10 minutes after warm-up, preferably with simultaneous supply-voltage logging.
3. Determine practical ADC architecture from measured noise, supply sensitivity, sampling rate and available datalogger hardware.
4. Characterize temperature drift, repeatability and variation among K49E units.

## Unresolved
Final ADC/controller selection, number and geometry of channels, reference sensor type, and manufacturer-specific K49E specifications.
