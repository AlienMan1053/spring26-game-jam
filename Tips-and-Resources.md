# Tools

You can build your game using simple, beginner-friendly tools.

**Recommendations:**
1. Pygame
2. Godot

Other engines + tools can be used if you feel comfortable. Just let us know what you will be using.

## 1. Pygame

 [Pygame](https://pypi.org/project/pygame-ce/) is a free, open-source library for making 2D games in Python.
- Handles graphics, sound, input, and basic game logic
- Beginner-friendly. Start with just Python knowledge

**Example**
A game just repeats this loop: **input → update → draw → repeat**

Example structure:
```python
import pygame
pygame.init()

screen = pygame.display.set_mode((800, 600))
running = True

while running:
    # 1. Input (events)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # 2. Update (game logic)
    # move things, check stuff

    # 3. Draw
    screen.fill((0, 0, 0))  # clear screen
    # draw shapes with screen.blit(...)
    pygame.display.flip()   # show changes

pygame.quit()
```

**What to Remember:**
* Init → start pygame
* Loop → keeps game running
* Events → handle input
* Draw every frame → or nothing shows
* Flip display → update screen

If you haven't used VSCode before, you should probably familiarize yourself with it if you are going to build your game using PyGame.

VSCode setup for Python:
https://www.youtube.com/embed/9o4gDQvVkLU?si=odk4pwgKAfwjVAjH

Pygame basic tutorial:
https://www.youtube.com/embed/blLLtdv4tvo?si=lXQ7dtIKV_k7Src1

---

## 2. Godot

[Godot](https://godotengine.org/) is a free, open-source game engine used to create 2D and 3D games. It includes built-in tools for graphics, physics, scripting, and scene design, so you can build games without needing many external programs.

It’s beginner-friendly thanks to its visual editor and simple scripting language (GDScript, similar to Python), making it easy to prototype and develop complete games quickly.

**Tutorials:**

There are plenty of great tutorials and resources on YouTube and online.

* [Godot platformer in 20 seconds](https://www.youtube.com/watch?v=thgdTkxeNJY)
* [Bouncing ball in Godot in 20 seconds](https://www.youtube.com/watch?v=GaT8veJJKOQ)


## General Resources
You may and are encouraged to use templates and resources online! 

There are lots of helpful Game Jam beginner tips videos on YouTube.

You can also use AI to generate skeleton code, functions, ideas, etc.

Template Examples:
* [Beginner PyGame templates](https://gist.github.com/MatthewJA/7544830)
* [itch.io Game Jam Game Starter Template](https://hatmix.itch.io/game-jam-starter-template)
* [itch.io Web Game Template](https://mangomoose.itch.io/web-game-template)
* [Godot 2D Platformer Starter Kit](https://godotengine.org/asset-library/asset/2201)
* [Godot Templates](https://godotengine.org/asset-library/asset?page=1&filter=template)
* [Narrative Web Game Template (HTML+CSS+JS)](https://ifthencreate.itch.io/narrativegametemplate)
* [Platformer](https://api.arcade.academy/en/2.6.17/examples/template_platformer.html)

Free Assets you can use 
* CraftPix 
* OpenGameArt 
* itch.io Free Assets 
* Kenney assets 

---

## Constraints and Design Tips: 
(i.e. How to keep yourself from getting lost in the sauce)

* **Games should be 2D only**

### **Scoping**
Most student teams over-scope. A tiny finished game is better than a big unfinished one!
Finished > Perfect

 * **Good examples:**

  * Click to stack blocks
  * Dodge falling objects
  * Rhythm tapping game
* **Bad examples:**

  * Open-world RPG ❌
  * Online multiplayer ❌
  * Story-driven adventure ❌
* If your idea sounds like a full Steam game, it’s too big.

**Game = Goal + Obstacle + Feedback**
  * **Example:**

    * Goal: Survive
    * Obstacle: Falling rocks
    * Feedback: Sound + score

That’s all you need for a complete game!



### **Design Constraints**
* **Games should be 2D only**
* 🕹️ **One Button Game**

  * Only one input (e.g., spacebar or mouse click)
  * Examples: Flappy Bird-style, timing-based games, endless runners
  * 👉 Best beginner-friendly restriction
* 🧱 **Single Mechanic Only**

  * One core interaction (jump, shoot, drag, rotate, etc.)
  * No combining systems
* 📦 **One Screen Game**

  * Everything happens on one screen
  * No levels, menus, or camera movement
* ⏱️ **30 Seconds of Gameplay**

  * Game must loop or end within 30 seconds
* 🎮 **No Player Movement**

  * Player stays still; game comes to them

**Recommendation:**
* Choose at least 2 constraints if you don't want to be in dev purgatory for days!
* One button + one screen + 30 seconds
---

## Development Process Tips
This isn't a strict schedule or checklist, but these practices can help you and your team stay informed on how everyone else is doing. These are similar practices to what AGILE software development teams do.

**1. Set a goal for each day.** e.g.:
* Day 1: Something works 
* Day 2: Playable (most important) 
* Day 3: Iterate 
* Day 4: Polish 
* Day 5: Submit!


**2. Have a basic rhythm for each day.** e.g.:

- **Beginning of day: Quick Check-In with team**
  - Yesterday: what did you do?
  - Today: pick ONE small goal
  - Any blockers (things you're stuck on)?

- 🎯 **Start with ONE Task**
  - Examples:
    - “Player moves”
    - “Enemy spawns”
    - “Score works”
  - If it takes more than a couple hours → too big

- 💻 **Build**
  - Build → Test → Fix → Repeat
  - (Test every ~10–15 min you're working)

- 🧪 **Quick Test (end of session)**
  - Can someone play it?
  - Is it clear what to do?

- 📣 **Post Progress (on Discord)**
  - Screenshot/clip + 1 sentence

- **Check Daily Goals**

- **One key rule:** If it’s not playable, stop adding new features!
