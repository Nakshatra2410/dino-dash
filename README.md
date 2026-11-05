# 🦖 Dino Dash – Endless Runner Game

A fun, lightweight, and interactive endless runner game inspired by the classic Chrome Dinosaur Game. Built entirely using **HTML, CSS, JavaScript, and HTML5 Canvas**, Dino Dash challenges players to jump over randomly generated cactus obstacles while trying to achieve the highest possible score.

The game features smooth animations, realistic jump physics, increasing difficulty, sound effects, and persistent high-score tracking — all packed into a single HTML file.

## 🎮 Live Gameplay

Run, jump, dodge obstacles, and see how long you can survive!

## ✨ Features

- **Continuous Running Animation:** The dinosaur runs continuously while the ground scrolls to create an endless running effect.
- **Dynamic Obstacles:** Randomly generated cactus obstacles with varying heights and spacing.
- **Realistic Jump Physics:** Gravity-based jumping with smooth movement and landing mechanics.
- **Increasing Difficulty:** Game speed gradually increases as the player progresses.
- **Collision Detection:** Detects collisions between the dinosaur and obstacles to trigger Game Over.
- **Score Tracking:** Displays the player's current score during gameplay.
- **High Score System:** Saves the highest score using browser `localStorage`, even after refreshing the page.
- **Start and Game Over Screens:** Interactive screens for starting and restarting the game.
- **Keyboard Controls:** Supports Spacebar and Up Arrow for jumping.
- **Mobile Support:** Touch-based controls for mobile devices.
- **Sound Effects:** Dynamically generated jump, collision, and score sounds using the Web Audio API.
- **Responsive Design:** Adapts to different screen sizes.
- **No External Dependencies:** Runs directly in a modern web browser without installing additional libraries or frameworks.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Game structure and Canvas element |
| CSS3 | Styling, layout, responsiveness, and visual effects |
| JavaScript (ES6+) | Game logic, physics, controls, and interactions |
| HTML5 Canvas | Rendering the dinosaur, obstacles, background, and animations |
| Web Audio API | Generating game sound effects |
| LocalStorage API | Persisting the player's high score |

## 📂 Project Structure

```text
Dino-Dash/
│
└── dino_dash.html
```

The entire project is contained in a single HTML file, including all HTML markup, CSS styling, and JavaScript functionality.

## 🚀 Getting Started

No installation, dependencies, or build tools are required.

### 1. Clone the Repository

```bash
git clone <repository-url>
```

### 2. Navigate to the Project Folder

```bash
cd Dino-Dash
```

### 3. Run the Game

Open `dino_dash.html` directly in Google Chrome or any modern web browser.

Alternatively, open the file using the VS Code Live Server extension.

That's it! The game is ready to play.

## 🕹️ Game Controls

| Control | Action |
|---|---|
| `Spacebar` | Jump |
| `↑ Up Arrow` | Jump |
| `Touch / Tap` | Jump on mobile devices |
| `R` | Restart after Game Over |
| `M` | Toggle sound effects |

## 🧠 How the Game Works

The game uses an animation loop powered by `requestAnimationFrame()` to continuously update and render the game.

### 1. Canvas Rendering
The HTML5 Canvas API draws the dinosaur, scrolling ground, clouds, and cactus obstacles.

### 2. Jump Physics
The dinosaur's vertical movement is calculated using velocity and gravity. Jumping applies an upward velocity, while gravity gradually pulls the dinosaur back toward the ground.

### 3. Obstacle Generation
Cactus obstacles are generated dynamically with randomized dimensions and spacing. They move toward the dinosaur to simulate forward movement.

### 4. Collision Detection
Bounding-box collision detection checks whether the dinosaur overlaps an obstacle. A collision immediately ends the current run.

### 5. Difficulty Progression
The game gradually increases its speed based on the distance travelled, making obstacles harder to avoid over time.

### 6. Score and High Score
The score increases as the game progresses. The highest score is stored in browser local storage so that it remains available across sessions.

### 7. Sound Effects
The Web Audio API generates simple sound effects programmatically without requiring external audio files.

## 🔧 Customization

The game contains a centralized settings object in the JavaScript section, making important gameplay parameters easy to modify.

```javascript
const settings = {
    gravity: 1900,
    jumpVelocity: -690,
    initialSpeed: 360,
    maxSpeed: 760,
    speedGain: 7.5,
    scoreRate: 12
};
```

You can modify these values to experiment with:

- Jump height and duration.
- Gravity and falling speed.
- Initial game speed.
- Maximum game speed.
- Difficulty progression.
- Score accumulation rate.

## 🌐 Browser Compatibility

Designed to work in modern browsers supporting:

- HTML5 Canvas
- JavaScript ES6+
- Web Audio API
- LocalStorage API
- Pointer Events

Recommended browser: Google Chrome.

## 🎯 Learning Outcomes

This project demonstrates practical implementation of:

- HTML5 Canvas-based game development.
- JavaScript game loops and animation.
- Basic physics simulation.
- Event handling and keyboard interactions.
- Randomized object generation.
- Collision detection algorithms.
- Browser storage management.
- Web Audio API integration.
- Responsive web design.

## 🔮 Future Enhancements

Some possible improvements include:

- Add different obstacle types.
- Introduce day and night themes.
- Add power-ups and special abilities.
- Implement multiple difficulty levels.
- Add a pause and resume feature.
- Introduce character customization.
- Add additional visual effects and animations.

## 📜 License

This project is open-source and available for learning, experimentation, and personal use.

---

**Built with ❤️ using HTML, CSS, JavaScript, and HTML5 Canvas.**

*Run. Jump. Survive. Beat your best!* 🦖