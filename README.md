# Snatch
COMP2501 Project - An puzzle solving escape game!

### Contributors
- Luke Harper
- Nick Chiasson

### Controls
| Key        | Action        |
| ---------- | ------------- |
| w          | Move forward  |
| a          | Strafe left   |
| s          | Move backward |
| d          | Strafe right  |
| MOUSE MOVE | Aim/look      |
| SPACE      | Interact      |
| n          | Next level    |
| r          | Reload level  |

### Objectives and mechanics
The objective of the game is to pass through the exit door in each stage, avoiding enemies and interacting with level components as necessary.

Interactive objects in the game consist of doors, light switches, and levers. Levers unlock doors, and light switches cause the enemies to break from their paths to go turn the lights back on.

With the lights on, enemies can see infinitely in a straight line in front of them until a wall obstructs their view (key phrase here is straight line). However, when the lights are off, enemies can only see a single space in front of themselves.

If you are seen by an enemy, you have 3 seconds to move from their line of sight before you get game over. If you step on the same space as an enemy (ie. get too close), it's an instant game over.

### Notes
When you get a game over, there is currently no visual indication, however you will know immediately because all controls lock. In this case, you are forced to either reload the level or continue to the next level.

The next level and reload level controls are available at any time during the game. As a result, I don't suggest hitting either of them on the menu screen, as I believe this will cause the game to freeze.

Finally, the game contains some memory leak issues and as a result it uses a LOT of memory during execution. Due to this issue, it is possible that one or both of the currently implemented stages will not load on some machines. Instead the game will crash while attempting to load the level.
