# Role_Playing_Game
HTML:
	• Step 1:
Create your HTML boilerplate. 
Add a title element and use the text RPG - Dragon Repeller.
Create a div element with id set to game within your body.

	• Step 2:
Create four div elements within your #game element. Give them the following respective id values, in order: stats, controls, monsterStats, and text

	• Step 3:
Create three span elements within your #stats element. Give each of them the class stat. Then give the first one the text XP: 0, the second one the text Health: 100, and the third one the text Gold: 50.

	• Step 4:
Wrap the numbers 0, 100, and 50 in span elements, and wrap those new span elements in strong elements. Then give your new span elements id values of xpText, healthText, and goldText, respectively.

	• Step 5:
For your #controls element, create three button elements. The first should have the id set to button1, and the text Go to store. The second should have the id set to button2, and the text Go to cave. The third should have the id set to button3, and the text Fight dragon.

	• Step 6:
Similar to your #stats element, your #monsterStats element needs two span elements. Give them the class stat and give the first element the text Monster Name: and the second the text Health: . After the text in each, add a strong element with an empty nested span element. Give the first inner span element an id of monsterName and the second inner span element an id of monsterHealth.

	• Step 7:
Give your #text element the following text:

Welcome to Dragon Repeller. You must defeat the dragon that is preventing people from leaving the town. You are in the town square. Where do you want to go? Use the buttons above.


CSS:
	• Step 8:
give the body a background-color set to #0a0a23.

	• Step 9:
Give the #text element a background-color of #0a0a23, a color of #ffffff, and 10px of padding on all sides.

	• Step 10:
Give your #game a maximum width of 500px and a maximum height of 400px. Set the background-color to #ffffff and the color to #ffffff.
Use margins to center it by setting the top margin to 30px, bottom margin to 0px, and the left and right margin to auto.
Finally, give it 10px of padding on all four sides.

	• Step 11:
Using a selector list give both your #controls and #stats elements a border of 1px solid #0a0a23, a #0a0a23 text color, and 5px of padding.

	• Step 12:
Give your #monsterStats element the same border and padding as your #stats element. Set its color to #ffffff and give it a #c70d0d background.

	• Step 13:
For now, hide your #monsterStats element with the display property. Do not change any of the other styling.

	• Step 14:
Give your .stat elements a padding-right of 10px.

	• Step 15:
Add some styles for your buttons. Start by setting the cursor property to pointer. Then set the text color to #0a0a23 and the background-color to #feac32.
Then set the background-image property to linear-gradient(#fecc4c, #ffac33). Lastly, set the border to 3px solid #feac32.


HTML (Checking/Debugging):
	• Step 16:
Create an empty script element.

	• Step 17:
The developer console will include errors that are produced by your code, but you can also use it to see values of variables in your code, which is helpful for debugging.
Add a console.log("Hello World"); line between your script tags. Then click the "Console" button to open the console. You should see the text Hello World.

	• Step 18:
After testing, remove your console.log("Hello World"); line. Then give your now empty script element a src attribute set to ./script.js.


JavaScript:
	• Step 19:
Add your console.log("Hello World"); line to this file, and see it appear in your console.

	• Step 20:
If displayed on you console, remove your console.log("Hello World"); line to begin writing your project code.
Declare a variable called xp.

	• Step 21:
Variables can be assigned a value. When you do this while you declare it, this is called initialization. Initialize your xp variable to have a value of 0, a number.

	• Step 22:
Initialize another variable called health with a value of 100, and a variable called gold with a value of 50

	• Step 23:
Create another variable called currentWeapon and set it to 0.

	• Step 24:
Ensure all your variables are with let.

	• Step 25:
Declare a variable called fighting but do not initialize it with a value.

	• Step 26:
Declare two more variables named monsterHealth and inventory, but do not initialize them.

	• Step 27:
Assign the inventory variable to have the value of stick.

	• Step 28:
The player's inventory in your game will be able to hold multiple items. You will need to use a data type that can do this. An array can be used to hold multiple values.
Change your inventory variable to be an array with the strings stick, dagger, and sword.

	• Step 29:
For now, you want the player to start with just the stick. Change the inventory array to have stick as its only value.

	• Step 30:
Create a button1 variable and use querySelector() to assign it your element with the id of button1. Remember that CSS id selectors are prefixed with a #.

	• Step 31:
Debugging; Check if code is running smoothly on all ends (HTML, CSS and JS).

	• Step 32:
button1 variable to be declared with the const keyword.

	• Step 33:
Use querySelector() to get the other two button elements using their ids: button2 and button3. Store them in variables called button2 and button3. Remember to use const.

	• Step 34:
Just like you did with the buttons, create variables for the following ids and use querySelector() to give them the element as a value:
text, xpText, healthText, goldText, monsterStats, and monsterName.

	• Step 35:
Use querySelector() to get the #monsterHealth element. Because you have already declared a monsterHealth variable earlier, you need to use a different variable name for this element.
Declare a new variable with the const keyword and name it monsterHealthText.

	• Step 36:
Functions are special tools that allow you to run sections of code at specific times. You can declare functions using the function keyword. Here is an example of a function called functionName - note the opening and closing curly braces. These indicate the section of code that is within the function.
Create an empty function named goStore.

	• Step 37:
For now, make your goStore function output the message Going to store. to the console.

	• Step 38:
Create a goCave function that prints Going to cave. to the console.

	• Step 39:
Create a fightDragon function that prints Fighting dragon. to the console.

	• Step 40:
Comments allow you to add notes to your code. In JavaScript, single-line comments can be written with // and multi-line comments can be written with /* and */.
Add a single-line comment that says initialize buttons.

	• Step 41:
button1 represents your first button element. These elements have a special property called onclick, which you can use to determine what happens when someone clicks that button.

You can access properties in JavaScript a couple of different ways. The first is with dot notation.

Use dot notation to set the onclick property of your button1 to the function reference of goStore.

	• Step 42:
Using the same syntax, set the onclick properties of button2 and button3 to goCave and fightDragon respectively.

Once you have done that, open your console and try clicking the buttons on your project.

	• Step 43:
The innerText property controls the text that appears in an HTML element. 

When a player clicks your Go to store button, you want to change the buttons and text. Remove the code inside the goStore function and add a line that updates the text of button1 to say Buy 10 health (10 gold).

	• Step 44:
Add a line that updates the text of button2 to say Buy weapon (30 gold) and update the text of button3 to say Go to town square.

	• Step 45:
You will also need to update the functions that run when the buttons are clicked again.

In your goStore() function, update the onclick property for each button to run buyHealth, buyWeapon, and goTown, respectively.

	• Step 46:
Now you need to modify your display text. Change the innerText property of the text to be You enter the store..

	• Step 47:
Create three new empty functions called buyHealth, buyWeapon, and goTown.

	• Step 48:
Move your goTown function above your goStore function. Then copy and paste the contents of the goStore function into the goTown function.

	• Step 49:
In your goTown function, change your button elements' innerText properties to be Go to store, Go to cave, and Fight dragon. Update your onclick properties to be goStore, goCave, and fightDragon, respectively.

Finally, update innerText property of your text to be You are in the town square. You see a sign that says Store..

	• Step 50:
You need to wrap the text Store in double quotes. Because your string is already wrapped in double quotes, you'll need to escape the quotes around Store. You can escape them with a backslash \.

	• Step 51:
You have repetition in the goTown and goStore functions. When you have repetition in your code, this is a sign that you need another function. Functions can take parameters, which are values that are given to the function each time it is run. Here is a function that takes a parameter called param

Create an empty update function that takes a parameter called location.

	• Step 52:
Create a variable called locations and set it to an empty array.

	• Step 53:
Add an empty object to your locations array.

	• Step 54:
Object properties are written as key: value pairs, where key is the name of the property (or the key), and value is the value that property holds.

Add a name property to your empty object and give it a value of town square.

	• Step 55:
Just like array values, object properties are separated by a comma. Add a comma after your name property and add a button text property with the value of an empty array.

	• Step 56:
Give your empty button text array three string elements. Use the three strings being assigned to the button innerText properties in the goTown function. Remember that array values are separated by commas.

	• Step 57:
Create another property in your object called button functions. Give this property an array containing the three functions assigned to the onclick properties in the goTown function. 

	• Step 58:
Add one final property to the object named text. Give this property the same string value as the one assigned to text.innerText in the goTown function.

	• Step 59:
Add a second object to your locations array. Following the pattern you used in the first object, create the same properties but use the values from the goStore function. Set the name property to store.

	• Step 60:
Now you can consolidate some of your code. Start by copying the code from inside the goTown function and paste it into your update function. Then, remove all the code from inside the goTown and goStore functions.

	• Step 61:
Inside the goTown function, call the update function.

	• Step 62:
You now need to pass the location argument into the update call. 

	• Step 63:
Pass in only the first element of the locations array by adding [0] at the end of the variable. 

	• Step 64:
Now your update function needs to use the argument you pass into it.

	• Step 65:
location["button text"] is an array with three elements. Change the button1.innerText assignment to be the first element of that array instead.

	• Step 66:
Update button2.innerText and button3.innerText to be assigned the second and third values of the button text array, respectively.

	• Step 67:
Following the same pattern as you did for the button text, update the three buttons' onclick assignments to be the first, second, and third values of the button functions array.

	• Step 68:
Update the text.innerText assignment to equal the text from the location object. However, instead of using bracket notation, use dot notation.

	• Step 69:
Update your goStore function to call the update function. Pass the second element of the locations array as your argument.

	• Step 70:
Create two more empty functions named fightSlime and fightBeast. These functions will be used in your upcoming cave object.

	• Step 71:
Add a third object to the locations array. Give it the same properties as the other two objects.

Set name to cave. Set button text to an array with the strings Fight slime, Fight fanged beast, and Go to town square. Set the button functions to an array with the variables fightSlime, fightBeast, and goTown. Set the text property to You enter the cave. You see some monsters..

	• Step 72:
Now that you have a cave location object, update your goCave function to call update and pass that new cave location. Remember that this is the third element in your locations array.

	• Step 73:
Now that your store and cave locations are complete, you can code the actions the player takes at those locations. Inside the buyHealth function, set gold equal to gold minus 10.

	• Step 74:
After the gold is updated, add a line to set health equal to health plus 10.

	• Step 75:
Update both lines inside your buyHealth function to use compound assignment.

	• Step 76:
Now that you are updating the gold and health variables, you need to display those new values on the game screen.

After your assignment lines, assign the innerText property of goldText to be the variable gold. Use the same pattern to update healthText with the health variable.

	• Step 77:
What if the player doesn't have enough gold to buy health? When you want to run code conditionally, you can use the if statement. Put all of the code in your buyHealth function inside an if statement.
For now, the if statement condition should be set to the string condition as a placeholder.

	• Step 78:
Change the if statement condition to check if gold is greater than or equal to 10.

	• Step 79:
Now when a player tries to buy health, it will only work if they have enough money. If they do not, nothing will happen. Add an else statement where you can put code to run if a player does not have enough money.

	• Step 80:
Inside the else statement, set text.innerText to equal You do not have enough gold to buy health..

	• Step 81:
Use const to create a weapons variable above your locations array. Assign it an empty array.

	• Step 82:
Just like your locations array, your weapons array will hold objects. Add four objects to the weapons array, each with two properties: name and power. The first should have the name set to stick and the power set to 5. The second should be dagger and 30. The third, claw hammer and 50. The fourth, sword and 100.

	• Step 83:
Inside your buyWeapon function, add an if statement to check if gold is greater than or equal to 30.

	• Step 84:
Similar to your buyHealth function, set gold equal to 30 less than its current value.

	• Step 85:
The value of the currentWeapon variable corresponds to an index in the weapons array. The player starts with a stick, since currentWeapon starts at 0 and weapons[0] is the stick weapon.

In the buyWeapon function, use compound assignment to add 1 to currentWeapon - the user is buying the next weapon in the weapons array.

	• Step 86:
Change your currentWeapon assignment to use the increment operator.

	• Step 87:
Now update the goldText element to display the new value of gold, and update the text element to display You now have a new weapon..

	• Step 88:
You should tell the player what weapon they bought. In between the two lines you just wrote, use let to initialize a new variable called newWeapon. Set this to equal weapons.

	• Step 89:
Use bracket notation to access an object within the weapons array and assign it to your newWeapon variable. Place the variable currentWeapon within the brackets.

	• Step 90:
weapons[currentWeapon] is an object. Use dot notation to get the name property of that object.

	• Step 91:
You can insert variables into a string with the concatenation operator +. Update the You now have a new weapon. string to say You now have a and the name of the new weapon. Remember to end the sentence with a period.

	• Step 92:
Back at the beginning of this project, you created the inventory array. Add the newWeapon to the end of the inventory array using the push() method.

	• Step 93:
Add the string In your inventory you have: - include the spaces at the beginning and the end.

	• Step 94:
At the end of the second text.innerText string you just added, use the concatenation operator to add the contents of inventory to the string.

	• Step 95:
You do not have enough gold to buy a weapon.

	• Step 96:
Once a player has the best weapon, they cannot buy another one. Wrap all of the code in your buyWeapon function inside another if statement. The condition should check if currentWeapon is less than 3 - the index of the last weapon.

	• Step 97:
Arrays have a length property that returns the number of items in the array. You may want to add new values to the weapons array in the future.

Change your if condition to check if currentWeapon is less than the length of the weapons array. An example of checking the length of an array myArray would look like myArray.length.

	• Step 98:
You now have an error to fix. The currentWeapon variable is the index of the weapons array, but array indexing starts at zero. The index of the last element in an array is one less than the length of the array.

Change the if condition to check weapons.length - 1, instead of weapons.length.

	• Step 99:
Add an else statement for your outer if statement. Inside this new else statement, set text.innerText to You already have the most powerful weapon!.

	• Step 100:
Once a player has the most powerful weapon, you can give them the ability to sell their old weapons.

In the outer else statement, set button2.innerText to Sell weapon for 15 gold. Also set button2.onclick to the function name sellWeapon.

	• Step 101:
Create an empty sellWeapon function.

	• Step 102:
Players should not be able to sell their only weapon. Inside the sellWeapon function, add an if statement with a condition that checks if the length of the inventory array is greater than 1.

	• Step 103:
Inside the if statement, set gold equal to 15 more than its current value. Also update goldText.innerText to the new value.

	• Step 104:
Use the let keyword to create a variable named currentWeapon. Don't assign it a value yet.

	• Step 105:
The shift() method on an array removes the first element in the array and returns it. Use this method to take the first element from the inventory array and assign it to your currentWeapon variable.

	• Step 106:
After your currentWeapon, use the concatenation operator to set text.innerText to the string You sold a , then currentWeapon, then the string ..

	• Step 107:
Now use the += operator to add the string In your inventory you have: and the contents of inventory to the text.innerText. Make sure to include the space at the beginning and end of the In your inventory you have: string.

	• Step 108:
Use an else statement to run when the inventory length is not more than one. Set the text.innerText to say Don't sell your only weapon!.

	• Step 109:
Below your weapons array, define a monsters variable and assign it an array. Set that array to have three objects, each with a name, level, and health properties. The first object's values should be slime, 2, and 15, in order. The second should be fanged beast, 8, and 60. The third should be dragon, 20, and 300.

	• Step 110:
Fighting each type of monster will use similar logic. Create an empty function called goFight to manage this logic

	• Step 111:
In your fightSlime function, set fighting equal to 0 - the index of slime in the monsters array. Remember that you already declared fighting earlier in your code, so you do not need let or const here.
On the next line, call the goFight function.

	• Step112:
Following the same pattern, use that code in the fightBeast and fightDragon functions. Remember that beast is at index 1 and dragon is at index 2. Also, remove the console.log call from your fightDragon function.

	• Step 113:
At the end of your code, create two empty functions named attack and dodge.

	• Step 114:
Add a new object to the end of the locations array, following the same properties as the rest of the objects. Set name to fight, button text to an array with Attack, Dodge, and Run, button functions to an array with attack, dodge, and goTown, and text to You are fighting a monster..

	• Step 115:
In the goFight function, call your update function with the fourth object in locations as an argument.

	• Step 116:
Below your update call, set the monsterHealth to be the health of the current monster. You can get this value by accessing the health property of monsters[fighting] with dot notation.

	• Step 117:
The HTML element that shows the monster's stats has been hidden with CSS. Display the monsterStats element by updating the display property of the style property to block. 

	• Step 118:
Now, set the innerText property of monsterName to be the name property of the current monster. Do the same for monsterHealthText and the health property.

	• Step 119:
Now you can build the attack function. First, update the text message to say The <monster name> attacks., replacing <monster name> with the name of the monster. 

	• Step 120:
On a new line, add the string You attack it with your <weapon>. to the text value, replacing <weapon> with the player's current weapon.

	• Step 121:
Next, set health to equal health minus the monster's level. 

	• Step 122:
Set monsterHealth to monsterHealth minus the power of the player's current weapon. Remember you have the currentWeapon variable and the power property.

	• Step 123:
this generates a random number between 1 and 5: Math.floor(Math.random() * 5) + 1;.
Following this pattern, use the addition operator (+) to add a random number between 1 and the value of xp to your monsterHealth -= weapons[currentWeapon].power.

	• Step 124:
Update healthText.innerText and monsterHealthText.innerText to equal health and monsterHealth.

	• Step 125:
Add an if statement to check if health is less than or equal to 0. If it is, call the lose function.

	• Step 126:
At the end of your if statement, add an else if statement to check if monsterHealth is less than or equal to 0. In your else if, call the defeatMonster function.

	• Step 127:
At the end of your code, create the defeatMonster and lose functions. Leave them empty for now.

	• Step 128:
Inside the dodge function, set text.innerText equal to the string You dodge the attack from the <monster>. Replace <monster> with the name of the monster, using the name property.

	• Step 129:
In your defeatMonster function, set gold equal to gold plus the monster's level times 6.7. You can get the monster's level with the level property.

Here is an example of setting num to num plus 5 * 8: num += 5 * 8. Use Math.floor() to round the result down.

	• Step 130:
Set xp to xp plus the monster's level.

	• Step 131:
Now update goldText and xpText to display the updated values.

	• Step 132:
Finish the defeatMonster function by calling the update function with locations[4] as the argument.

	• Step 133:
Your locations array doesn't have a fifth element, so locations[4] doesn't work.
Add a new object at the end of the locations array, following the same structure as the other objects. Set name to kill monster, set button text to an array with three Go to town square strings, set button functions to an array with three goTown variables, and set text to The monster screams Arg! as it dies. You gain experience points and find gold..

	• Step 134:
The word Arg! should have quotes around it. Besides escaping quotes, there is another way you can include quotation marks inside a string.

Change the double quotes around the string The monster screams Arg! as it dies. You gain experience points and find gold. to single quotes ', then add double quotes around Arg!.

	• Step 135:
After a monster is defeated, the monster's stat box should no longer display.

On the first line of the update function, use monsterStats.style.display to change the display value to none.

	• Step 136:
In the lose function, call the update function and pass in the sixth object of your locations array. Note that you haven't created this object just yet.

	• Step 137:
At the end of your code, create a restart function. Inside this function, set xp to 0, health to 100, gold to 50, currentWeapon to 0, and set inventory to an array with the string stick.

Also update the innerText properties of goldText, healthText, and xpText to their current values.

Finally, call the goTown() function.

	• Step 138
In the locations array, add another object at the end. Set the name property to lose, set button text to an array with three REPLAY? strings, set button functions to an array with three restart variables, and set text to You die. ☠️. You can copy that text to use the emote.

	• Step 139:
Back to your attack function - inside the else if block, create another if and else statement. If the player is fighting the dragon (fighting would be 2), call the winGame function. Move the defeatMonster() call to the else block.

For this step, you will need to use the strict equality (===) operator to check if fighting is equal to 2. The strict equality operator will check if the values are equal and if they are the same data type.

	• Step 140:
JavaScript has a conditional operator called the ternary operator. This can be used as a one-line if-else statement. The syntax is: condition ? true : false.

Change your new if-else statement to a ternary.

	• Step 141:
After the lose function, create a function called winGame. Inside the winGame function, call the update function and pass in locations[6].

	• Step 142:
Add another object in the locations array. Everything should be the same as the lose object, except the name should be win and the text should be You defeat the dragon! YOU WIN THE GAME! 🎉.

	• Step 143:
Inside your attack function, change your health -= monsters[fighting].level; line to health -= getMonsterAttackValue(monsters[fighting].level);. This sets health equal to health minus the return value of the getMonsterAttackValue function, and passes the level of the monster as an argument.

	• Step 144:
Below your attack function, create an empty function named getMonsterAttackValue. It should take level as a parameter.

	• Step 145:
The attack of the monster will be based on the monster's level and the player's xp. In the getMonsterAttackValue function, use const to create a variable called hit. Assign it the equation (level * 5) - (Math.floor(Math.random() * xp));.

This will set the monster's attack to five times their level minus a random number between 0 and the player's xp.

	• Step 146:
Log the value of hit to the console to use in debugging. Remember that you can do this with console.log().

	• Step 147:
Use the return keyword to return the value of hit at the end of the function.

	• Step 148:
In getMonsterAttackValue, change return hit to a ternary operator that returns hit if hit is greater than 0, or returns 0 if it is not.

	• Step 149:
In your attack function, below the health variable, create an if statement. Set the condition to call the isMonsterHit function.

	• Step 150:
Move your monsterHealth assignment into your if block.

	• Step 151:
Add an else statement to the first if statement inside your attack() function. In the else statement, use the += operator to add the text You miss. to the end of text.innerText.

	• Step 152:
Now create the isMonsterHit function. This will return a boolean value (true or false) to be used in your if statement. Return the result of the comparison Math.random() > .2.

	• Step 153:
The player should hit if either Math.random() > .2 or if the player's health is less than 20.

	• Step 154:
On every attack, there should be a chance that the player's weapon breaks. At the end of the attack function, add an empty if statement with the condition Math.random() <= .1.

	• Step 155:
Use the += operator to add Your <weapon> breaks., with a space in front of Your, to the end of text.innerText. Replace <weapon> with the last item in the inventory array using inventory.pop(), which will remove the last item in the array AND return it so it appears in your string.

	• Step 156:
Decrement the value of currentWeapon in your if statement, after you update the text.

	• Step 157:
Use the logical AND operator && to add a second condition to your if statement. The player's weapon should only break if inventory.length does not equal (!==) one.

	• Step 158:
Now you can add a small easter egg (hidden feature) to your game.

Create a new function called easterEgg which calls the update function with locations[7] as the argument.

	• Step 159:
Create an empty pick function with a parameter named guess.

	• Step 160:
Create two new functions named pickTwo and pickEight.

Inside each of those, call the pick() function and pass either 2 or 8 as the argument depending on the function name.

	• Step 161:
Add another object to your locations array. Set name to easter egg, set button text to an array with the strings 2, 8, and Go to town square?, set button functions to an array with the variables pickTwo, pickEight, and goTown, and text to You find a secret game. Pick a number above. Ten numbers will be randomly chosen between 0 and 10. If the number you choose matches one of the random numbers, you win!.

	• Step: 162:
Inside pick, use const to initialize a variable named numbers and set it to an empty array.

	• Step 163:
After your numbers array, create a while loop.

Your while loop should run while numbers.length is less than 10.

	• Step 164:
Inside your while loop, push a random number between 0 and 10 to the end of the numbers array. You can create this random number with Math.floor(Math.random() * 11).

	• Step 165:
After the while loop, set text.innerText to equal You picked <someGuess>. Here are the random numbers:. Replace <someGuess> with the guess function parameter.

	• Step 166:
At the end of the string, before the final quote, insert the new line escape character \n. This will cause the next part you add to text.innerText to appear on a new line.




With this, your RPG game is complete! You can now play around - can you defeat the dragon?![image](https://github.com/FrankySuazo/Role_Playing_Game/assets/114836913/12a12861-db2a-40c4-8728-41024a71c2de)
