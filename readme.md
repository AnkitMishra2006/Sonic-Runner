# 🦔 Sonic Ring Run

A fast-paced endless runner game featuring Sonic the Hedgehog, built with JavaScript and the Kaplay game engine. Jump, collect rings, and avoid enemies in this exciting side-scrolling adventure!

## 🚀 Live Demo

**[Play the Game](https://sonic-runner06.netlify.app/)**

## 🎮 Game Features

- **Endless Running**: Infinite side-scrolling gameplay with increasing difficulty
- **Ring Collection**: Collect rings to increase your score
- **Enemy Combat**: Jump on Motobug enemies to destroy them and earn bonus points
- **Score Multiplier**: Chain enemy defeats for higher score multipliers
- **Ranking System**: Earn ranks from F to S based on your performance
- **Responsive Controls**: Play with keyboard (Space), mouse click, or touch
- **Progressive Difficulty**: Game speed increases over time for added challenge
- **Sound Effects**: Immersive audio with background music and sound effects

## 🕹️ How to Play

### Controls

- **Space Bar** / **Left Mouse Click** / **Touch Screen**: Make Sonic jump

### Gameplay

1. Sonic runs automatically from left to right
2. Jump to avoid Motobug enemies on the ground
3. Collect yellow rings to increase your score (+1 point each)
4. Jump on enemies to destroy them and earn bonus points (+10 × multiplier)
5. Chain enemy defeats while airborne to increase your score multiplier
6. Survive as long as possible as the game gets faster!

### Scoring System

- **Rings**: +1 point each
- **Enemy Defeat**: +10 points (×1 for first enemy)
- **Score Multiplier**: Increases with consecutive enemy defeats while airborne
- **Ranking**: F (0-49), E (50-79), D (80-99), C (100-199), B (200-299), A (300-399), S (400+)

## 🛠️ Technology Stack

- **Game Engine**: [Kaplay](https://kaplayjs.com/) v3001.0.12
- **Build Tool**: [Vite](https://vitejs.dev/) v6.2.0
- **Language**: JavaScript (ES6+)
- **Graphics**: Custom sprite sheets and animations
- **Audio**: WAV and MP3 sound files
- **Deployment**: Netlify

## 📁 Project Structure

```
sonic-runner/
├── public/
│   ├── fonts/
│   │   └── mania.ttf              # Custom font
│   ├── graphics/
│   │   ├── chemical-bg.png        # Background image
│   │   ├── motobug.png           # Enemy sprite sheet
│   │   ├── platforms.png         # Platform tiles
│   │   ├── ring.png              # Ring animation sprite sheet
│   │   └── sonic.png             # Sonic sprite sheet
│   └── sounds/
│       ├── city.mp3              # Background music
│       ├── Destroy.wav           # Enemy destruction sound
│       ├── Hurt.wav              # Damage sound
│       ├── HyperRing.wav         # Special ring sound
│       ├── Jump.wav              # Jump sound effect
│       └── Ring.wav              # Ring collection sound
├── src/
│   ├── entities/
│   │   ├── motobug.js            # Enemy entity logic
│   │   ├── ring.js               # Ring entity logic
│   │   └── sonic.js              # Player character logic
│   ├── scenes/
│   │   ├── game.js               # Main gameplay scene
│   │   ├── gameOver.js           # Game over screen
│   │   └── mainMenu.js           # Main menu scene
│   ├── kaplayCtx.js              # Game engine configuration
│   └── main.js                   # Entry point and asset loading
├── index.html                    # HTML entry point
├── package.json                  # Dependencies and scripts
├── vite.config.js               # Vite configuration
└── README.md                     # This file
```

## 🚀 Getting Started

### Prerequisites

- **Node.js** (version 14 or higher)
- **npm** or **yarn**

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/AnkitMishra2006/Sonic-Runner.git
   cd Sonic-Runner
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start development server**

   ```bash
   npm run dev
   ```

4. **Open your browser**
   - Navigate to `http://localhost:5173`
   - Start playing!

### Build for Production

```bash
npm run build
```

The built files will be in the `dist/` directory.

### Preview Production Build

```bash
npm run preview
```

## 🎨 Game Assets

### Sprites

- **Sonic**: 8×2 sprite sheet with running and jumping animations
- **Ring**: 16×1 sprite sheet with spinning animation
- **Motobug**: 5×1 sprite sheet with running animation
- **Background**: Scrolling chemical plant themed background
- **Platforms**: Tiled platform graphics

### Audio

- **Background Music**: Looping city theme
- **Sound Effects**: Jump, ring collection, enemy destruction, and damage sounds

## 🎯 Game Mechanics

### Physics

- **Gravity**: 5000 units (configurable)
- **Jump Force**: 1700 units
- **Game Speed**: Starts at 300, increases by 50 every second

### Collision Detection

- **Ring Collection**: Area-based collision detection
- **Enemy Interaction**:
  - Ground contact: Game over
  - Airborne contact: Enemy destruction + score bonus

### Spawning System

- **Enemies**: Random spawn intervals (0.8-2.5 seconds)
- **Rings**: Random spawn intervals (0.5-3 seconds)
- **Positioning**: Off-screen right, move left at game speed

## 🏆 High Score System

The game features a persistent high score system that saves your best performance:

- Scores are saved locally in browser storage
- Best score and rank are displayed on the game over screen
- Ranking system provides goals for improvement

## 🛡️ Browser Compatibility

- **Chrome**: ✅ Fully supported
- **Firefox**: ✅ Fully supported
- **Safari**: ✅ Fully supported
- **Edge**: ✅ Fully supported
- **Mobile Browsers**: ✅ Touch controls supported

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'Add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Contribution Ideas

- Add new enemy types
- Implement power-ups
- Create new background themes
- Add more sound effects
- Improve mobile responsiveness
- Add particle effects

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Ankit Mishra**

- GitHub: [@AnkitMishra2006](https://github.com/AnkitMishra2006)
- Project: [Sonic-Runner](https://github.com/AnkitMishra2006/Sonic-Runner)

## 🙏 Acknowledgments

- **Sonic the Hedgehog** - Original character by SEGA
- **Kaplay** - Excellent game engine for web games
- **Vite** - Fast build tool and development server
- **Netlify** - Hosting and deployment platform

**Made with ❤️ and JavaScript**

_Ready to run fast? [Play Sonic Ring Run now!](https://sonic-runner06.netlify.app/)_
