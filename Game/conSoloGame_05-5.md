# Module 3 project 5th of 5

## 1. Random Number Generation Function (randomNumber):

- This function generates a random integer between a given <code>min</code> and <code>max</code> value using the <code>Math.random()</code> function.
- It multiplies the result of <code>Math.random()</code> by the difference between <code>max</code> and <code>min</code>, adds <code>min</code>, and then uses <code>Math.floor()</code> to round down to the nearest integer.

## 2. Function to Check if Player Wants to Fight or Skip (fightOrSkip):

- This function prompts the player to choose whether they want to fight or skip the battle.
- If the player chooses to skip, it confirms their decision and deducts 10 units of money (if available) from the player's account.
- It returns <code>true</code> if the player chooses to skip and <code>false</code> otherwise.

## 3. Fight Function (fight):

- This function simulates a battle between the player and an enemy.
- It keeps track of whose turn it is to attack using the <code>isPlayerTurn</code> variable.
- Inside a while loop, it continues the battle until either the player or the enemy's health drops to 0.
- During each turn, it prompts the player to choose whether to fight or skip using the <code>fightOrSkip</code> function.
- It calculates the damage dealt based on the attacker's attack power and applies it to the opponent's health.
- It alternates between the player's and the enemy's turns until the battle concludes.

## 4. Function to Start a New Game (startGame):

- This function resets the player's stats at the beginning of each game.
- It iterates through each enemy in the <code>enemyInfo</code> array, allowing the player to fight them one by one.
- It prompts the player to visit the shop after each battle if they are still alive.
- If the player loses all their health or defeats all the enemies, it calls the <code>endGame</code> function.

## 5. Function to End the Entire Game (endGame):

- This function displays the end-game message, including the player's score and whether they achieved a new high score.
- It prompts the player if they want to play again and restarts the game if they choose to do so.

## 6. Shop Function (shop):

- This function prompts the player to choose between refilling their health, upgrading their attack, or leaving the store.
- Depending on the player's choice, it calls the respective methods in the <code>playerInfo</code> object to refill health or upgrade attack.

## 7. Function to Get Player's Name (getPlayerName):

- This function prompts the player to enter their robot's name.
- It continues to prompt the player until they provide a non-empty and non-null name.
- It returns the player's name.

## 8. Player and Enemy Information:

- Information about the player (such as name, health, attack, and money) is stored in the <code>playerInfo</code> object.
- Information about enemy robots is stored in the <code>enemyInfo</code> array, with each enemy represented as an object containing their name and attack power.

## 9. Run Game:

- The game starts by calling the <code>startGame</code> function, initiating the game loop and prompting the player to fight enemies sequentially.
