# GPlay - Command Line MP3 Player

A modern, cross-platform command line MP3 player written in Python3.

## Features

- Play, pause, next, previous track controls
- Volume control
- Playlist management
- Track information display (title, artist, duration)
- Interactive command mode
- Command line arguments support
- Cross-platform compatibility

## Installation

1. Clone this repository
2. Create a virtual environment (recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Linux/MacOS
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Command Line Arguments

```bash
# Basic usage
python gplay.py /path/to/mp3s

# Play first track
python gplay.py /path/to/mp3s --play

# Play next track
python gplay.py /path/to/mp3s --next

# Set volume
python gplay.py /path/to/mp3s --volume 0.5
```

### Interactive Mode

Run without any arguments to enter interactive mode:

```bash
python gplay.py
```

Available commands in interactive mode:
- `p` - Play/Pause
- `n` - Next track
- `r` - Previous track
- `s` - Stop
- `v` - Set volume (0.0 to 1.0)
- `q` - Quit

## Requirements

- Python 3.6+
- pygame
- colorama
- tqdm
- mutagen

## Dependencies

The player uses pygame for audio playback, which requires SDL2 libraries. On Linux systems, you may need to install the following:

```bash
sudo apt-get install libsdl2-dev libsdl2-mixer-dev
```

## Note

This is a cross-platform version of the original Termux MP3 Player. It no longer requires Termux:API and can be used on any system that supports Python3.
