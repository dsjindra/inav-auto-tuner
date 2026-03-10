# INAV Auto Tuner

A browser-based INAV blackbox analyzer that turns decoded flight logs into actionable PID and navigation tuning suggestions.

## Highlights
- Multi-log CSV ingestion with flexible header detection
- Gyro noise and PSD peak analysis
- Step-response detection with configurable threshold and minimum duration
- Navigation drift metrics (XY/Z RMS), poshold error, and wind estimate support
- Safe/Medium/Aggressive PID profile generation with CLI output
- Session export/import for repeat tuning workflows

## Usage
1. Open `index.html` in your browser.
2. Load decoded INAV logs (`.csv`).
3. Run analysis, review warnings/metrics, then generate PID variants.
4. Copy CLI commands into INAV Configurator and test safely.

## Notes
- Suggestions are starting points, not final values.
- Always bench-test and perform controlled test flights before full missions.
