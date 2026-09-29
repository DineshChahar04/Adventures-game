#Adventure Game

Welcome to my **Adventure Game**
This is a simple **text-based adventure game** made using Python.
In this game, you enter your name and make different choices.
Your choices decide whether you **win or lose the game**.
This project is made for beginners who are learning Python and want to practice:
* Variables
* `input()`
* `print()`
* `if`, `elif`, and `else`
* Nested `if` statements
* String methods
* User choices
* Basic game logic

------------------------------------------------------------------------------------

## How the Game Works

The game starts by asking for your name.
```python
name = input("Type your name: ")
```
Then the game welcomes you:
```python
print("Welcome", name, "to this adventure!")
```
After that, you reach a dirt road.
You have two choices:
```text
LEFT
RIGHT
```
Your choice decides what happens next.

-----------------------------------------------------------------------------------------------------

#  Game Story

You are walking on a dirt road.
The road comes to an end.
You have two options:
```text
Left
Right
```

## If You Choose Left
You reach a river.
You can:
*  Walk around the river
*  Swim across the river
###  Swim
If you choose `swim`:
```text
You swam across and were eaten by an alligator.```
 **You lose!**
### Walk
If you choose `walk`:
```text
You walked for many miles, ran out of water and you lost the game.
```
 **You lose!**

---------------------------------------------------------------------------------------------

# If You Choose Right

You reach a bridge.
The bridge looks wobbly.
You can:
```text
Cross
Back
```
##  Choose Back
If you choose `back`:
```text
You go back and lose.
```
 **You lose!**

## Choose Cross
If you choose `cross`, you successfully cross the bridge.
But then you meet a stranger! 
The stranger asks if you want to talk.
You can choose:
```text
Yes
No
```
### Choose Yes
The stranger gives you gold.
```text
You talk to the stranger and they give you gold. You WIN!
```
 **YOU WIN!**

### Choose No
You ignore the stranger.
The stranger becomes offended.
```text
You ignore the stranger and they are offended and you lose.
```
 **You lose!**

--------------------------------------------------------------------------------------------

#  How to Run the Game

## 1. Install Python
First, make sure Python is installed on your computer
You can check it by opening Command Prompt or Terminal and typing:
```bash
python --version
```
If Python is installed, you will see something like:
```text
Python 3.x.x
```
------------------------------------------------------------------


##  Run the Game

Open the terminal inside the project folder and run:
```bash
python adventure.py
```
The game will start.

--------------------------------------------------------------------

# Python Concepts Used

## 1. Variables
The game uses a variable called `name`.
```python
name = input("Type your name: ")
```
The user's name is stored inside the `name` variable.

## 2. input()
`input()` is used to take information from the player.
Example:
```python
answer = input("Choose left or right: ")
```
The player can type:
```text
left
```
or:
```text
right
```

## 3. print()
`print()` displays something on the screen.
Example:
```python
print("You win!")
```
Output:
```text
You win!
```

## 4. if Statement
The `if` statement checks a condition.
Example:
```python
if answer == "left":
    print("You went left.")
```
This means:
> If the player enters `"left"`, run this code.

## 5. elif
`elif` means **else if**.
Example:
```python
if answer == "left":
    print("You went left.")
elif answer == "right":
    print("You went right.")
```
The program checks the first condition.
If it is false, it checks the `elif` condition.

## 6. else
`else` runs when none of the previous conditions are true.
Example:
```python
else:
    print("Not a valid option.")
```
So if the player enters:
```text
hello
```
the game displays:
```text
Not a valid option.
```

# Using .lower()
The game uses:
```python
.lower()
```
Example:
```python
answer = input("Left or right? ").lower()
```
This converts the user's answer into lowercase.
So these inputs:
```text
LEFT
Left
lEfT
left
```
all become:
```text
left
```
This makes the game easier for the player.

# Nested if Statements
This project also uses **nested if statements**.
A nested `if` means an `if` statement inside another `if` statement.
For example:
```python
if answer == "right":
    answer = input("Cross or back? ")
    if answer == "cross":
        print("You crossed the bridge.")
```
The second `if` only happens after the player chooses `right`.
This is useful for creating different paths in a game.

------------------------------------------------------------------------------

# Game Flow
The game can be understood like this:

```text
                 START
                   |
              Enter Name
                   |
              Dirt Road
              /         \
           LEFT          RIGHT
            |              |
          River          Bridge
         /     \         /     \
      SWIM     WALK    BACK    CROSS
        |        |       |       |
       LOSE     LOSE    LOSE   Stranger
                                  |
                              /       \
                            YES        NO
                             |          |
                            WIN        LOSE
```

----------------------------------------------------------------------------------------------

#  Project Structure
The project is very simple:
```text
Adventure-Game/
│
├── adventure.py
│
└── README.md
```

### `adventure.py`
Contains the complete Python game.

### `README.md`
Contains information about the project, gameplay, installation, and Python concepts.

------------------------------------------------------------------------

#  Technologies Used
*  **Python**
*  **VS Code/jupyter notebook** (recommended)
*  **GitHub**
No external Python libraries are required.

#  Features
*  Interactive text-based gameplay
*  Player name input
*  Multiple paths
*  River adventure
*  Bridge adventure
*  Stranger encounter
*  Winning path
*  Multiple losing paths
*  Invalid input handling
*  Nested decision-making

#  Future Improvements
I can improve this game in the future by adding:
*  Player health
*  Gold system
*  Inventory
*  Enemies
*  Monsters
*  More locations
*  Keys and locked doors
*  Puzzles
*  Random events
*  Different endings
*  Play again option
*  Save game system
*  Sound effects
*  Graphical interface

-------------------------------------------------------------------------------------------------

# What I Learned
While making this project, I practiced how to:
```text
Take user input
      ↓
Store it in variables
      ↓
Check the user's choice
      ↓
Use if / elif / else
      ↓
Create different game paths
      ↓
Give the player different endings
```
This project helped me understand how basic Python programming can be used to create an interactive game.

-----------------------------------------------------------------------------------------

# Author
**Dinesh Chahar**
Beginner Python Developer!
Currently learning:
*   C#
*  DSA
*  OOP
  

------------------------------------------------------

## If You Like This Project\
If you found this project interesting, you can:
------>>> Star the repository

### Thanks for Playing!
**Choose your path carefully...**
**Left or Right? **
