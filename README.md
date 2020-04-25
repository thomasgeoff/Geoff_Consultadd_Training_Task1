# Guess The River Size
#### by Geoff Thomas

Python mini project, part of the Consultadd's [Python Training](https://consultadd.com/it-training-services/python-training-placement/).

## Introduction
It is an interactive Python game application that runs in the command line or terminal based on your OS. It starts by authenticating users and prompts the user for a 2D matrix input of 1's representing river & 0's representing land. A [BFS](https://en.wikipedia.org/wiki/Breadth-first_search) algorithm is used to compute the river sizes array. Then the user is prompted to guess the river sizes at each index. If all the user guesses are right then he/she is declared as the winner.

## Prerequisites
1. Download and install [Python 3.x](https://www.python.org/downloads/)
2. Download the project Git repository and unzip it to the desired directory

## Project contents

This project consists of the following files:
* **welcome_note.txt** - is the text file containing the welcome note displayed at the beginning of the game
* **game_instructions.txt** - is the text file containing the instructions for the game.
* **Task_Training_Data.csv** - is the CSV file containing all the registered users
* **read_csv.py** - contains a single function which read the user information from the Task_Training_Data.csv file
* **authenticate_data.py** - imports the registered users from read_csv.py and contains multiple functions described below:
  * authenticate_user(): authenticates the users by prompting the user for a name and email to matches with registered users
  * show_welcome_note(): displays the welcome note if the users get into the game
  * show_game_instruction(): displays the game instructions if the user wants to play
  * get_matrix_input(): prompts the user to input a 2D matrix of 1's and 0's
* **game_functionality.py** - imports the 2D matrix input from authenticate_data.py and contains two functions to perform the game logic as described below:
  * find_river_size(): takes the 2D matrix as input and find the river sizes using a BFS(breadth-first search) algorithm.
  * guess_the_river_sizes(): takes the river_size array as input and prompt the user to guess the river size at each index. The user guesses are evaluated against the river_size array to determine the winning percentage of the user. 
* run.py - is the file executed to run the game.

## Usage

Suppose your downloaded project folder is in "C:\Guess_River_Size\run.py" on Windows or "~/Guess_River_Size/run.py" on an Unix-like systems like Mac or Linux.
* **Windows**
  * Open Command line:   Start menu -> Run  and type cmd
  * Type:```C:\python27\python.exe C:\Guess_River_Size\run.py```
                             
      **OR**
  * Open Command line: Start menu -> type cmd -> Run as administrator
  * Type:```python C:\Guess_River_Size\run.py```

* **Mac OS X**
  * Open Command line: Finder-> Go menu -> Applications -> Terminal
  * Type:```python ~/Guess_River_Size/run.py```
* **Linux**
  * Open a Linux terminal: press Ctrl+Alt+T in Ubuntu or press Alt+F2 or Type gnome-terminal and press enter.
  * Type:```python ~/Guess_River_Size/run.py```
**Note:** Make sure you are in the right directory.

## Contact

[Portfolio](www.thomasgeoff.com)

## You wanna make a Readme.md file?
[www.makeareadme.com](https://www.makeareadme.com/)
