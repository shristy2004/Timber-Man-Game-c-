# Timber Man Game (C++ with SFML)

## Overview

Timber Man is a fast-paced arcade game built using C++ and SFML. You control a lumberjack cutting a tree while avoiding branches. The game focuses on timing and quick decisions.

## Features

* Smooth 2D graphics using SFML
* Real-time gameplay loop
* Increasing difficulty
* Score tracking
* Keyboard-based controls

## Tech Stack

* Language: C++
* Graphics Library: SFML (Simple and Fast Multimedia Library)
* Compiler: g++ / MSVC

## Requirements

* C++ compiler (g++ or Visual Studio)
* SFML installed (version 2.5 or later recommended)

## Installation

### 1. Install SFML


#### On Windows

* Download SFML from https://www.sfml-dev.org/download.php
* Extract it
* Set up include and lib paths in your compiler

### 2. Clone the repository

```bash
git clone https://github.com/shristy2004 /timber-man.git
cd timber-man
```

### 3. Compile and Run

#### On Linux (g++)

```bash
g++ src/main.cpp -o timberman -lsfml-graphics -lsfml-window -lsfml-system
./timberman
```

#### On Windows (MinGW example)

```bash
g++ src/main.cpp -o timberman -IC:\SFML\include -LC:\SFML\lib -lsfml-graphics -lsfml-window -lsfml-system
timberman.exe
```

## Project Structure

```bash
timber-man/
│
├── src/                # C++ source files
│   └── main.cpp
├── assets/             # Textures, fonts, sounds
├── README.md
```

## Game Mechanics

* Player switches between left and right sides of the tree
* Each key press cuts the tree
* Branches appear randomly
* Collision with a branch ends the game
* Score increases with each successful cut
* Game speed increases over time

## Controls

* A / Left Arrow → Move left and cut
* D / Right Arrow → Move right and cut
* Esc → Exit

## How It Works

* SFML handles rendering, window, and input
* Sprites represent player, tree, and branches
* Random generation controls branch placement
* Collision detection checks player safety
* Game loop updates frame-by-frame

   

## Future Improvements

* Add sound effects and background music
* Add animations for cutting
* Add menu and restart screen
* Add high score saving system
* Improve UI and visuals

## Common Issues

* Missing SFML DLLs on Windows
  → Copy SFML DLL files into the executable folder

* Black screen or missing textures
  → Check correct asset paths

## Contributing

1. Fork the repo
2. Create a new branch
3. Commit changes
4. Open a pull request

## License

Open-source project. Free to use and modify.

## Author

SHRISTY

GitHub: https://github.com/shristy2004 

## Acknowledgements

Inspired by the original Timberman game and built using SFML.
