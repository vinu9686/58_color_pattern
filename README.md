# Memory Color Pattern

A Simon-style memory game built with **Python** and **Pygame**. Watch the color sequence, then repeat it by clicking the pads in the same order. Each successful round adds one color to the pattern.

## Implemented tasks

All four tasks from the original lab README have been implemented:

1. **Sequence duplication fix** — each successful round appends exactly one new color to the existing sequence.
2. **Dynamic playback speed** — flash and pause durations decrease as the sequence grows. The flash duration has a 120 ms minimum and the pause has a 70 ms minimum.
3. **Pad sounds** — each color has a distinct generated tone. Tones play when a pad lights during playback and when the player clicks it. If audio is unavailable, the game continues without sound.
4. **Player-turn timer** — a countdown bar appears while the player enters the pattern. The time allowance decreases in later rounds, to a minimum of 3 seconds. Running out of time ends the game.

## Requirements

- Python 3.10 or newer
- Pygame

## Setup and run

Install Pygame:

```bash
python -m pip install pygame
```

Start the game from the project directory:

```bash
python main.py
```

## How to play

- Watch the pads light up and listen to their tones.
- Left-click the pads to repeat the complete sequence in order before the timer runs out.
- An incorrect click or an expired timer ends the game.
- Press **R** on the Game Over screen to start a new game.
- Close the window to exit.

## Project structure

```text
.
├── game/
│   ├── color_button.py   # Pad drawing and hit detection
│   └── game_engine.py    # Game state, sequence, timing, audio, and rendering
├── main.py               # Pygame window and main loop
└── README.md
```

## Submission checklist

- [ ] Record a 10-second video before the changes, showing the original issue.
- [ ] Record a 10-second video after the changes, showing the fixed sequence and implemented features.
- [ ] Include the link to the LLM chat page with the complete conversation history.
