// *********************************************************
// Course: TCP1101 PROGRAMMING FUNDAMENTALS 
// Year: Trimester 1, 2022/23 (T2215) 
// Lab: T14L 
// Names: KAWSAR | CHEN FU LIN | LAU JUN XING 
// IDs: 1211310827 | 1221301545 | 1201102941
// Emails: mdrisveyhasan1@gmail.com | fulincheng1018@gmail.com | xinglau92@gmail.com
// Phones: +601169727851 | +60163864848 | +60164074733
// *********************************************************

# T14L GROUP 1
# Alien vs. Zombie

Please introduce the game here.

You may add one signature screenshot of your program here or above the title. Check out [this tutorial](https://www.digitalocean.com/community/tutorials/markdown-markdown-images) to learn how to do it.

Please provide the YouTube link to your [Video Demo]([https://youtube.com](https://www.youtube.com/watch?v=2GPoesbnCJE).

## Compilation Instructions

Provide instructions on how to compile your program, especially when it is non-trivial.

1. g++ main.cpp
2. .\a

## User Manual

--HOW TO USE--

Default setting:
There will be a default setting provided if user does not wish to make any changes. User will be asked if they would like to make changes. User will only be allowed to enter "y" or "n". If user enters different characters or numbers, users will be asked to re-enter the input. 

Board setting:
When user wants to update or customise its board setting, it will lead them into the board setting. User will be asked to enter the number of rows, number of columns and number of zombies. If user accidentally enters other than integer number, they will be asked to re-enter again. Besides, if user enters even number, they will be asked to enter again. After that, the gameboard will be created according to user's input. The alien will also be shown at the center of the board automatically.

Gameboard:
The gameboard class would create an empty gameboard with the provided dimantions to the class constructor.
Create a gameboard: Gameboard board_name = Gameboard(int number_of_rows, int number_of_cols);
The gameboard has 5 different properties respectively columns, rows, total_cols, total_rows and the pointer to the 2D array of the actual gameboard namely "board".
The board will have 2*provided_rows + 1 rows and 2*provided_cols + 1 columns in total.
Within these rows and columns only the odd places would be empty for game characters.

Example: Let's say you want to put a zombie in the first top right corner of the board, you can access the top right corner with board[1][1] selector and you can set it to whatever you want.

Showing the gameboard: The Gameboard object will have a default showGameboard() methood that will allow you to show the gameboard as it is.
Example: board_name.showGameboard();

Characters:
All the characters will have some common characteristics as below:
char name: name of the character
int life: total life of the character
int impact: hit impact of the character
int x_pos: character position on the x dimension
int y_pos: character position on the y dimension
bool alive: if the character is alive after getting hit

Also they will have the common movement method.
Movement methods:
move_up();
move_down();
move_right();
move_left();
Note: Every time you move the character, it will move by 2 rows or columns as the board itself has it's own elements occopying certain places on the board.

Beside movements they will have a gotHit methood calling which would change the life of the character according to the hit impact and set the "alive" property as "false" if the life becomes < 0.

Alien:
Beside the common characteristics, alien would have its "int max_life" and "int attacs".
The name is set to 'A' as default.
Methoods:
Beside the common methoods described earlier it would have the below methoods:
addLife(): This methood will increase the life of the alien till max_life with the provided increment.
attacked(): This will increase the "attacks" number by one.

Example:
Create the alien object:- Alien alien_name = Alien(int set_maxLife, int set_impact, int set_x, int set_y);
Get name:- alien_name.name;
Get x position:- alien_name.x_pos;
Add life:- alien_name.addLife();
Increase attakcs number:- alien_name.attacked();
Got hit:- alien_name.gotHit();
Move:- alien_name.move_up();

Zombie:
It would have all the common characteristics and methoods described in the Characters section.
Example:
Create a zombie object:- Zombie zombie_name = Zombie(char set_name, int alienLife, int set_x, int set_y);
Get x position:- zombie_name.x_pos;
Get name:- zombie_name.name;
Got hit:- zombie_name.gotHit();

Rock:
It will have all the common characteristics.
Beside common methoods it will have reveal() methood to reveal its hidden item. The hidden item would be picked up randomly and returned as a char value. You will have to create a new game object based on the returned char value and put it back to the gaemboard on the same place as the rock holds.
Example:
You cna create and access the properties of the object following previous examples.

Pod:
Beside common characteristics it would have an attack_radius, you will have to set the radious as you create the object.
The name is set to 'P' as default.
The impact is set to 10 as default.
Example:
You cna create and access the properties of the object following previous examples.

## Progress Log

- [Part 1](PART1.md)
- [Part 2](PART2.md)

## Contributors

Please replace the following with your group members' names. 

- Kawsar
- Cheng Fu Lin
- Lau Jun Xing
