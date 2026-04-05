# My setup

*Hardware, software, and how it all fits together.*

## The devices

**CPAP**: Löwenstein prismaSMART max (since Jan 2025). APAP mode, pressure range 10–14 cmH₂O. Data on SD card, read daily.

**Pulse oximeter**: Wellue O2Ring. Measures SpO₂ and heart rate throughout the night, every second. Data transfer via Bluetooth (BLE) to a Raspberry Pi.

**Sleep stages**: Apple Watch. Provides Deep/Core/REM/Awake classification via Apple Health.

**Video**: REOLINK camera. Infrared night vision, RTSP stream, recorded via ffmpeg on the Raspberry Pi.

**Raspberry Pi**: The heart of overnight monitoring. Runs unattended, starts automatically each evening, captures BLE data from the O2Ring and video from the camera.

## The software

**OSCAR**: Open Source CPAP Analysis Reporter. My entry point into CPAP data analysis. Shows pressure, flow, events, leak — everything on the SD card.

**SDA5 (System-5)**: My own analysis system. Python, PostgreSQL, over 1,500 commits. Processes CPAP, O2Ring, Apple Health, and video data in an automated 12-step morning routine. Produces HTML night reports with narrative, correlations, and context.

Four previous system generations (S1–S4), each rebuilt from scratch. The first two with ChatGPT, the last two with Claude.

## The daily routine

Morning: SD card out of the CPAP, start the morning routine, wait 3–5 minutes. After that, a complete night report is ready — with AHI, SpO₂ statistics, sleep stages, respiratory rate, and a narrative assessment.

All data goes into a PostgreSQL database. Currently: over 619 nights, 21 months, without gaps.

---

*Back: [Tools](index.md)*
