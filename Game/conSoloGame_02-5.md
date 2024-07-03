# Module 3 project 2nd of 5

## 1. Player and Enemy Initialization:

<pre>
var playerName = window.prompt("What is your robot's name?");
var playerHealth = 100;
var playerAttack = 10;
var playerMoney = 10;

var enemyNames = ['Roborto', 'Amy Android', 'Robo Trumble'];
var enemyHealth = 50;
var enemyAttack = 12;
</pre>

This section initializes variables representing the player's robot <code>(playerName, playerHealth, playerAttack, playerMoney)</code> and multiple enemy robots <code>(enemyNames, enemyHealth, enemyAttack)</code>.

## 2. Console Logs and Array Operations:

<pre>
console.log(enemyNames);
console.log(enemyNames.length);
console.log(enemyNames[0]);
console.log(enemyNames[3]);
</pre>

These lines demonstrate console logging and accessing elements of the <code>enemyNames</code> array. enemyNames is an array containing names of different enemy robots. <code>enemyNames.length</code> returns the number of elements in the array. <code>enemyNames[0]</code> accesses the first element of the array, and <code>enemyNames[3]</code> tries to access the fourth element, which doesn't exist (arrays are zero-indexed).

## 3. Fight Function:

<pre>
var fight = function(enemyName) {
  // Fight logic
};
</pre>

This defines a function named <code>fight</code> that takes an <code>enemyName</code> parameter. Inside this function is the logic for the battle between the player's robot and a single enemy robot.

## 4. Main Game Loop:

<pre>
for (var i = 0; i < enemyNames.length; i++) {
  // Main game loop
}
</pre>

This loop iterates over each enemy in the <code>enemyNames</code> array, allowing the player to fight each enemy one at a time.

### Inside the Game Loop:

- The game loop checks if the player's robot is still alive <code>(playerHealth > 0)</code>. If the player is alive, it proceeds to the next enemy. Otherwise, it ends the game.
- For each enemy, the player is informed of the round number and a specific enemy is picked from the <code>enemyNames</code> array.
- The <code>fight</code> function is called, passing the name of the current enemy as an argument.
- After the fight, if the player's robot is not alive <code>(playerHealth <= 0)</code>, the game ends.
