# Nostalgic Game (Tokyo)

A 2D pixel-art platformer for iOS, built in Swift with **SpriteKit** and **GameplayKit** for the Apple Developer Academy's *Challenge 6*. You play as a character running through ghost-haunted levels, collecting items, dodging spikes and facing a Ghost King boss.

## Features

- **Platforming controls:** run, jump and wall slide, driven by a player state machine (idle, run, jump, wall slide, eating, death).
- **Two levels** built with SpriteKit tile maps, plus a debug level for testing.
- **Enemies:** wandering ghosts that can be made dizzy, and a boss (the Ghost King) with idle, dash and pause behaviors.
- **Items and events:** keys, chests, pickaxe and stones, with an inventory and checkpoints.
- **Hazards:** spikes, deep-end pits and temporary blocks.
- **Dialogue and tutorial:** text boxes triggered by in-world events, signs and a jump tutorial.
- **UI and flow:** start scene, pause pop-up, restart button, game over and success scenes.
- **Audio:** background music and an audio manager.

## Architecture

The game follows an **entity–component** design on top of GameplayKit:

| Folder | Contents |
| --- | --- |
| `Entity/` | Game objects: player, ghosts, boss, items, spikes, tiles, signs, event triggers, and an entity manager |
| `Components/` | Reusable behaviors: movement, jump, physics, animation, inventory, message, wander, killable, temporary lifetime |
| `States/` | Player and ghost state machines |
| `Boss/` | Ghost King entity and movement states |
| `Scenes/`, `Nodes/` | Start, menu, game over and success scenes, text dialogue |
| `Stage02/` | Level 2 and the tile map assets |
| `Tools/` | Extensions for physics masks, sprite nodes, textures and tile maps |

## Tech stack

![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white) ![SpriteKit](https://img.shields.io/badge/SpriteKit-000000?style=for-the-badge&logo=apple&logoColor=white) ![GameplayKit](https://img.shields.io/badge/GameplayKit-FF9500?style=for-the-badge&logo=apple&logoColor=white) ![Xcode](https://img.shields.io/badge/Xcode-147EFB?style=for-the-badge&logo=xcode&logoColor=white)

## Running the project

Requirements: Xcode and an iPhone or simulator running **iOS 16.5 or later**.

1. Clone the repository:
   ```bash
   git clone https://github.com/Luan-Aiezza/Nostalgic_Game.git
   ```
2. Open `Tokyo/Tokyo.xcodeproj` in Xcode.
3. Select an iPhone simulator or device and press **Run** (⌘R).

## Team

Developed by [Luan Aiezza](https://github.com/Luan-Aiezza), Jessica Souza and Cecilia Maia Guimaraes.
