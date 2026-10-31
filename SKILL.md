---
name: lauza-clipper
description: Plan and edit Lauza podcast clips with the established yellow/gray/black visual identity, centered speaker, captions, explanatory animation, and synchronized audio. Use for Lauza clipper tasks; apply Vordev branding only when explicitly requested.
---

# Lauza podcast clipper

Work in the user's existing Remotion workspace. Keep each job in
`brands/lauza/<job>`, global components in `src/shared`, browser media in
`public/brands/lauza/<job>`, and rendered artifacts in `out/<job>`.
Use existing project registration; preserve unrelated user changes.

## Start with the actual brief

Read `brand.json` and [visual direction](references/visual.md) for this brand.
Use [toolchain](references/toolchain.md) for setup, skill routing and reference sources.
Use `templates/plan.json` as an example job contract, not a working renderer.

The palette is approved. Typography is a proposal; Fira Sans was rejected.
Preview Montserrat before locking the font for a new job. Existing user font
choices override this proposal. Keep Vordev's identity separate.

## Plan before editing

Inspect the clip's audio, dimensions, rotation, timebase and camera cuts.
Preserve source A/V timestamps when converting 29.97 fps to 30 fps; do not
change speech speed just to meet a frame rate. Center the speaker per shot;
smooth face tracking within shots and switch tracking immediately at cuts.

Transcribe when necessary, or use the user's transcript. Validate cue order,
overlaps, missing words, punctuation, actual numbers and word timestamps.
Phrase windows are not word timestamps. Never silently average overlaps or
interpolate word starts and then label the result accurately synchronized.
If only phrase timings exist, align them to the real recording or label the
word timing approximate and make a short review preview before full production.

Deliver a timecoded beat plan: quote, visual, purpose, assets, caption and SFX.
Wait for the requested plan approval; if execution was already authorized,
continue within that approval. Use one main visual idea per sentence and quiet
footage where expression carries the point. Animation density follows the clip;
33.87 seconds from an earlier test is not a universal quota.

## Synchronization comes before polish

Produce a clean preview with centered speaker and original speech. Check lip
sync near the start, middle, end and camera cuts at real speed. Separate actual
lip-sync, subtitle timing, illustration timing and playback latency issues.
Waveform correlation can establish whether an export added audio delay; it
does not prove lips were synchronized in the source. Mouth-energy correlation
and synthetic speech matching are diagnostic estimates, not lip-sync ground truth.
If direct listening/viewing is unavailable, disclose that verification limit;
do not certify lip sync from proxy scores or successful encoding alone.

Default `videoDelayFrames` to zero. Apply a source-specific correction only
with evidence of its direction and magnitude. Keep speech intact, retime face
tracking consistently, then verify the encoded result. Do not reuse the
unvalidated 100 ms Timothy correction for other clips or call it confirmed.
Timothy v1–v3 are design experiments; the user still reported sync problems.

After that check, add 2–5-word captions, highlight active words, build the
approved animation beats, and place SFX on the same frame clock. Verify timed
words and important reveals against audible speech, not just caption metadata.

## Delivery standards

Output 1080×1920, 9:16, 30 fps. Keep face and essential text unobstructed;
avoid the bottom 300 px and lower-right platform UI. Use the conservative
bounds in `brand.json` where framing allows.

Remove fillers or pauses over 0.4 s only at verified quiet boundaries; inspect
both sides of each cut. Preserve intentional delivery and avoid clipped syllables.
Voice bus −16 LUFS; music about 11 LU below voice with speech ducking;
final master −14 LUFS and true peak at or below −1.5 dBTP. Measure the encoded file.

Use frame-driven Remotion timing. GSAP must be paused/seeked from the frame;
Three.js must follow that same clock. Choose HTML/SVG for straightforward
illustration; use Three.js when depth/material adds meaning. Inspect contact
sheets and fast motion, run type checks, then review lip sync at real speed.
When render/export is requested, provide the MP4 path and material limitations.
Do not label an export final merely because encoding and type checks pass.
