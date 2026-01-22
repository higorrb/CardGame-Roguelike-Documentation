# CardGame-Roguelike-Documentation

Card Game Prototype (Work in Progress)

This project is a technical study developed using the Godot Engine and GDScript. The primary goal is to build a functional turn-based combat system inspired by deckbuilders, focusing on modular architecture and robust system logic.

Technical Features

    Turn-Based Combat System: State management controlling transitions between the Player's turn and the Enemy AI's turn.

    Card & Hand Management: System responsible for handling card data, including drawing from the deck, managing the player's hand size, and moving used cards to the discard pile. It includes an interactive "drag and drop" interface for card activation.

    Dice-Based Mechanics: Implementation of randomized dice rolls (D4, D6, D20) with support for dynamic damage and healing modifiers.

    Decision-Making AI: Logic-based enemy behavior that evaluates current health percentages to decide between offensive (attack) or defensive (heal) actions.

    Status Effect System: Scalable framework for applying and tracking status effects such as Weakness, Critical, Shields, and Healing.

    Dynamic UI & Visual Feedback: Real-time HUD updates including a floating combat text system and a detailed event log.

Tech Stack

    Engine: Godot 4.3

    Language: GDScript

    Design Patterns: Signal-based communication for UI decoupling and static methods for optimized visual effect instantiation.




Visual Documentation

1. Intent and Status System

The enemy AI displays icons for its next intended action and updates damage modifiers based on active status effects.

<img width="1272" height="717" alt="image" src="https://github.com/user-attachments/assets/85c7ac27-d14d-4c0a-a9e8-87c00a626fba" />

2. Combat Log and Event Tracking

The system provides a detailed record of every dice roll and action, ensuring transparency in gameplay mechanics.

<img width="770" height="238" alt="image" src="https://github.com/user-attachments/assets/b62a4819-70ce-43d3-9867-f9ea1dd18655" />

3. Visual Feedback (Floating Text)

Real-time damage and healing calculations are displayed directly over entities using color-coded labels.

<img width="1231" height="692" alt="image" src="https://github.com/user-attachments/assets/8cacd5ab-765c-49a7-9ed0-e3193d6013eb" />
