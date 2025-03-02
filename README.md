# Personal MPV Configuration

This repository contains my personal configuration for [mpv](https://mpv.io/), a free, open-source, and cross-platform media player.

## Overview

This configuration is optimized for high-quality video playback with a modern UI using the uosc script. It includes:

- Hardware-accelerated video playback
- High-quality video scaling and processing
- Customized UI with uosc (modern UI replacement)
- Thumbnail previews on the timeline
- Optimized subtitle rendering
- Convenient keyboard shortcuts

## Features

### Video

- Hardware acceleration with `hwdec=auto-safe`
- High-quality scaling with `ewa_lanczossharp` for upscaling
- Debanding for smoother gradients
- Motion interpolation for smoother playback
- Display-based video sync

### Audio

- Audio language preferences (English, Japanese)
- Volume normalization
- Maximum volume set to 200%

### Subtitles

- Subtitle language preferences (English, Sinhala)
- Fuzzy subtitle auto-loading
- Customized subtitle appearance with Roboto font
- Improved subtitle visibility with borders and shadows

### User Interface

- Modern UI with [uosc](https://github.com/tomasklaen/uosc)
- Thumbnail previews on the timeline with thumbfast
- Customized OSD appearance
- Clean and minimal design

### Quality of Life

- Automatic position saving when quitting
- Screenshot functionality (PNG format)
- Automatic loading of similar named files
- Cache settings for smoother streaming playback
- YouTube-DL integration for online videos

## Installation

1. Clone this repository to your mpv configuration directory:

   **Linux/macOS**: `~/.config/mpv/`
   **Windows**: `%APPDATA%\mpv\`

   ```bash
   git clone https://github.com/ThilinaTLM/mpv-config ~/.config/mpv
   ```

2. Make sure you have the required dependencies:
   - mpv (latest version recommended)
   - yt-dlp (for online video playback)

## Structure

- `mpv.conf` - Main configuration file
- `uosc.conf` - Configuration for the uosc user interface
- `scripts/` - Custom scripts directory
  - `thumbfast.lua` - Script for thumbnail generation
  - `uosc/` - Modern UI replacement script
- `fonts/` - Custom fonts
  - `Roboto-Regular.ttf` - Main font for UI and subtitles
  - `uosc_icons.otf` - Icons for the uosc interface
  - `uosc_textures.ttf` - Textures for the uosc interface

## Customization

Feel free to modify any of these files to suit your preferences:

- Edit `mpv.conf` to change video, audio, and general settings
- Edit `uosc.conf` to customize the user interface
- Add or remove scripts in the `scripts/` directory

## Credits

- [mpv](https://mpv.io/) - The media player
- [uosc](https://github.com/tomasklaen/uosc) - Modern UI replacement
- [thumbfast](https://github.com/po5/thumbfast) - Thumbnail script

## License

This configuration is provided as-is, feel free to use and modify as needed.
