# DoGit

Directory Structure of Java Files<br>
--------------------------------------
````
+FKApplyDesign
  -+src
   -+Players
    - Player.java
    - Machine.java
    - Human.java
   -+State
    - State.java
    - StateManager.java
    - StateUpdater.java
    - Point.java
   - PlayGround.java
   - RunTest.java
  - Compile.sh
  - Run.sh
````
Directory Structure of Class Files
-------------------------------------
````
+FKApplyDesign
  -+src
   -+Players
    - Player.class
    - Machine.class
    - Human.class
   -+State
    - State.class
    - StateManager.class
    - StateUpdater.class
    - Point.class
   -+Playground
    - PlayGround.class
   - RunTest.class
  - Run.sh
````
Design Plan 
----------------------------------
````
Instance of a Game Being Played at a Moment 
|''''''''''''''''''''''''''''''''''''''''''''''''''''''|
| |''''''''| |'''''''''|         |'''''''''''|         |
| |Player1 | | Player2 |         |   State   |         |
| |        | |         |         |           |         |
| '''''''''' '''''''''''         '''''''''''''         |
|                                                      |
|                |''''''''''''''| |'''''''''''''|      |
|                | State Updater| | StateManager|      |
|                |              | |             |      |
|                '''''''''''''''' '''''''''''''''      |
|                           PlayGround                 |
''''''''''''''''''''''''''''''''''''''''''''''''''''''''
````


**Playground** Class Which Act As A Box Where Game is Played<br>

**Player** is an Interface act as a Base for Human and Machine Player<br>

**Human** and Machine Class Plays their Moves and they have a symbol they play<br>

**State** initialises the state and prints the State<br>

**StateUpdater** as the name Suggests Contains a State Variable and Updates the state and checks its value<br>

**StateManager** manages the State and Checks if Someone Has Won and returns accordingly<br>

**PlayGround** Contains the Objects of Players, State, Manager, Updater and the game is played and it act as a box<br>

**RunTest** Runs The PlayGround

Added Functionality Thinking of Future Requirements
-----------------
-Multiple Players
-M X N Row For TicTacToe
-K Check 
Like Tic Tac Toe is (3,3,3)
Extend it to (M,N,K)
-can Change the Date Structure
-can Change the ui

TODO
-----
-Improve Interactiveness
-Design Document
-Class Document




