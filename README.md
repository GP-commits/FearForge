# FearForge

Perfect 👍
Below is a **clean, jam-ready README** you can **copy–paste directly**.
It explains **every mechanic clearly**, in a way **judges + other devs understand instantly**.

---

# 🎮 GAME README

## 🩸 Game Title

**WHAT I DIDN’T DO**
*(Psychological Horror – Story Driven)*

---

## 🧠 Core Concept

This is a **first-person psychological horror game** focused on **guilt, silence, and consequences**.

The player controls a **father searching for his missing daughter**.
There is **no combat**, **no inventory UI**, and **no dialogue choices**.

The horror comes from:

* Movement
* Sound
* Environmental triggers
* Realization of inaction

---

## 🎮 Controls

| Input          | Action                       |
| -------------- | ---------------------------- |
| Mouse          | Look around                  |
| Keyboard       | Move                         |
| No Mouse Click | No clicking used in gameplay |

All interactions are **automatic and proximity-based**.

---

## 🧩 Core Mechanics Explained

---

### 🟦 1. Plate-Based Trigger System (Main Mechanic)

The entire game progression is controlled using **invisible / visible plates** placed in the world.

**How it works:**

* When the player **steps on a plate**, an event is triggered
* Each plate works **only once**
* Plates control:

  * Dialogue audio
  * Story progression
  * Spawning new elements
  * Monster activation

This avoids:

* UI prompts
* Clicking
* Complex interaction logic

---

### 🔊 2. Dialogue Audio System

* All story is told through **voice dialogue**
* Dialogue plays when stepping on specific plates
* Each dialogue plays **only once per gameplay**
* No subtitles or UI clutter

Audio is used to:

* Guide the player
* Build tension
* Reveal story details gradually

---

### 🔑 3. Key Acquisition Mechanism

**No inventory UI is used.**

**How it works:**

* A key model exists in the world
* A **Key Plate** is placed near it
* When the player steps on the plate:

  * The key is considered “picked up”
  * The key model disappears
  * A BoolValue (`HasRoomKey`) is set on the player

This keeps the system:

* Invisible
* Simple
* Story-focused

---

### 🚪 4. Door Unlock Mechanism

Doors do not open with clicks or animations.

**How it works:**

* Doors are simple Parts
* A **Door Plate** is placed in front of the door
* When the player steps on the plate:

  * If the player **has the key** → the door disappears
  * If not → nothing happens

This reinforces the theme:

> Some doors only open after it’s too late.

---

### 🧍‍♂️ 5. Player Progression Control

The player **cannot trigger future events early**.

Progression is controlled by:

* Spawning plates only after certain story moments
* Destroying old plates after use

This ensures:

* Linear story flow
* No sequence breaking
* No confusion

---

### 👹 6. Monster Activation Mechanism

The monster already has its **own AI script**.

**Important design choice:**

* The monster exists from the start
* Its AI script (`NPC`) is **disabled initially**

**Activation flow:**

1. Player steps on **Daughter Scream Plate**
2. Daughter scream audio plays
3. Monster AI script is enabled
4. Monster begins to move

The monster represents:

* Guilt
* Consequences
* What the player avoided

---

### 🏠 7. Environment-Driven Storytelling

There are:

* No cutscene videos
* No text popups

Story is told through:

* Audio
* Doors disappearing
* Objects vanishing
* Monster presence
* Player movement

The player **connects the story themselves**.

---

## 🧱 Technical Design Choices

* **Server Scripts** are used for:

  * Key logic
  * Door logic
  * Plate triggers
* **Local Scripts** are used only for:

  * Menu
  * Camera & input
* No complex AI modifications
* Asset-pack enemy logic preserved

---

## 🎯 Design Philosophy

* Less mechanics, more meaning
* No hand-holding
* Horror through implication
* Silence as a theme
* Player movement = player choice

---

## 🏁 Ending Philosophy

The game does not focus on:

* Winning
* Losing
* Multiple endings

The goal is:

> To make the player understand **what they didn’t do**.

---

## 🏆 Why This Game Stands Out

* No combat
* No UI dependency
* Strong narrative theme
* Audio-first horror
* Clean, stable systems
* Jam-friendly scope

---

## 📌 One-Line Summary

> A psychological horror game where progression is driven by footsteps, sound, and guilt — not weapons.

---

If you want, I can also:

* Shorten this README for submission
* Convert it to Markdown for GitHub
* Add a **Controls + Credits** section
* Write a **judge-facing description**

Just tell me 👍
