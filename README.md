# CyVerse Timelapse Image Series

Extracted plant growth timelapses from the CyVerse Data Store for the [AstroBotany calibration database](https://dr-richard-barker.github.io/AstroBotany_calibration_image_sharing_and_analysis/).

## Series

See `catalog.json` for the complete list of extracted series with frame counts and metadata.

### Directory Structure

Each series folder contains:
- `timelapse.mp4` — H.264 encoded video at 30 fps, all-intra key frames for frame-accurate seeking
- `manifest.json` — Metadata: frame count, video size, codec, creation timestamp

### Usage

The AstroBotany app can ingest these series via the CyVerse source adapter by pointing to this repository's `catalog.json`:
- Source URL: `https://raw.githubusercontent.com/dr-richard-barker/timelapse-image-series/main/catalog.json`

### Source Data

Original images extracted from CyVerse Data Store iRODS:
- Path: `/iplant/home/dr_richard_barker/`
- Access: Authenticated iRODS (gocmd)

---
Generated: $(date)
