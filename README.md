# Role_Playing_Game

	• HTML:
Created HTML boilerplate. 
Add a title element and use the text RPG - Dragon Repeller.
Created a div element with id set to game within body.

Created four div elements within #game element. Give them the following respective id values, in order: stats, controls, monsterStats, and text

Created three span elements within your #stats element. Give each of them the class stat. Then give the first one the text XP: 0, the second one the text Health: 100, and the third one the text Gold: 50.

Wrap the numbers 0, 100, and 50 in span elements, and wrap those new span elements in strong elements. Then gave new span elements id values of xpText, healthText, and goldText, respectively.

For #controls element, create three button elements. The first should have the id set to button1, and the text Go to store. The second should have the id set to button2, and the text Go to cave. The third should have the id set to button3, and the text Fight dragon.

Similar to #stats element, #monsterStats element needs two span elements. Gave them the class stat and give the first element the text Monster Name: and the second the text Health: . After the text in each, add a strong element with an empty nested span element. Give the first inner span element an id of monsterName and the second inner span element an id of monsterHealth.

Give your #text element the following text:

Welcome to Dragon Repeller. You must defeat the dragon that is preventing people from leaving the town. You are in the town square. Where do you want to go? Use the buttons above.

	• CSS:
Gave the body a background-color set to #0a0a23.

Give the #text element a background-color of #0a0a23, a color of #ffffff, and 10px of padding on all sides.

Gave #game a maximum width of 500px and a maximum height of 400px. Set the background-color to #ffffff and the color to #ffffff.
Use margins to center it by setting the top margin to 30px, bottom margin to 0px, and the left and right margin to auto.
Finally, give it 10px of padding on all four sides.

Using a selector list give both #controls and #stats elements a border of 1px solid #0a0a23, a #0a0a23 text color, and 5px of padding.

Give your #monsterStats element the same border and padding as your #stats element. Set its color to #ffffff and give it a #c70d0d background.

For now, hided #monsterStats element with the display property. Did not change any of the other styling.

Gave .stat elements a padding-right of 10px.

Added some styles for buttons. Started by setting the cursor property to pointer. Then set the text color to #0a0a23 and the background-color to #feac32.
Then set the background-image property to linear-gradient(#fecc4c, #ffac33). Lastly, set the border to 3px solid #feac32.

	• HTML (Checking/Debugging):
Create an empty script element.

The developer console will include errors that are produced by the code, but can also use it to see values of variables in the code, which is helpful for debugging.
Add a console.log("Hello World"); line between your script tags. Then click the "Console" button to open the console. You should see the text Hello World.

After testing, removed console.log("Hello World"); line. Then gave now empty script element a src attribute set to ./script.js.

	• JavaScript:
Added console.log("Hello World"); line to this file, and see it appear in the console.

If displayed on the console, removed console.log("Hello World"); line to begin writing the project code.
Declare a variable called xp.

Variables can be assigned a value. When you do this while you declare it, this is called initialization. Initialize your xp variable to have a value of 0, a number.

Initialize another variable called health with a value of 100, and a variable called gold with a value of 50

Create another variable called currentWeapon and set it to 0.

Ensure all variables are with let.

Declare a variable called fighting but do not initialize it with a value.

Declare two more variables named monsterHealth and inventory, but did not initialize them.

Assign the inventory variable to have the value of stick.

The player's inventory in the game will be able to hold multiple items. Will need to use a data type that can do this. An array can be used to hold multiple values.
Changed inventory variable to be an array with the strings stick, dagger, and sword.

For now, wanted the player to start with just the stick. Change the inventory array to have stick as its only value.

Created a button1 variable and use querySelector() to assign it a element with the id of button1. Remember that CSS id selectors are prefixed with a #.

Debugging; Check if code is running smoothly on all ends (HTML, CSS and JS).

button1 variable to be declared with the const keyword.

Use querySelector() to get the other two button elements using their ids: button2 and button3. Store them in variables called button2 and button3. Remember to use const.

Just like with the buttons, created variables for the following ids and use querySelector() to give them the element as a value:
text, xpText, healthText, goldText, monsterStats, and monsterName.

Used querySelector() to get the #monsterHealth element. Because had already declared a monsterHealth variable earlier, needed to use a different variable name for this element.
Declare a new variable with the const keyword and name it monsterHealthText.

Functions are special tools that allow you to run sections of code at specific times. Now could declare functions using the function keyword. Here is an example of a function called functionName - note the opening and closing curly braces. These indicate the section of code that is within the function.
Create an empty function named goStore.

For now, made goStore function output the message Going to store. to the console.

Created a goCave function that prints Going to cave. to the console.

Created a fightDragon function that prints Fighting dragon. to the console.

Comments allow you to add notes to your code. In JavaScript, single-line comments can be written with // and multi-line comments can be written with /* and */.
Add a single-line comment that says initialize buttons.

button1 represents the first button element. These elements have a special property called onclick, which you can use to determine what happens when someone clicks that button.

Now could access properties in JavaScript a couple of different ways. The first is with dot notation.

Used dot notation to set the onclick property of button1 to the function reference of goStore.

Using the same syntax, set the onclick properties of button2 and button3 to goCave and fightDragon respectively.

Once that has been done, open your console and try clicking the buttons on the project.

The innerText property controls the text that appears in an HTML element. 

When a player clicks your Go to store button, wanted to change the buttons and text. Remove the code inside the goStore function and add a line that updates the text of button1 to say Buy 10 health (10 gold).

Add a line that updates the text of button2 to say Buy weapon (30 gold) and update the text of button3 to say Go to town square.

Will also need to update the functions that run when the buttons are clicked again.

In goStore() function, update the onclick property for each button to run buyHealth, buyWeapon, and goTown, respectively.

Now needed to modify your display text. Change the innerText property of the text to be You enter the store..

Created three new empty functions called buyHealth, buyWeapon, and goTown.

Moved goTown function above the goStore function. Then copy and paste the contents of the goStore function into the goTown function.

In goTown function, changed button elements' innerText properties to be Go to store, Go to cave, and Fight dragon. Update your onclick properties to be goStore, goCave, and fightDragon, respectively.

Finally, update innerText property of your text to be You are in the town square. You see a sign that says Store..

Needed to wrap the text Store in double quotes. Because string is already wrapped in double quotes, needed to escape the quotes around Store. Can escape them with a backslash \.

Having repetition in the goTown and goStore functions. When having repetition in the code, this is a sign that needs another function. Functions can take parameters, which are values that are given to the function each time it is run. Here is a function that takes a parameter called param

Created an empty update function that takes a parameter called location.

Created a variable called locations and set it to an empty array.

Add an empty object to your locations array.

Object properties are written as key: value pairs, where key is the name of the property (or the key), and value is the value that property holds.

Added a name property to empty object and give it a value of town square.

Just like array values, object properties are separated by a comma. Add a comma after name property and add a button text property with the value of an empty array.

Gave empty button text array three string elements. Use the three strings being assigned to the button innerText properties in the goTown function. Remember that array values are separated by commas.

Create another property in the object called button functions. Gave this property an array containing the three functions assigned to the onclick properties in the goTown function. 

Added one final property to the object named text. Give this property the same string value as the one assigned to text.innerText in the goTown function.

Added a second object to your locations array. Following the pattern used in the first object, created the same properties but use the values from the goStore function. Set the name property to store.

Now can consolidate some of the code. Started by copying the code from inside the goTown function and paste it into the update function. Then, remove all the code from inside the goTown and goStore functions.

Inside the goTown function, call the update function.

Needed to pass the location argument into the update call. 

Pass in only the first element of the locations array by adding [0] at the end of the variable. 

Now updated function needs to use the argument pass into it.

location["button text"] is an array with three elements. Changed the button1.innerText assignment to be the first element of that array instead.

Updated button2.innerText and button3.innerText to be assigned the second and third values of the button text array, respectively.

Following the same pattern as did for the button text, update the three buttons' onclick assignments to be the first, second, and third values of the button functions array.

Updated the text.innerText assignment to equal the text from the location object. However, instead of using bracket notation, use dot notation.

Updated the goStore function to call the update function. Pass the second element of the locations array as the argument.

Created two more empty functions named fightSlime and fightBeast. These functions will be used in the upcoming cave object.

Added a third object to the locations array. Gave it the same properties as the other two objects.

Set name to cave. Set button text to an array with the strings Fight slime, Fight fanged beast, and Go to town square. Set the button functions to an array with the variables fightSlime, fightBeast, and goTown. Set the text property to You enter the cave. You see some monsters..

Now in the cave location object, updated goCave function to call update and pass that new cave location. Remember that this is the third element in your locations array.

Now that store and cave locations are complete, now can code the actions the player takes at those locations. Inside the buyHealth function, set gold equal to gold minus 10.

After the gold is updated, add a line to set health equal to health plus 10.

Updated both lines inside to buyHealth function to use compound assignment.

Now that's updating the gold and health variables, needed to display those new values on the game screen.

After the assignment lines, assigned the innerText property of goldText to be the variable gold. Used the same pattern to update healthText with the health variable.

What if the player doesn't have enough gold to buy health? When you want to run code conditionally, needed to use the if statement. Put all of the code in the buyHealth function inside an if statement.
For now, the if statement condition should be set to the string condition as a placeholder.

Changed the if statement condition to check if gold is greater than or equal to 10.

Now when a player tries to buy health, it will only work if they have enough money. If they do not, nothing will happen. Added an else statement where the code runs if a player does not have enough money.

Inside the else statement, set text.innerText to equal You do not have enough gold to buy health..

Use const to create a weapons variable above your locations array. Assign it an empty array.

Just like he locations array, the weapons array will hold objects. Added four objects to the weapons array, each with two properties: name and power. The first should have the name set to stick and the power set to 5. The second should be dagger and 30. The third, claw hammer and 50. The fourth, sword and 100.

Inside the buyWeapon function, add an if statement to check if gold is greater than or equal to 30.

Similar to buyHealth function, set gold equal to 30 less than its current value.

The value of the currentWeapon variable corresponds to an index in the weapons array. The player starts with a stick, since currentWeapon starts at 0 and weapons[0] is the stick weapon.

In the buyWeapon function, use compound assignment to add 1 to currentWeapon - the user is buying the next weapon in the weapons array.

Change the currentWeapon assignment to use the increment operator.

Now updated the goldText element to display the new value of gold, and update the text element to display You now have a new weapon..

Should tell the player what weapon they bought. In between the two lines just wrote, use let to initialize a new variable called newWeapon. Set this to equal weapons.

Used bracket notation to access an object within the weapons array and assign it to your newWeapon variable. Place the variable currentWeapon within the brackets.

weapons[currentWeapon] is an object. Use dot notation to get the name property of that object.

Inserted variables into a string with the concatenation operator +. Update the You now have a new weapon. string to say You now have a and the name of the new weapon. Remember to end the sentence with a period.

Back at the beginning of this project, created the inventory array. Added the newWeapon to the end of the inventory array using the push() method.

Added the string In your inventory you have: - include the spaces at the beginning and the end.

At the end of the second text.innerText string just added, use the concatenation operator to add the contents of inventory to the string.

You do not have enough gold to buy a weapon.

Once a player has the best weapon, they cannot buy another one. Wrap all of the code in the buyWeapon function inside another if statement. The condition should check if currentWeapon is less than 3 - the index of the last weapon.

Arrays have a length property that returns the number of items in the array. May want to add new values to the weapons array in the future.

Changed if condition to check if currentWeapon is less than the length of the weapons array. An example of checking the length of an array myArray would look like myArray.length.

Now have an error to fix. The currentWeapon variable is the index of the weapons array, but array indexing starts at zero. The index of the last element in an array is one less than the length of the array.

Changed the if condition to check weapons.length - 1, instead of weapons.length.

Added an else statement for outer if statement. Inside this new else statement, set text.innerText to You already have the most powerful weapon!.

Once a player has the most powerful weapon, you can give them the ability to sell their old weapons.

In the outer else statement, set button2.innerText to Sell weapon for 15 gold. Also set button2.onclick to the function name sellWeapon.

Create an empty sellWeapon function.

Players should not be able to sell their only weapon. Inside the sellWeapon function, add an if statement with a condition that checks if the length of the inventory array is greater than 1.

Inside the if statement, set gold equal to 15 more than its current value. Also update goldText.innerText to the new value.

Used the let keyword to create a variable named currentWeapon. Don't assign it a value yet.

The shift() method on an array removes the first element in the array and returns it. Use this method to take the first element from the inventory array and assign it to your currentWeapon variable.

After the currentWeapon, use the concatenation operator to set text.innerText to the string You sold a , then currentWeapon, then the string ..

Now used the += operator to add the string In your inventory you have: and the contents of inventory to the text.innerText. Make sure to include the space at the beginning and end of the In your inventory you have: string.

Used an else statement to run when the inventory length is not more than one. Set the text.innerText to say Don't sell your only weapon!.

Below the weapons array, define a monsters variable and assign it an array. Set that array to have three objects, each with a name, level, and health properties. The first object's values should be slime, 2, and 15, in order. The second should be fanged beast, 8, and 60. The third should be dragon, 20, and 300.

Fighting each type of monster will use similar logic. Create an empty function called goFight to manage this logic

	• Step 111:
In your fightSlime function, set fighting equal to 0 - the index of slime in the monsters array. Remember that you already declared fighting earlier in your code, so you do not need let or const here.
On the next line, call the goFight function.

Following the same pattern, use that code in the fightBeast and fightDragon functions. Remember that beast is at index 1 and dragon is at index 2. Also, remove the console.log call from the fightDragon function.

At the end of the code, create two empty functions named attack and dodge.

Added a new object to the end of the locations array, following the same properties as the rest of the objects. Set name to fight, button text to an array with Attack, Dodge, and Run, button functions to an array with attack, dodge, and goTown, and text to You are fighting a monster..

In the goFight function, call the update function with the fourth object in locations as an argument.

Below the update call, set the monsterHealth to be the health of the current monster. Could get this value by accessing the health property of monsters[fighting] with dot notation.

The HTML element that shows the monster's stats has been hidden with CSS. Display the monsterStats element by updating the display property of the style property to block. 

Now, setted the innerText property of monsterName to be the name property of the current monster. Do the same for monsterHealthText and the health property.

Builded the attack function. First, update the text message to say The <monster name> attacks., replacing <monster name> with the name of the monster. 

On a new line, added the string You attack it with your <weapon>. to the text value, replacing <weapon> with the player's current weapon.

Next, set health to equal health minus the monster's level. 

Set monsterHealth to monsterHealth minus the power of the player's current weapon. The currentWeapon variable and the power property.

This generates a random number between 1 and 5: Math.floor(Math.random() * 5) + 1;.
Following this pattern, use the addition operator (+) to add a random number between 1 and the value of xp to your monsterHealth -= weapons[currentWeapon].power.

Update healthText.innerText and monsterHealthText.innerText to equal health and monsterHealth.

Add an if statement to check if health is less than or equal to 0. If it is, call the lose function.

At the end of if statement, add an else if statement to check if monsterHealth is less than or equal to 0. In your else if, call the defeatMonster function.

At the end of the code, create the defeatMonster and lose functions. Leave them empty for now.

Inside the dodge function, set text.innerText equal to the string You dodge the attack from the <monster>. Replace <monster> with the name of the monster, using the name property.

In the defeatMonster function, set gold equal to gold plus the monster's level times 6.7. Player can get the monster's level with the level property.

Here is an example of setting num to num plus 5 * 8: num += 5 * 8. Use Math.floor() to round the result down.

Set xp to xp plus the monster's level.

Now updated goldText and xpText to display the updated values.

Finish the defeatMonster function by calling the updated function with locations[4] as the argument.

Locations array doesn't have a fifth element, so locations[4] doesn't work.
Added a new object at the end of the locations array, following the same structure as the other objects. Set name to kill monster, set button text to an array with three Go to town square strings, set button functions to an array with three goTown variables, and set text to The monster screams Arg! as it dies. You gain experience points and find gold..

The word Arg! should have quotes around it. Besides escaping quotes, there is another way that can include quotation marks inside a string.

Change the double quotes around the string The monster screams Arg! as it dies. You gain experience points and find gold. to single quotes ', then add double quotes around Arg!.

After a monster is defeated, the monster's stat box should no longer display.

On the first line of the update function, use monsterStats.style.display to change the display value to none.

In the lose function, call the update function and pass in the sixth object of locations array. Note that haven't created this object just yet.

At the end of the code, create a restart function. Inside this function, set xp to 0, health to 100, gold to 50, currentWeapon to 0, and set inventory to an array with the string stick.

Also update the innerText properties of goldText, healthText, and xpText to their current values.

Finally, call the goTown() function.

In the locations array, add another object at the end. Set the name property to lose, set button text to an array with three REPLAY? strings, set button functions to an array with three restart variables, and set text to You die. ☠️. You can copy that text to use the emote.

Back to the attack function - inside the else if block, create another if and else statement. If the player is fighting the dragon (fighting would be 2), call the winGame function. Move the defeatMonster() call to the else block.

For this step, needed to use the strict equality (===) operator to check if fighting is equal to 2. The strict equality operator will check if the values are equal and if they are the same data type.

JavaScript has a conditional operator called the ternary operator. This can be used as a one-line if-else statement. The syntax is: condition ? true : false.

Changed the new if-else statement to a ternary.

After the lose function, created a function called winGame. Inside the winGame function, call the update function and pass in locations[6].

Added another object in the locations array. Everything should be the same as the lose object, except the name should be win and the text should be You defeat the dragon! YOU WIN THE GAME! 🎉.

Inside the attack function, change your health -= monsters[fighting].level; line to health -= getMonsterAttackValue(monsters[fighting].level);. This sets health equal to health minus the return value of the getMonsterAttackValue function, and passes the level of the monster as an argument.

Below the attack function, create an empty function named getMonsterAttackValue. It should take level as a parameter.

The attack of the monster will be based on the monster's level and the player's xp. In the getMonsterAttackValue function, use const to create a variable called hit. Assign it the equation (level * 5) - (Math.floor(Math.random() * xp));.

This will set the monster's attack to five times their level minus a random number between 0 and the player's xp.

Logged the value of hit to the console to use in debugging. Remember that you can do this with console.log().

Use the return keyword to return the value of hit at the end of the function.

In getMonsterAttackValue, change return hit to a ternary operator that returns hit if hit is greater than 0, or returns 0 if it is not.

In the attack function, below the health variable, create an if statement. Set the condition to call the isMonsterHit function.

Move the monsterHealth assignment into the if block.

Added an else statement to the first if statement inside the attack() function. In the else statement, use the += operator to add the text You miss. to the end of text.innerText.

Now create the isMonsterHit function. This will return a boolean value (true or false) to be used in the if statement. Return the result of the comparison Math.random() > .2.

The player should hit if either Math.random() > .2 or if the player's health is less than 20.

On every attack, there should be a chance that the player's weapon breaks. At the end of the attack function, added an empty if statement with the condition Math.random() <= .1.

Used the += operator to add Your <weapon> breaks., with a space in front of Your, to the end of text.innerText. Replace <weapon> with the last item in the inventory array using inventory.pop(), which will remove the last item in the array AND return it so it appears in the string.

Decrement the value of currentWeapon in the if statement, after the update the text.

Use the logical AND operator && to add a second condition to the if statement. The player's weapon should only break if inventory.length does not equal (!==) one.

Added a small easter egg (hidden feature) to your game.

Created a new function called easterEgg which calls the update function with locations[7] as the argument.

Created an empty pick function with a parameter named guess.

Created two new functions named pickTwo and pickEight.

Inside each of those, call the pick() function and pass either 2 or 8 as the argument depending on the function name.

Added another object to your locations array. Set name to easter egg, set button text to an array with the strings 2, 8, and Go to town square?, set button functions to an array with the variables pickTwo, pickEight, and goTown, and text to You find a secret game. Pick a number above. Ten numbers will be randomly chosen between 0 and 10. If the number they choose matches one of the random numbers, they win!.

Inside pick, use const to initialize a variable named numbers and set it to an empty array.

After the numbers array, created a while loop.

While loop should run while numbers.length is less than 10.

Inside the while loop, push a random number between 0 and 10 to the end of the numbers array. Created this random number with Math.floor(Math.random() * 11).

After the while loop, set text.innerText to equal You picked <someGuess>. Here are the random numbers:. Replace <someGuess> with the guess function parameter.

At the end of the string, before the final quote, insert the new line escape character \n. This will cause the next part you add to text.innerText to appear on a new line.




With this, the RPG game is complete! You can now play around - can you defeat the dragon?
