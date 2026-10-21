# Just a Hare Higher

A 2D platformer built with Python and Pygame. Play through levels as a rabbit, charge jumps to navigate platforms, collect items, avoid enemies, and reach the finish. The project also includes a custom tile-map editor for creating and saving levels.

## Features

- **Chargeable jumping:** Hold the jump key to charge a jump, then release it to launch.
- **Platforming physics:** Horizontal movement, collision handling, and coyote time for more forgiving jumps.
- **Enemies:** Multiple enemy types with distinct behaviors, including enemies that throw projectiles.
- **Collectibles:** Collect carrots and radishes to increase separate score totals.
- **Level progression:** Reach the finish collectible to complete a level.
- **Save data:** Store level completion, collectible totals, scores, and completion times.
- **Custom level editor:** Place and remove tiles, rotate assets, switch between grid and off-grid placement, and save maps as JSON.
- **Game settings:** Adjust display size and volume through the settings menu.

## Requirements

- Python 3
- Pygame

## Installation

Clone the repository and enter its directory:

```bash
git clone https://github.com/Elio-togm/Just-a-Hare-Higher.git
cd Just-a-Hare-Higher
```

Install Pygame:

```bash
python -m pip install pygame
```

## Running the Game

From the repository root, run:

```bash
python game.py
```

Keep the repository's `data/` and `scripts/` directories in place. The game loads its assets, level maps, and save data from the project directory.

## Controls

| Action | Input |
|---|---|
| Move left | Left Arrow or A |
| Move right | Right Arrow or D |
| Charge a jump | Hold Up Arrow, W, or Space |
| Execute a jump | Release the jump key |
| Exit | Escape |

The game also includes a debug input path. Consult the current source for additional debug controls.

## Level Editor

Launch the editor from the repository root:

```bash
python scripts/editor.py
```

The editor lets you create tile maps that the game can load.

| Action | Input |
|---|---|
| Pan around the map | Arrow keys or W, A, S, D |
| Place tiles | Left mouse button |
| Remove tiles | Right mouse button |
| Change tile group | Mouse wheel |
| Change tile variant | Hold Left Shift and use the mouse wheel |
| Toggle grid placement | G |
| Rotate selected tile | Left Ctrl |
| Save the map | O, then enter a map name |
| Exit | Escape |

Maps are saved as JSON files under `data/maps/`. Use a map name appropriate for the game's level-loading system when creating levels intended for normal gameplay.

## Project Structure

```text
Just-a-Hare-Higher/
├── game.py
├── scripts/
│   ├── editor.py
│   ├── entities.py
│   ├── tilemap.py
│   ├── utils.py
│   └── clouds.py
└── data/
    ├── maps/
    └── save_data/
```

The project also includes additional asset directories and supporting files.

## Technical Focus

This project explores real-time game loops, player movement and physics, collision detection, entity updates, collectible and enemy behavior, camera scrolling, JSON-based level data, and custom game-development tools.

## License

See the repository's license file for licensing information.
