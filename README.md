**This isn't the final version of this small project i've done. Sadly i lost the final one so this one will have to do.**

A short first-person shooter game developed using Unity and C#.

The player must navigate through a labyrinth, encounter hostile enemies, and eliminate all of them to complete the objective.

The project focuses on implementing shooting mechanics, weapon interactions, enemy behavior, and animations primarily through code.

Gameplay Features:

  Weapon System

    Two available weapons: Pistol and Rifle.

    Players can pick up and drop weapons throughout the game.

    Each weapon has its own shooting characteristics, including different fire rates and recoil.

    Shooting and reloading animations are primarily implemented through C# code.

  Health and Ammo

    Remaining ammo is diplayed

    Health bar is displayed and it changes colors the lower it is.

  Enemy AI

    Enemies have multiple behavior modes, allowing them to react differently depending on the situation.

  The enemies use a Finite State Machine (FSM) implemented in C# to control their behavior. Each enemy can transition between four different states depending on the player's position, visibility, and combat conditions.

AI States

    Idle — The enemy remains stationary for a certain period before resuming patrol.

    Patrolling — The enemy moves between predefined patrol points, occasionally stopping.

    Chasing — When the player is detected, the enemy pursues their last known position.

    Attacking — When the player is visible and within attack range, the enemy stops moving and begins shooting.

Technical Implementation

    Unity NavMeshAgent handles enemy movement and pathfinding through the labyrinth.

    Physics.Raycast is used to detect whether the enemy has a clear line of sight to the player.

    Last-known-position tracking allows enemies to pursue the player's previously detected location.

    Health-based behavior influences transitions between attacking and patrolling.

    Shooting mechanics include configurable fire rates, randomized bullet spread, muzzle flashes, and sound effects.

    Damage feedback temporarily changes the enemy's material when hit.


  Implemented behaviors include:

    Patrolling — Enemies move around their environment.

    Shooting — Enemies engage the player in combat.

    Retreating — Enemies can retreat during encounters.

Game Environment

    A labyrinth-style level designed for exploration and combat.

<img width="2560" height="1234" alt="Screenshot 2026-11-09 142910" src="https://github.com/user-attachments/assets/f845336b-1013-4226-a911-f26d3cc6252e" />
