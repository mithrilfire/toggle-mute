# Toggle Mute

Basic microphone toggle script with sound effects.

## To-do

- [ ] Add sound efect files to project.
- [ ] Add cli flag for built-in feature, it's too specific.
- [ ] Add help text for command line.
- [ ] Add Installation section, icon, and images to `README.md`

## Features

1. Toggle your external microphone with `mute` command.
2. Play sound effects related to next microphone state.
3. If somehow connection to external microphone lost, don't toggle built-in microphone and play error sound.

## Prerequisites

This script uses `pactl`(included in `pulseaudio-utils`), `paplay` command-line tools, so these need to be installed in your system.

Currently sound effects don't comes with script. They need to be in a folder named `assets/` which be in same directory with script. Default file names are can be changed from script. 

**File Names:**
- Alert: `alrt.wav`
- Mute: `mute.wav`
- Unmute: `unmt.wav`

**Example file structure:**
```
.
├── assets
│   ├── alrt.wav
│   ├── mute.wav
│   └── unmt.wav
├── mute
└── README.md
``` 