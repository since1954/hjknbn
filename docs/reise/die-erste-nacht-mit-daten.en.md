# The first night with data

*July 14, 2024. A pulse oximeter, a CPAP machine, and the beginning of something I hadn't seen coming.*

## The setup

The CPAP machine had been running for years: a Löwenstein Prisma Smart, APAP mode, pressure range 7–12 cmH₂O. What was missing was independent oxygen saturation measurement — because the device itself doesn't measure SpO₂.

I bought a Wellue O2Ring. A small ring that records oxygen saturation and heart rate on your finger throughout the night. Plus: OSCAR, the open-source software for reading CPAP data from the SD card.

On July 14, 2024, I recorded both simultaneously for the first time. Night 1 in the database.

## What the data showed

Average AHI in July 2024 was 4.29. Not bad. But the O2Ring told a different story: the ODI (Oxygen Desaturation Index) was around 21 — meaning 21 oxygen desaturations per hour, significantly more than the apnea events the CPAP counted.

The CPAP machine said: "Everything's under control." The O2Ring said: "Something else is happening that the device doesn't see."

## The config odyssey

What followed were four months of trial and error. Six different pressure configurations between July and October 2024 — from APAP to a fixed-pressure experiment (aborted after one night when AHI spiked to 327) to the first stable setting.

In September 2024 the monthly AHI reached 15.58 — a value that would have remained invisible without my own data collection. It would have drowned in the annual average at the next doctor's visit.

By October the AHI stabilized around 4. But the ODI stayed at 21, regardless of configuration. That was the first real insight: CPAP pressure controls the apneas, but the oxygen desaturations apparently have their own dynamic.

## What I didn't know yet

That this spreadsheet would turn into a full analysis system. That within 18 months I'd build four generations of software, together with an AI. That I'd eventually calculate respiratory rate directly from raw CPAP waveforms, synchronize sleep videos with physiology data, and simulate a closed-loop oxygen supplementation system.

On July 14, 2024, all I knew was: my CPAP machine isn't telling me the whole story. And I wanted to hear the rest.

---

*Next: [The device switch](der-geraetewechsel.md)*
