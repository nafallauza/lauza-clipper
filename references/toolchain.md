# Toolchain and reference routing

## Production stack

| Tool | Job | Requirement |
| --- | --- | --- |
| Remotion + React/TypeScript | Composition, video, captions, shared frame clock | Primary engine |
| GSAP | Choreography | Optional per beat; pause and seek from the Remotion frame |
| Three.js | Depth, lights, 3D props | Use when the idea needs 3D |
| FFmpeg / ffprobe | Metadata, safe cuts, mixing, loudness, encoding checks | Required for media work |
| Facecammaxxing `fcm.py` | Tracking, cut-outs, check frames, effect rendering via `plan.json` | Preferred when provisioned and suitable |
| Verified word timestamps | Caption/illustration alignment to actual speech | Obtain or align when word accuracy is required |

Check actual installed dependencies and models before promising this pipeline.
Matching `remotion` and `@remotion/*` versions must stay pinned together.
`fcm.py track`, `check` and `render` require the upstream environment and its own
schema. This kit's template is a broader job contract, not a drop-in FCM plan.
Map its `effects` into an upstream-valid FCM plan and validate with `fcm.py check`.
Do not fabricate a tracker or claim matte/face effects ran when setup is absent.

Use Remotion Studio for preview when available. An offline SVG/FFmpeg fallback
can render simple vector scenes; disclose its limits and match fonts, frame
clock, tracking and offsets. Browser/network restrictions in the previous
Timothy session do not establish the capabilities of a future environment.

## Skills to use when available

- `remotion-best-practices`: route to the relevant Remotion guidance.
- `remotion-create`: composition setup; `remotion-markup`: layers/motion/editing.
- `remotion-captions`: captions; `remotion-multimedia`: media handling.
- `remotion-studio` and `remotion-render`: preview and export.
- `bang-motion`: cinematic/explainer direction; adapt timing to Remotion.
- `facecammaxxing`: tracking, behind-person layers and face-aware effects.
- `claude-animation`: optional illustrated B-roll; not the main talking-head editor.

Use installed skills by their actual paths. Do not assume these dependencies
are bundled with this kit, and do not copy entire third-party skills unnecessarily.

## User-supplied learning references

- `KITAB EDITING PAKE CLAUDE.pdf`: Nadiv's editing workflow and audio/subtitle SOP.
- `17 Efek Video AI by Kadafi Devayana.pdf`: effects selected by spoken meaning.
- `facecammaxxing-main.zip`: the user's face-aware effect pipeline archive.
- `claude-animation-skill-main.zip`: hand-drawn/code animation reference archive;
  its README identifies `https://github.com/buildwithhanif/claude-animation-skill`.

These files are external references, not included or installed by this kit.
The kit contains original workflow notes and licensed Montserrat font assets;
it does not bundle source podcast footage, music from others, PDFs or the archives.
