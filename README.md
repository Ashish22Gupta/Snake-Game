# 🐍 Snake Game
### Classic Arcade Snake — Browser Edition

> ⚠️ **DISCLAIMER:** This is a **personal learning and portfolio project**. It is a browser-based recreation of the classic Snake arcade game, built for educational and demonstration purposes. All game logic runs entirely in the browser — no data is collected, stored, or transmitted.

A modern take on the timeless Snake game, built with jQuery and vanilla CSS. Guide a lime-green snake around a dark arena, eat glowing blue food to grow, and avoid hitting the walls or your own tail. Features a custom SVG snake head with eyes and tongue, a rainbow-gradient restart button, keyboard + on-screen touch controls, and a responsive layout that adapts to mobile.

![Version](https://img.shields.io/badge/Version-1.0.0-32CD32)
![Status](https://img.shields.io/badge/Status-Portfolio%20Project-F4B400)
![Responsive](https://img.shields.io/badge/Responsive-Desktop%20%26%20Mobile-2D6A4F)

---

## 🔗 Live Links

- **Live Demo:** [blockade-snake-gmae.netlify.app](https://blockade-snake-gmae.netlify.app)
- **Source Code:** [github.com/Ashish22Gupta/Snake-Game](https://github.com/Ashish22Gupta/Snake-Game)

---

## ✨ Implemented Features

### 🎮 Core Gameplay
- **Classic Snake Mechanics** - Move continuously in four directions; eat food to grow; avoid walls and self-collision.
- **Growing Snake** - Each food item increases the score by 1 and extends the tail by one segment.
- **Self-Collision Detection** - Game ends if the head overlaps any body segment.
- **Wall Collision Detection** - Game ends if the head leaves the arena boundaries.
- **Speed** - Fixed `200ms` tick rate via `setInterval`.

### 🐍 Custom Snake Rendering
- **SVG Head with Direction** - The head rotates 0°/90°/180°/270° based on movement direction, with two black eyes.
- **Red SVG Tongue** - A forked tongue SVG extends in front of the head, also direction-aware.
- **Rounded Body Segments** - Body pieces use `border-radius: 5px`; the tail is a full circle (`50%`).
- **Directional Positioning** - Body and tongue offsets recalculate per direction so the visual stays coherent.

### 🍎 Animated Food
- **Glowing Blue Orb** - Food pulses between blue and white with a `glow` keyframe animation.
- **Random Placement** - Spawns at a random grid-aligned position within the arena bounds.

### 🎨 Visual Design
- **Purple Backdrop** - `rgb(165, 102, 223)` page background for a vibrant arcade feel.
- **Dark Arena** - `#333` playfield with a diagonal striped red border via `border-image`.
- **Rainbow Restart Button** - Animated gradient button (yellow → orange → red → violet → purple → blue) that cycles on hover.
- **Restart on Game Over** - Injects a restart button inside the arena after a loss, with a built-in SVG refresh icon.

### 📱 Responsive & Touch Controls
- **Keyboard Support** - Arrow keys control direction, with a guard preventing 180° reversals.
- **On-Screen Buttons** - D-pad style controls (↑ ← ↓ →) appear on screens up to `1280px` wide.
- **Fluid Arena** - Arena scales via `100vw` capped at `500px` for mobile and desktop.
- **Touch-Optimized Buttons** - 50×50px orange buttons with `:active` darkening feedback.

### 🏆 Score Display
- **Live Score** - Score updates at the top in real time as food is eaten.
- **Final Score on Loss** - Displays `"Your Score is: X"` and alerts the final score on game over.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Markup with arena, controls, and score containers |
| **CSS3** | Gradients, border-image, keyframe animations, responsive media queries |
| **jQuery 3.6** | DOM creation, event handling, element manipulation |
| **Vanilla JS logic** | Snake movement, collision detection, food spawning |
| **Inline SVG** | Snake head tongue, restart icon |
| **Netlify** | Static hosting and deployment |

---

## 📁 Project Structure

```text
Snake-Game/
└── index.html          # Self-contained game: markup + styles + logic
