# 2D Platformer Game

A classic 2D platformer game built with Unity, featuring dynamic gameplay, multiple enemy types, collectibles, and a boss battle system.

## 🎮 Game Overview

This is a side-scrolling platformer where players navigate through challenging levels, collect coins, defeat enemies, and battle bosses while racing against time. The game features smooth character animations, responsive controls, and an engaging gameplay loop.

## ✨ Features

### Core Gameplay
- **Player Movement**: Smooth horizontal movement and jumping mechanics with physics-based controls
- **Life System**: 3 lives with visual feedback and respawn mechanics
- **Timer System**: 60-second countdown timer adding urgency to gameplay
- **Score System**: Collect coins to increase your score with audio feedback
- **Water Hazards**: Fall into water and respawn at safe positions

### Enemy System
Multiple enemy types with unique behaviors:
- **Snails**: Ground-based enemies
- **Birds**: Flying enemies with egg-dropping mechanics
- **Spiders**: Web-crawling enemies
- **Frogs**: Jumping enemies
- **Boss Battles**: Special boss encounters with health systems and stone-throwing attacks

### UI & Menus
- **Main Menu**: Start game, access help, settings, and quit options
- **Game Over Screen**: Restart or quit when lives are depleted
- **HUD**: Real-time display of lives, coins, and timer
- **Pause Functionality**: Press ESC to return to main menu

### Visual Features
- Animated player character with walk, jump, and idle states
- Animated enemies and collectibles
- Parallax background system for depth
- Bonus blocks with interactive animations
- Customizable UI with multiple color themes (Blue, Green, Orange, Pink, Purple, Red)

## 🎯 Game Controls

| Action | Key |
|--------|-----|
| Move Left | A / Left Arrow |
| Move Right | D / Right Arrow |
| Jump | Spacebar |
| Shoot | (If enabled) |
| Pause/Menu | ESC |

## 🛠️ Technical Details

### Built With
- **Engine**: Unity (2D)
- **Language**: C#
- **Physics**: Unity Physics2D
- **UI**: Unity UI & TextMeshPro

### Project Structure
```
Assets/
├── Animations/          # Character and enemy animations
├── Prefabs/            # Reusable game objects
│   ├── Player Prefab/
│   ├── Enemy Prefabs/
│   └── Collectable Items/
├── Scenes/             # Game scenes
│   ├── Menu.unity      # Main menu scene
│   └── GameScene-ALU.unity  # Main gameplay scene
├── Scripts/            # C# game logic
│   ├── Player Scripts/
│   ├── Enemy Scripts/
│   ├── Boss Scripts/
│   ├── Controller Scripts/
│   ├── Camera Scripts/
│   └── Helper Scripts/
├── Sprites/            # 2D graphics and textures
└── Sounds/             # Audio files
```

### Key Scripts
- **PlayerMovement.cs**: Handles player movement, jumping, and ground detection
- **PlayerDamage.cs**: Manages player health, lives, and respawn system
- **GameManager.cs**: Controls game flow, timer, and scene transitions
- **ScoreManager.cs**: Tracks and displays coin collection
- **MainMenuController.cs**: Manages menu navigation
- **GameMenuController.cs**: Handles in-game menu actions (Play, Replay, Quit)
- **CameraFollow.cs**: Smooth camera tracking of player
- **BossScript.cs**: Boss AI and attack patterns
- **Enemy Scripts**: Individual AI for each enemy type

## 🚀 How to Run

### Prerequisites
- Unity Hub installed
- Unity Editor (2020.3 or later recommended)

### Setup Instructions
1. **Clone or Download** the project
2. **Open Unity Hub**
3. Click **Add** and navigate to the project folder
4. Select the Unity version (or let Unity Hub install the required version)
5. **Open the project**
6. In Unity, navigate to `Assets/Scenes/`
7. Open **Menu.unity** to start from the main menu
8. Press the **Play** button in Unity Editor

### Building the Game
1. Go to **File → Build Settings**
2. Add scenes in this order:
   - Menu.unity
   - GameScene-ALU.unity
3. Select your target platform (Windows, Mac, Linux)
4. Click **Build** and choose output folder
5. Run the executable file

## 🎨 Customization

### Changing UI Theme
The game includes 6 color themes for UI elements:
- Navigate to `Assets/Puzzle stage & settings GUI Pack/`
- Choose from: Image_blue, Image_green, Image_orange, Image_pink, Image_purple, Image_red
- Replace button sprites in the UI to change the theme

### Adjusting Difficulty
Modify these values in the Inspector:
- **Player Speed**: Adjust in PlayerMovement component
- **Jump Power**: Modify jumpPower variable
- **Timer Duration**: Change countTime in GameManager
- **Enemy Behavior**: Tweak individual enemy scripts

## 🎯 Game Mechanics

### Life System
- Start with 3 lives
- Lose a life when touching enemies or falling in water
- Respawn at last safe position or near water exit point
- Game Over screen appears when all lives are lost

### Timer System
- 60-second countdown per level
- Timer displayed in MM:SS format
- Game restarts when timer reaches zero
- Timer panel notification on time up

### Respawn System
- Safe position tracking (last ground position)
- Water respawn with offset positioning
- 2-second invulnerability after respawn

## 📝 Future Enhancements
- Multiple levels with increasing difficulty
- Power-ups and special abilities
- Sound effects and background music
- High score system with persistence
- Mobile touch controls
- Additional enemy types and boss battles

## 🐛 Known Issues
- Unity Connect token exchange errors (can be ignored or work offline)
- Camera continues following player briefly after death (visual only)

## 📄 License
This project is available for educational and personal use.

## 🤝 Contributing
Feel free to fork this project and submit pull requests for improvements!

---

**Enjoy the game!** 🎮✨
