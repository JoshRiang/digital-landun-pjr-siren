# Digital Landun PJR Siren

A browser-based emergency siren simulator with six siren patterns and an air horn, inspired by Indonesian PJR (Patroli Jalan Raya) highway patrol vehicles.

![Siren App](https://user-images.githubusercontent.com/placeholder/siren-app.png)

## Siren Patterns

| Button | Pattern | Behavior |
|--------|---------|----------|
| **Wail** | Slow rising/falling tone | Hold for momentary, click to toggle loop |
| **Yelp** | Fast oscillating tone | Hold for momentary, click to toggle loop |
| **Phaser** | Police warning sweep | Hold for momentary, click to toggle loop |
| **Horn** | Air horn blast | Hold only, pauses active siren |
| **Pulsar** | Pulsing electronic tone | Hold for momentary, click to toggle loop |
| **HighLow** | Ambulance two-tone | Hold for momentary, click to toggle loop |

## Toggle Mode

Use the **Toggle** button (bottom) to switch between modes:
- **Red (off)**: Buttons play only while held (momentary)
- **Green (on)**: Buttons click to start/stop looping sirens

Only one siren plays at a time. The horn overrides the active siren and resumes it on release.

## Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (jQuery)
- **Audio**: Gapless5.js for seamless looping
- **Sound Files**: MP3 (7 tracks in `audio/`)

## Project Structure

```
├── index.html           # Main interface
├── css/
│   └── style.css        # Styling
├── js/
│   ├── siren.js         # Siren control logic
│   ├── gapless5.js      # Gapless audio library
│   └── gapless5_license.txt
└── audio/
    ├── SIREN_1.mp3      # Wail
    ├── SIREN_2.mp3      # Yelp
    ├── POLICE_WARNING.mp3  # Phaser
    ├── AIRHORN_EQD.mp3  # Horn
    ├── AMBULANCE_WARNING.mp3  # HighLow
    └── phaser.mp3       # Pulsar
```

## Usage

Open `index.html` in any modern browser. Audio streams from GitHub raw URLs, so an internet connection is required.

## Status

This project is closed. The successor lives at https://joshriang.cloud/works/landun-pjr

## Credits

- Gapless5.js by Regaip Sen (MIT License)

## License

MIT License