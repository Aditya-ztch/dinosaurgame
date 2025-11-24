## 🦖 Chrome Dinosaur — Java Swing Game

A fully working recreation of the **Chrome offline Dinosaur Game**, built using **Java AWT/Swing**.  
The player jumps to avoid cacti, scores points over time, and restarts after Game Over.

---

## 🎮 Gameplay

You control a dinosaur running endlessly.  
Cacti appear at random intervals and move from right to left.  
Jump over them to survive.  
The longer you survive → **the higher your score**.

---

## 🧰 Tech Stack

- **Language:** Java
- **GUI Framework:** Swing + AWT
- **Game Loop:** `javax.swing.Timer`
- **Rendering:** `Graphics.drawImage(...)`

No external game engines — pure Java code.

---

## 📁 Project Structure
dinosaurgame/
├── app.java # Creates the game window (JFrame) and launches the game
├── ChromeDinosaur.java # Game logic, player, obstacles, rendering, physics, collision
└── img/ # Game assets (sprites, icons)
├── dino-run.gif
├── dino-dead.png
├── dino-jump.png
├── cactus1.png
├── cactus2.png
├── cactus3.png
├── game-over.png




> ⚠️ All images must be inside the `img/` folder relative to `ChromeDinosaur.java`.  
> The game loads them using:
> ```java
> new ImageIcon(getClass().getResource("./img/filename")).getImage();
> ```

---

## 🚀 How to Run

### Option 1 — Using IDE
1. Open project in IntelliJ, VS Code, Eclipse, etc.
2. Run `app.java`
3. Window launches → Play!

---

### Option 2 — Using Terminal

Compile:
```bash
javac app.java ChromeDinosaur.java

