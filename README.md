# Pacman Game

A classic Pacman game implementation using vanilla JavaScript and HTML5 Canvas. Navigate through the maze, collect all the food pellets, and avoid the ghosts!

## 🎮 Features

- **Classic Pacman Gameplay**: Navigate through a maze collecting food pellets
- **Animated Characters**: Smooth animations for Pacman and ghosts
- **AI Ghosts**: Four intelligent ghosts that chase Pacman using pathfinding algorithms
- **Score System**: Track your score as you collect food
- **Lives System**: Start with 3 lives
- **Win/Lose Conditions**: Win by collecting all food, lose if you run out of lives

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- A local web server (optional, but recommended)

### Installation

1. Clone or download this repository
2. Ensure all files are in the same directory:
   - `index.html`
   - `game.js`
   - `pacman.js`
   - `ghost.js`
   - `assets/animations.gif`
   - `assets/ghost.png`

3. Open `index.html` in your web browser
   - For best results, use a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     
     # Using PHP
     php -S localhost:8000
     ```
   - Then navigate to `http://localhost:8000` in your browser

## 🎯 How to Play

### Controls

- **Arrow Keys** or **WASD** to move Pacman
  - Left Arrow / A: Move left
  - Right Arrow / D: Move right
  - Up Arrow / W: Move up
  - Down Arrow / S: Move down

### Gameplay

1. Use the arrow keys or WASD to navigate Pacman through the maze
2. Collect all the orange food pellets to win
3. Avoid the ghosts - if they catch you, you lose a life
4. You have 3 lives total
5. Win by reaching a score of 100 (collecting all food)
6. Game over if you lose all lives

### Objective

- Collect all food pellets in the maze
- Avoid collision with ghosts
- Achieve the highest score possible

## 📁 Project Structure

```
Pacman/
├── index.html          # Main HTML file with canvas
├── game.js            # Game logic, rendering, and game loop
├── pacman.js          # Pacman class with movement and collision
├── ghost.js           # Ghost class with AI pathfinding
├── assets/
│   ├── animations.gif # Pacman animation sprites
│   └── ghost.png      # Ghost sprites
└── README.md          # This file
```

## 🔧 Technical Details

### Technologies Used

- **HTML5**: Structure and canvas element
- **JavaScript (ES6+)**: Game logic and classes
- **Canvas API**: 2D rendering and animations

### Game Mechanics

- **Game Loop**: Runs at 30 FPS
- **Collision Detection**: Map-based collision system
- **Ghost AI**: Breadth-First Search (BFS) pathfinding algorithm
- **Ghost Behavior**: 
  - Ghosts chase Pacman when within range
  - Ghosts use random targets when Pacman is out of range
  - Ghost speed is half of Pacman's speed

### Map System

The game uses a 2D array map where:
- `0` = Empty space (outside walls)
- `1` = Wall
- `2` = Food pellet
- `3` = Eaten food pellet

## 🎨 Customization

You can easily customize the game by modifying variables in `game.js`:

- `fps`: Change the game frame rate
- `ghostCount`: Number of ghosts (default: 4)
- `lives`: Starting lives (default: 3)
- `wallColor`: Maze wall color
- `foodColor`: Food pellet color

## 🐛 Known Issues

- Ghosts may occasionally get stuck or behave unexpectedly in certain map configurations
- The game does not support mobile touch controls (keyboard only)

## 📝 License

This project is open source and available for educational purposes.

## 🙏 Acknowledgments

- Classic Pacman game by Namco
- Built for learning JavaScript game development

---

**Enjoy playing!** 🎮👻

