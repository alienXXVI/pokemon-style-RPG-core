# Pokémon-Style RPG Core

## Description
This project focuses on recreating the fundamental systems found in classic 2D monster-catching RPGs. It provides a robust foundation for character movement, environmental interaction, and seamless transitions between different game maps (such as moving from an overworld into a building).

## Technologies
-   **Godot Engine**
-   **GDScript**
-   **Godot Scene System**

## Features
-   **Grid-Based Movement**: Precise player movement synchronized with animations for an authentic retro feel.
-   **Scene Management**: A centralized system to handle fading and switching between different game locations.
-   **Interactive Environment**:
    -   **Tall Grass**: Detection system for player entry, capable of triggering wild encounter logic.
    -   **Doors/Portals**: Automated teleports between scenes when the player interacts with specific entry points.

## How to Run


### Prerequisites

-   **Godot Engine 3.x or 4.x** (depending on the specific project version) installed.
    

### Step-by-Step Instructions

1.  **Clone or Download** the repository to your local machine.
2.  **Open Godot Engine** and select "Import".
3.  **Navigate to the folder** containing the `project.godot` file and select it.
4.  **Press F5** or the "Play" button in the top right corner to run the project.

## Project Structure

-   **`Player.gd`**: Handles input, movement logic, and player-state animations.
-   **`SceneManager.gd`**: Manages global transitions and scene loading with transition effects.
-   **`Door.gd`**: Script for interactive objects that transport the player to new coordinates or scenes.
-   **`TallGrass.gd`**: Manages the logic for when a player steps into encounter zones.

## What I Learned

-   **State Management**: Using GDScript to manage complex player states (moving, idling, interacting).
-   **Signal Implementation**: Utilizing Godot's signal system for communication between environment objects (like grass or doors) and the main game logic.
-   **Singleton Patterns**: Implementing the `SceneManager` as an Autoload (Singleton) to maintain state during scene changes.

## Future Improvements

-   **Turn-Based Battle System**: Implement a complete combat interface and monster stats logic.
-   **Inventory & Party Menu**: Create a UI system for managing items and caught creatures.
-   **NPC Dialogue**: Add an interaction system for talking to non-playable characters with text boxes.




