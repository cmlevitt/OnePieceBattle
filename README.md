# M4OEP-cmlevitt-cyarberr-aajoshi

*****ONE PIECE BATTLE GAME*****
*Callie Levitt, Apoorva Joshi, & Caden Yarberry*

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**CONTEXT:**
One Piece is an anime and manga which has been running for over 25 years. It follows the story of a pirate adventure, and the two
main factions are the pirates and the marines. These two forces are in opposition, but there are also often fights between two pirate 
crews or occasionally within the marine faction. Characters in this series have a variety of abilities, most common being weapons, 
the power of "haki" (based on willpower, can increase a characters powers of observation or defense/strength, among other things), and
"devil fruits" (a magical fruit which gives the person who eats it a power...far to arbitrary and complicated for me to explain fully - 
just take my word for it).

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**PROGRAM SUMMARY**
-Module 4 Concepts:
We utilized Graphics for C++, 8-bit Drawing, Keyboard input, Mouse Input, and multiple screens in a graphics window.
-The game is based off an existing OEP from module 2 by Callie Levitt and Caden Yarberry. This project adds graphics to the existing concept of a One Piece
themed battle game. There are multiple screens which allow user input from the keyboard and mouse clicking buttons, allowing them to either play as a random character or
choose from the main cast of the series. They then get to encounter enemies, and chose to either fight or try to run away, and can attack using a button which they must
click multiple times to generate attack power (confetti!!) There are screens for each action, 

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**FUTURE WORK**
We had some difficulty implementing the sprites, and would love to have a more colorful and dynamic user interface with sprites that move according to the 
users actions, as well as more custom sprites for different characters. We would also want to refine the gameplay further making fights include multiple attacks,
and have some skill (like speed of button clicking) play into the users success in their battle. 

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**CITATIONS**
--This code utilized some starter code which was reworked from the module 1 "Monsters", module 4 "Confetti Button", and 
"Runner" projects, as well as "Graphics Starter" written by Lisa Dion, as well as some file input code reworked from a past Data Structures and
Algorithms project. The rest is self authored!

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**KNOWN BUGS**
-The waves are a little wonky
-One issue is that if you choose a random character and get a strawhat then you can still fight other strawhats which is less of a bug and more just sad because they are friends and shouldn't be fighting

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**GRADE JUSTIFICATION**
We believe we should get over 120 points.
We utilized every concept covered in this module.
• OpenGL is used for graphics and GLFW for all keyboard inputs
• Drawing is used to display all our buttons and battle confetti
• Keyboard input(s) are used to swap between certain screens
• Mouse input(s) are used to click buttons to swap between screens
• Non-input-based event(s) are used on the waves in the beginning to reset them to the left when they go off screen
• Multiple screens in the same graphics window: we have many many screens.
• Graphics with C++ classes

We also implement pixel art for enemy ships (both pirate and marine), the waves at the beginning and a pixelated strawhat jolly roger on the win screen

All code is thoroughly commented and reasonably well arranged/consistent.
It is also quite complex.
We read from two separate files containing character information, turn each of those characters into pirate or marine objects which are both child classes of Player, and then pass those objects into vectors. From there we let the user press s to start the game. Once they start the game they can choose (by clicking a button on screen) to select a character from the original 5 Strawhat pirates (Luffy, Zoro, Nami, Usopp, or Sanji) OR just get a random character. The character they choose becomes the “player” variable and then that character gets removed from the vectors of characters so they cannot fight their own character. If they chose a Strawhat pirate the other Strawhats get removed from the vectors as they are all friends and it would be mean to make them fight. Those vectors then get shuffled so it's a mystery who they will fight every time. After getting a character they have a 50-50 chance to encounter an enemy from the marine or pirate vector. The name of that enemy will be displayed along with a ship of that character’s affiliation type (pirate ship or marine battleship). On this encounter screen there will also be two buttons to FIGHT or RUN if they choose to run there is a 50-50 chance they escape (avoid having to fight the character they encountered, a good choice to make if you know that character is stronger than the one you chose). Otherwise they have to fight. If they fight both Pirate and Marine objects have an Attack they can call which gives them a slightly randomized number based on how strong the character would be. If the player’s attack number is higher they win the fight and move on. Otherwise they lose and have to exit the program. If they win 5 fights though then they get the win screen and win and are happy.
There is also the whole drawing rectangles (Rects which are Shapes) for the buttons displayed, and making them change colors. There is also also reading in the vectors of Rects from text files to make pixel art.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------