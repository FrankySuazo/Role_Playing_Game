# ⚔️ Role Playing Game

A browser-based **Role Playing Game built with HTML, CSS, and JavaScript** where the player explores different locations, purchases equipment, fights monsters, earns experience and gold, and ultimately attempts to defeat a dragon.

The goal of this project was to strengthen my understanding of **JavaScript fundamentals and interactive web development** by building a complete game around state management, functions, objects, arrays, conditional logic, DOM manipulation, and randomized game mechanics.

**Can you defeat the dragon? 🐉**

## 🎮 How the Game Works

The player begins with:

- ❤️ **100 Health**
- 💰 **50 Gold**
- ⭐ **0 XP**
- 🪵 A **Stick** as the starting weapon

From the town square, the player can choose where to go and what to do.

### 🏪 Visit the Store

The store allows the player to:

- Purchase additional health
- Buy increasingly powerful weapons
- Manage an inventory
- Sell weapons for additional gold

Weapons progress from:

`Stick → Dagger → Claw Hammer → Sword`

Each weapon has its own attack power.

### 🕳️ Explore the Cave

The cave contains enemies of different difficulty levels:

- Slime
- Fanged Beast
- Dragon

Defeating enemies rewards the player with **XP and gold**, which can then be used to become stronger before attempting the final battle.

### ⚔️ Combat

During combat, the player can:

- Attack
- Dodge
- Run

Combat contains randomized elements, so attacks and damage are not completely predictable.

Player damage depends on the currently equipped weapon and accumulated XP, while enemy damage is influenced by the monster's level.

Weapons also have a chance of breaking during combat, adding additional risk to each fight.

### 🐉 Win Condition

The ultimate objective is to defeat the **Dragon**.

If the player's health reaches zero first, the game ends and can be restarted.

Defeat the dragon and you win. 🎉

## 🧠 How It Was Built

The game separates the interface, styling, and game logic across:

```text
Role_Playing_Game/
├── Index.html
├── styles.css
├── script.js
└── README.md
```

### HTML

HTML provides the game interface, including:

- Player statistics
- Monster statistics
- Action buttons
- Game text and messages

### CSS

CSS controls the visual presentation and layout of the game interface.

### JavaScript

JavaScript contains the main game engine.

The game tracks state using variables such as:

```javascript
let xp = 0;
let health = 100;
let gold = 50;
let currentWeapon = 0;
let inventory = ["stick"];
```

Arrays of objects are used to organize game data such as weapons, monsters, and locations.

For example, weapons contain both a name and attack power:

```javascript
const weapons = [
  { name: "stick", power: 5 },
  { name: "dagger", power: 30 },
  { name: "claw hammer", power: 50 },
  { name: "sword", power: 100 }
];
```

Instead of creating completely separate interfaces for every location, the game updates the existing interface dynamically.

Each location defines its available buttons, functions, and descriptive text. JavaScript then changes the DOM based on the player's current location.

This allowed the same interface to represent the town, store, cave, battles, victory screen, and game-over screen.

## 🎲 Randomized Game Mechanics

The project also uses `Math.random()` to introduce unpredictability.

Randomness affects several parts of the game, including:

- Whether attacks hit
- Attack damage
- Weapon breaking
- A hidden number-based minigame

This makes the game behave differently between playthroughs instead of following one completely predetermined sequence.

## 🥚 Easter Egg

The game contains a small hidden number game.

The player chooses a number, and JavaScript generates ten random numbers. If the selected number appears among them, the player wins additional gold. Otherwise, the player loses health.

This feature gave me additional practice using:

- `while` loops
- `for` loops
- Arrays
- `.push
