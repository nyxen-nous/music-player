MP3 Player

A simple command-line MP3 player written in Python with [Pygame](https://www.pygame.org/). It lists the songs in a local music folder, lets you select one by number, and provides playback controls from the terminal.

## Features

- Detects and lists `.mp3` files
- Select a track by its number
- Pause, resume, or stop the current track
- Return to the song list after stopping playback
- Handles missing audio folders, missing files, and invalid input

## Requirements

- Python 3
- Pygame

## Installation

Clone or download the project, then install the dependency:

```bash
pip install pygame
```

## Add music

The program looks for a folder named `musicMP3` **beside the project folder**. With this layout:

```text
parent-folder/
├── music player/
│   ├── main.py
│   └── README.md
└── musicMP3/
    ├── song-one.mp3
    └── song-two.mp3
```

Place your MP3 files in `musicMP3`. Only files ending in lowercase `.mp3` are included.

## Run

From the project directory, run:

```bash
python main.py
```

Choose a song number when prompted. While a song is playing, use these controls:

| Key | Action |
| --- | --- |
| `P` | Pause |
| `R` | Resume |
| `S` | Stop and return to the song list |

Enter `Q` at the song-selection prompt to quit the player.

## Project structure

```text
music player/
├── main.py       # Player application
├── README.md     # Project documentation
└── .gitignore
```
