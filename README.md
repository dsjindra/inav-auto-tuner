# INAV Auto Tuner

**Free browser-based blackbox analyzer & PID suggester for INAV pilots**

Upload decoded INAV logs (CSV) → Get noise PSD, configurable step responses, posHold drift/wind estimates, XY/Z nav divergence warnings → Tiered PID gains (Safe / Medium / Aggressive) with copy-paste CLI diffs.  
Optimized for stable position hold, RTH, and autonomous flight. No install required!

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-donate-yellow?logo=buymeacoffee)](https://buymeacoffee.com/midilo)

## Features
- Drag-and-drop multi-log CSV upload with flexible header detection
- Gyro noise: Welch PSD, dominant frequencies, severity, peaks (20–500 Hz)
- Step response: Auto-suggest threshold, min duration filter, rise/overshoot/settling/RMS error
- Nav metrics: PosHold error (RMS/max/mean vs target), wind estimate, cross-track error
- Warnings: No aggressive maneuvers, missing nav columns, high drift/noise
- PID suggestions: Main (P/I/D/FF) + Nav (XY Pos/Vel, Z Pos/Vel) with full INAV CLI blocks
- Tiers: Safe (stability-focused), Medium (balanced), Aggressive (responsive)
- UI: Dark/light mode, zoomable charts (Chart.js), progress bar, session JSON save/load

## Quick Start
1. Decode your .bbl/.bfl log: `blackbox_decode yourlog.bbl > decoded.csv` (or use Blackbox Explorer)  
2. Open `index.html` in any browser  
3. Drag/drop CSV(s) → Adjust settings (auto threshold button!) → Run Analysis  
4. Review warnings/metrics → Generate PIDs → Copy CLI to INAV Configurator  
5. Test safely — start with Safe tier!

**Always bench-test and fly controlled. Suggestions are data-driven starting points only.**

## Screenshots

**Upload & Loaded Logs**  
![Upload interface with drag-drop and loaded log info](screenshots/INAV-Tuner-Upload-Dark.png?raw=true)

**Tune PIDs – Tiered Suggestions & CLI Diffs**  
![Safe/Medium/Aggressive PID cards with notes and copy buttons](screenshots/INAV-Tuner-TunePIDs.png?raw=true)

**Analysis – Warnings, Noise PSD, Step Response, Nav Metrics**  
![Warnings panel, gyro PSD table, step response table, nav RMS cards](screenshots/INAV-Tuner-Analysis-Warnings.png?raw=true)

**Navigation Position & Velocity Charts**  
![Pos X/Y/Z and Vel X/Y/Z traces with zoom](screenshots/INAV-Tuner-Navigation-Charts.png?raw=true)

**Attitude – Gyro vs Setpoint + PSD Spectrum**  
![Roll/Pitch/Yaw gyro vs setpoint overlays and noise spectrum](screenshots/INAV-Tuner-Attitude-Charts.png?raw=true)

## Support & Feedback
If this saves you tuning time or helps avoid crashes, consider [buying me a coffee ☕](https://buymeacoffee.com/midilo) — it funds hosting, new features (cloud upload?), and keeps it free!

Star ⭐ the repo if useful. Issues/PRs welcome for bugs, requests, or improvements.

#FPV #INAV #Blackbox #PIDTuning #DroneTuning #AutonomousFlight

Made with ❤️ by DJ (@CZ_Lab4)
