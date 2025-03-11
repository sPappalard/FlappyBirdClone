# Flappy Bird Clone

A clone of the popular mobile game 'Flappy Bird' developed in Unity for Android devices.


<img src="https://github.com/sPappalard/FappyBird-Clone/assets/149112901/3cfb7e82-06c1-495d-b008-50de0343f0df" alt="GIF">


## Game Overview

This is a simple implementation of the classic Flappy Bird game where players control a bird that must navigate through a series of pipes without hitting them. The game features:

- Simple one-touch controls
- Randomly generated pipes at varying heights
- Score tracking
- Game over screen with restart functionality
- Sound effects

## How It Works

### Game Mechanics

- **Controls**: Tap the screen to make the bird flap its wings and gain altitude
- **Objective**: Navigate through as many pipes as possible without colliding
- **Scoring**: Each successfully passed pipe awards one point
- **Game Over**: Occurs when the bird collides with a pipe or the ground

### Technical Implementation

The game is built using several key scripts:

#### GameController.cs
Manages the core game mechanics:
- Controls the spawning of pipes at random heights
- Handles the game over state
- Maintains the global game state that other scripts reference

#### Flappy.cs
Controls the player character (the bird):
- Implements physics-based movement using Rigidbody2D
- Handles player input (screen taps)
- Detects collisions with obstacles
- Triggers game over state and UI elements
- Manages sound effects for flapping and collisions

#### Tubi.cs (Pipes)
Manages the pipe obstacles:
- Controls horizontal movement of pipes from right to left
- Handles pipe destruction when they move off-screen
- Increments the score when the player successfully passes through
- Plays a sound effect when a point is scored

#### Pavimento.cs (Floor)
Controls the scrolling floor:
- Creates an endless scrolling effect
- Resets position when it reaches the end point
- Stops scrolling when game over occurs

#### Punti.cs (Points)
Manages the score display:
- Keeps track of the player's score
- Updates the UI text element with the current score

#### Restart.cs
Handles game restart functionality:
- Resets the game state when the restart button is pressed
- Reloads the game scene

## Features

- **Endless Gameplay**: The game continues as long as the player can avoid obstacles
- **Progressive Difficulty**: As players advance, navigating through pipes becomes challenging
- **Simple UI**: Clean interface with score display and restart button
- **Audio Feedback**: Sound effects for flapping, scoring, and game over
- **Authentic Experience**: Maintains the challenging and addictive nature of the original game

## Development

This game was developed using Unity and C#, with careful attention to recreating the feel and mechanics of the original Flappy Bird game while optimizing for Android devices.

## Installation

To install and play on an Android device:
1. Download the APK file
2. Enable installation from unknown sources in your device settings
3. Install the APK
4. Launch the game and start playing!

## Contributing

Feel free to fork this repository and make your own improvements. Pull requests are welcome!

## License

This project is licensed under the MIT License --->  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
