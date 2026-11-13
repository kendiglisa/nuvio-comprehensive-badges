# Nuvio Comprehensive Badges

A single Fusion badge configuration for Nuvio.

## Import URL

`https://raw.githubusercontent.com/kendiglisa/nuvio-comprehensive-badges/main/badges.json`

Import this one URL in Nuvio → Settings → Streams → Fusion Badge URLs.

## What's included

- 167 original release, resolution, HDR, codec, audio, edition, service, container, subtitle, 3D, frame-rate and disc-structure filters.
- 83 language badges, each with its own group ID so multiple language badges can appear together.
- Dual Audio, Multi Audio and Original Audio badges in a separate audio-mode group.
- 99 groups and 253 total filters.

## Image hosting

- The original 167 badge PNGs are stored in this repository's root.
- The 83 language badges and 3 audio-mode badges are served as PNG images by Shields.io's raster service. This avoids requiring 86 additional files in the repository.

## Language detection limitations

Language badges match explicit language names or ISO-639-2/3 codes in the stream title returned by an add-on. They cannot inspect a media file's audio tracks. A title containing only `DUAL AUDIO` can show the Dual Audio badge but cannot reveal which two languages are present.

Two-letter language codes are intentionally not matched on their own to reduce false positives. Use full language names or three-letter codes in stream names where possible.

## Notes

Nuvio displays at most one matching badge per group. Each language therefore has a distinct group ID; this allows titles such as `Hindi English Dual Audio` to show Hindi, English and Dual Audio badges together.
