# Module 3 project 4th of 5

## 1. Random Number Generation Function:

- The <code>randomNumber</code> function generates a random numeric value between a minimum and maximum value (inclusive). It's used to generate random damage values for attacks.

## 2. Fight Function:

- The <code>fight</code> function simulates a battle between the player's robot and an enemy robot.
- It continues to loop while both the player and the enemy have health greater than 0.
- Inside the loop, it prompts the player to choose whether to fight or skip the battle.
- Depending on the player's choice, it either proceeds with the battle or skips it, adjusting player's health and money accordingly.
- It calculates damage for each attack based on random numbers and updates the health of the player and the enemy accordingly.
- The loop ends when either the player or the enemy loses all their health.

## 3. Main Game Loop:

- The <code>startGame</code> function serves as the main game loop.
- It resets the player's stats at the beginning of each game.
- It iterates over each enemy robot in the <code>enemyInfo</code> array, allowing the player to fight each one sequentially.
- After each battle, it checks if the player is still alive and if there are more enemies to fight.
- If the player is still alive and there are more enemies, it prompts the player to visit a shop to buy health refills or attack upgrades.
- If the player loses all their health or there are no more enemies, it ends the game and asks if the player wants to play again.

## 4. End Game Function:

- The <code>endGame</code> function displays a message indicating the end of the game and whether the player won or lost.
- It prompts the player if they want to play again and restarts the game if they choose to do so.

## 5. Shop Function:

- The <code>shop</code> function allows the player to spend their money to refill their health or upgrade their attack.
- It prompts the player to choose between refilling health, upgrading attack, or leaving the store.
Depending on the player's choice, it adjusts the player's stats and money accordingly.

## 6. Player and Enemy Information:

- Information about the player's robot and the enemy robots is stored in <code>playerInfo</code> and <code>enemyInfo</code> objects, respectively.
- <code>playerInfo</code> contains the player's name, health, attack power, and money, along with methods to reset health, refill health, and upgrade attack.
- <code>enemyInfo</code> is an array of objects, each containing information about an enemy robot, including their name and attack power.

## 7. Console Logs:

- Console logs are used to display information about the enemy robots and their properties.

## 8. Game Start:

- The <code>startGame()</code> function is called at the end to start the first game when the page loads.
