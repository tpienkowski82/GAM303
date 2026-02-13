# GAM 303 – Shadow Run: Data Heist (Alpha)

## Overview
Shadow Run: Data Heist is a single-level stealth prototype built in Unreal Engine 5. The alpha focuses on core functionality: hazards, interactions, and a win/lose condition.

## How to Run
1. Open the project in Unreal Engine 5.
2. Open the Alpha map (set as Game Default Map).
3. Press Play.

## Controls
- WASD: Move
- Mouse: Look
- Interact (E): Pick up objects / collect keycard (if applicable)

## Alpha Gameplay Loop (Milestone Two)
1. Complete the hack puzzle at the terminal to open the secure door.
2. A keycard spawns after the hack succeeds.
3. Pick up the keycard (sets HasKeycard = true).
4. Return to the terminal:
   - If HasKeycard = true and you enter the terminal WinRange → YOU WIN (GameMode HandleWin)
   - If you do not have the keycard → nothing happens

## Hazards / Fail Condition
- Turrets track the player and fire projectiles when in range.
- Detection trigger volume causes a fail state (GameMode HandleFail).

## Test Plan + Traceability
See: docs/GAM303_Traceability_and_TestPlan_Pienkowski.xlsx

## Known Issues / Future Work
- UI/HUD is planned for final submission.
- Visual meshes/materials for terminal/keycard are placeholder primitives for alpha.
