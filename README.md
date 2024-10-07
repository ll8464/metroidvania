Hello!

This is a Single scene metroidvania where you play a small robot! Made with Kaboom! Tutorial assistance from FreeCodeAcademy.

The goal of this project is get practice in setting up scenes, managing state, and implementing controls.

\*If you see a gray checkered scene, just press enter key.

Current Controls:
Left and right arrow keys - move left and right
X - jump
Z - a

Objective - Defeat the boss!

Bug Fix

The Boss would not activate after entering the arena. The solution was to return the if (currentState.playerInBossFight || currentState.isBossDefeated) statement in the roomUtils. It was preventing the playerInBossFight state from be set to true, which
the entire logic of the Boss depend on to activate it's state.
