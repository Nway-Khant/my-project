# Module 3 project 3rd of 5

## 1. Player and Enemy Initialization:
The code initializes variables representing the player's robot <code>(playerName, playerHealth, playerAttack, playerMoney)</code> and multiple enemy robots <code>(enemyNames, enemyHealth, enemyAttack)</code>.

## 2. Fight Function:
- The <code>fight</code> function takes an <code>enemyName</code> parameter and simulates a battle between the player's robot and a single enemy robot.
- It continues to loop while both the player and the enemy have health <code>(playerHealth > 0 && enemyHealth > 0)</code>.
- Inside the loop, it prompts the player to choose whether to fight or skip the battle.
Depending on the player's choice, it either proceeds with the battle or skips it, adjusting player's health and money accordingly.
- The loop ends when either the player or the enemy loses all their health.

## 3. Main Game Loop:
- The <code>startGame</code> function serves as the main game loop.
- It resets the player's stats at the beginning of each game.
- It iterates over each enemy robot in the <code>enemyNames</code> array, allowing the player to fight each one sequentially.
- After each battle, it checks if the player is still alive and if there are more enemies to fight.
- If the player is still alive and there are more enemies, it prompts the player to visit a shop to buy health refills or attack upgrades.
- If the player loses all their health or there are no more enemies, it ends the game and asks if the player wants to play again.

## 4. Shop Function:
- The <code>shop</code> function allows the player to spend their money to refill their health or upgrade their attack.
- It prompts the player to choose between refilling health, upgrading attack, or leaving the store.
- Depending on the player's choice, it adjusts the player's stats and money accordingly.

## 5. End Game Function:
- The <code>endGame</code> function displays a message indicating the end of the game and whether the player won or lost.
- It prompts the player if they want to play again and restarts the game if they choose to do so.

## 6. Start Game:
- The <code>startGame()</code> function is called at the end to start the first game when the page loads.