# MacNativeTV

MacNativeTV is an unofficial experimental macOS integration of EDCB, Amatsukaze, KonomiTV, and supported TV tuners. It is a community port and is not supported by the upstream projects.

> **Status: preparation build; not released.** This project has not been validated on a clean second Mac, and redistribution conditions for every bundled component still need a final review. Do not treat this repository as a stable recording solution.

## Downloads

When a release is published, download the `.tar.gz` archive and its `.sha256` checksum from the Releases page. The archive includes the setup guide. Verify the checksum before extracting it.

## Requirements

- macOS 15 or later (Intel or Apple silicon)
- DTV02A-5TS-P or PLEX PX-MLT5PE tuner, with its compatible powered case and antenna setup
- A valid B-CAS card and applicable viewing contract for encrypted broadcasts
- Internet access for first-time runtime setup

## Important

- Start with a short test recording and keep a separate backup of important recordings.
- Long-running recording, sleep recovery, all tuner combinations, and all channels are not guaranteed.
- KonomiTV is recommended in Chrome; browser-specific playback behavior may vary.
- Do not expose EDCB or KonomiTV ports directly to the public internet.
- Each bundled component keeps its own license and notices. See the archive's `LICENSE`, `licenses/`, and `source/` materials before redistribution.

## Upstream projects

- [EDCB](https://github.com/xtne6f/EDCB)
- [Amatsukaze](https://github.com/nekopanda/Amatsukaze)
- [KonomiTV](https://github.com/tsukumijima/KonomiTV)
- [px4_drv](https://github.com/tsukumijima/px4_drv)
