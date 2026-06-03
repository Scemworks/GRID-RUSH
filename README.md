# Grid Rush: Focus & Speed Trainer

Grid Rush is a modern, responsive, high-performance web game designed to test and improve your peripheral vision, mental focus, and reflexes. Inspired by the classic **Schulte Grid** and "Touch the Numbers" speed tests, it challenging players to find and click randomized numbers in sequential order as fast as possible.

The entire application is self-contained in a single `index.html` file using vanilla CSS, modern HTML5 semantic elements, and native JavaScript.

## 🚀 Features

### 1. Game Modes
- **Classic Mode (1-25)**: A 5x5 grid containing numbers 1 to 25. Click them sequentially from 1 to 25.
- **Speed Rush Mode (1-50)**: A dynamic 5x5 grid. Clicking a number from 1 to 25 replaces it with its counterpart + 25 (e.g., clicking `1` turns the cell into `26`). Complete the board by clicking up to `50`.

### 2. Premium Theme System
Choose from three gorgeous, curated themes:
*   🌌 **Cyberpunk Dark**: A neon-drenched dark aesthetic with glowing borders, magenta/cyan gradients, and deep backdrop filters. (Default)
*   ⚪ **Minimalist Mono**: A clean, high-contrast black-and-white layout with sharp edges and subtle modern shadows.
*   🌴 **Vaporwave Retro**: Pastel pinks, light purples, teal accents, and retro-futuristic gradients.

### 3. Integrated Audio Synthesizer
The game features responsive sound effects generated entirely programmatically using the browser's native **Web Audio API** (no external audio files to download!):
- **Correct Hit**: A crisp, positive high synth chime.
- **Incorrect Hit**: A low-frequency buzz accompanied by a satisfying screen-shake animation.
- **Victory Arpeggio**: An uplifting retro 8-bit success melody.
- Sound effects can be muted/unmuted instantly from the header controls.

### 4. Precision Timing & Stats
- Uses `performance.now()` for millisecond-accurate timing.
- Active game tracking shows your next target, current speed (clicks per second), and progress.
- Canvas-based confetti explosion upon winning the game.

### 5. Local Leaderboard
- Tracks your top 5 personal best times for each mode.
- Scores are persisted using the browser's `localStorage`.

---

## 🛠️ Technology Stack
- **HTML5**: Semantic tags (`<header>`, `<main>`, `<footer>`, `<canvas>`).
- **CSS3**: Custom properties (CSS variables), grid layout, flexbox, dynamic glassmorphism, responsive viewports, transitions, and keyframe animations.
- **JavaScript (ES6+)**: Vanilla scripting, Fisher-Yates shuffle algorithm, custom Web Audio synthesis, standard web animation frames for canvas particles.

---

## 🎮 How to Play & Run
1. Since the application is fully client-side and self-contained, you can run it simply by opening `index.html` in any web browser.
2. Select your desired **Theme** and **Game Mode** using the top controls.
3. Click the **Start Game** button or click the number **1** cell directly to start the timer.
4. Scan the grid and click the numbers in increasing sequential order (1, 2, 3...).
5. If you make a mistake, you'll hear a buzzer and the screen will shake briefly. Keep going!
6. Once you click the final number, the timer stops, confetti flies, and your score is calculated. If you make it into the Top 5, your score will be added to the Leaderboard.
