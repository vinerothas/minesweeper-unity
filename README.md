# minesweeper-unity

This project takes a spin on the classis minesweeper game. It includes (among others) utility items, 
scoring system, time constraints and board choice. The game used to have a working multiplayer using an 
Amazon EC2 server for matchmaking. The players could interact with each other by placing mines or making 
some tiles momentarily inaccessible using different skills. Charges for the skills are obtained through
uncovering tiles. This system still works in singleplayer, but offensive skills are disabled. I abandoned this
project after starting to rewrite the game to handle the game state on the server to avoid potential cheating.
I stopped working on the project in order to have more time for studying.  

## How to play
You need unity player to run Saper.exe.  
Choose singleplayer and then pick your preferred board. Uncover tiles using left-click and 
mark mines using right-click (classic minesweeper rules). Sometimes when uncovering tiles
you will get charges for the skills shown below the board. Charges will show up as a number
in the upper right corner of the corresponding skill. Choose a skill using left-click or numbers 1, 2 or 3.
Use the skill using left-click. Cancel using a skill by right-click.  
Skills:  
1. Boot: use on a covered tile. The tile becomes uncovered if it's empty, or is marked with a flag if it's a mine.  
2. Grenade: use on a covered tile. Uncovers tiles in a cross pattern and removes any mines inside it. 
The tiles become scorched, which is a purely visual effect.  
3. Radar: place on an uncovered tile. A scanning line will appear which will show blips once it touches
a tile containing an unflagged mine.  

Clicking on a mine doesn't end the game, but you get negative points. A tile with an exploded mine will 
not show how many mines there are around it.
