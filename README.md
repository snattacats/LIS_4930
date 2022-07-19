# Choose Your Own Adventure Text Game (Untitled)

### Summary
This is small choose your own adventure game where the choices you make impact your character and future events. This game encourages replayability as you can take multiple paths through the game. Whatever path you choose will eventually meet up at the end, but the journey to get their will be different depending on your choices.

### Setting
The setting takes place in a fictional/fantasy land set in a time period of medieval times. 

### Gameplay
The gameplay consists of reading the text and making a choice from the prompt given. The player starts out with creating a character, the character can be randomly generated for quick ease of use. If the player wants a randomly generated character type the word "random" when prompted. Doing so will generate a random name, age, weight, and gender. Conversely the player can type "custom" when prompted to manually set these details. All other character's details have been pre-defined/pre-randomized by the author. The age, weight, and gender details will affect events in the game. At anytime the player is prompted to type a choice, the player can instead type "player" to see all current stats/detail about their character, in order to make a more informed decision. If the player were to die, the program will end and must be started again, causing the player to start over from the beginning.

----


## File Descriptions


### Main and main.py
The main folder and file consist of the heart of this project. Here all entire story/adventure has been written and allocated properly into branching paths. At the top contains imported packages I have made as well as pre-made ones. It also predefines the user as new_player and uses the p_class class' attributes needed to finish creating a character.

### Names and Name_Gen.py
The Names folder is a package I made for, right now, generating random names. In the Name_Gen.py file, I have made 3 list for a first, middle, and last syllable; each of these lists contain short 2-4 letter strings that when combined will make somewhat of a name. The random_name() function I made, is defined by first setting a variable 'name' to an empty string, afterwards a random number between 1,4 is selected and depending on the number will either make a 3 or 4 syllable word for the random name using 1 random string from each of the 3 lists respectively. In the case of a 4 syllable name, the middle_syl twice. This package uses the random package as well.

### Player and p_class.py
The Player folder holds the class needed to keep track of the player character's stats. The p_class.py file imports the Names package and random package for use. The class is defined as Player and contains 6 different attributes or stats for the player character. __init__() function houses the frame work of the player class, while the player_stats() function is used to display all the character's information/stats when called by the player by typing "player" into the prompt. The create_player_random() function is called when the player decides to use a random character creation by typing "random" into the prompt. The function sets all Player class attributes with a pre-defined stat or randomly chosen one. Only the age, weight, name, gold and gender is randomized; Attack Power and health are pre-defined. The create_player() function, functions the same way but instead of randomized stats the player will be able to enter their own. This only applies to the name, age, weight, and gender stats. Gold will still be randomized and attack power and health will still be pre-defined.

----


## Notes

I tried my best to set error checks and have a coherent story that makes sense even after actions the player makes. I tripled checked for grammar and spelling mistakes, but I'm sure I missed some so I apologize. As of right now, the program does not run on another interface or GUI platform, only within python's console. In the future I will learn how to implement this. Please have fun playing I made this as a project for a class, but it has a lot of love in it because I love these types of games myself.
