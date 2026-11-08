# Magnetometer / Georadar — Project context

Updated: 2026-11-08

## Purpose
Independent low-cost geophysical magnetometer project, with future georadar subsystem. Separate from the DY1703A audio-player project.

## Proposed architecture
- Modular magnetic sensor array, more than seven channels; exact count not yet fixed (8/12/16/24+ considered).
- Two spatially separated reference sensors (REF-A, REF-B); correction must be validated experimentally.
- External ADC for analog sensors, controller from ESP32 family, GPS, orientation/IMU, local SD recording, smartphone Wi-Fi UI.
- Electronics in KiCad; mechanics in FreeCAD/SolidWorks; processing in Python/QGIS.
- Preserve raw measurements separately from calibrated and derived data.

## Available hardware
- K49E linear Hall sensor, marking K49E / 6Y071L; manufacturer not confirmed.
- LSM303DLHC for orientation/motion assistance.
- Separate MultiChannel_datalogger project with ADS1256 experience; check actual hardware before reuse.

## Engineering principles
- Characterize one K49E channel before scaling the array.
- Keep assumptions separate from measured facts.
- Track sensor positions, calibration, temperature, supply voltage and timestamps.
- GitHub repository StePol/magnetometer-georadar is the canonical technical project record.
