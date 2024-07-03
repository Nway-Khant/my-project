# Module 3 project 1st of 5

## 1. Player and Enemy Initialization:

<pre>
- var playerName = window.prompt("What is your robot's name?");
- var playerHealth = 100;
- var playerAttack = 10;
- var playerMoney = 10;

- var enemyName = "Roborto";
- var enemyHealth = 50;
- var enemyAttack = 12;
</pre>

Here, the code prompts the user to input the name of their robot using <code>window.prompt</code>. It then initializes various attributes for the player (health, attack power, money) and the enemy (name, health, attack power).

## 2. Fight Function Declaration:

<pre>
var fight = function () {
  // Code for fighting...
};
</pre>

This defines a function named <code>fight</code>. Inside this function is the logic for the battle between the player's robot and the enemy robot.

## 3. Fight Logic:

- The <code>fight</code> function begins with displaying a welcome message using <code>window.alert</code>.
- It then prompts the user to choose whether to fight or skip the battle.

### If

- If the user chooses to fight <code>(promptFight === "fight" || promptFight === "FIGHT")</code>:
- The player's attack power is subtracted from the enemy's health.
- The result of the attack is logged to the console and shown to the user via alerts.
- If the enemy's health drops to or below 0, the enemy is considered defeated.<hr>

- The enemy then attacks the player, deducting the player's health accordingly.
- The result of the attack is logged and shown to the user via alerts.
- If the player's health drops to or below 0, the player is considered defeated.<hr>

### else if

- If the user chooses to skip the battle <code>(promptFight === "skip" || promptFight === "SKIP")</code>:
- The user is asked for confirmation.
- If confirmed, a message is displayed indicating that the player has decided to skip the fight, and some money is deducted from the player.
- If not confirmed, the <code>fight</code> function is called again, allowing the user to choose again.<hr>

### else

- If the user inputs an invalid option, they are alerted to pick a valid option.
