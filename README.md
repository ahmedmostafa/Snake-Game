# CPPND: Capstone Snake Game Example

This is a starter repo for the Capstone project in the [Udacity C++ Nanodegree Program](https://www.udacity.com/course/c-plus-plus-nanodegree--nd213). The code for this repo was inspired by [this](https://codereview.stackexchange.com/questions/212296/snake-game-in-c-with-sdl) excellent StackOverflow post and set of responses.

<img src="snake_game.gif"/>

The Capstone Project gives you a chance to integrate what you've learned throughout this program. This project will become an important part of your portfolio to share with current and future colleagues and employers.

In this project, you can build your own C++ application or extend this Snake game, following the principles you have learned throughout this Nanodegree Program. This project will demonstrate that you can independently create applications using a wide range of C++ features.

## New Features:
* The player can pause and resume the game via space button.
* The wondow automatically terminates when the snake dies, and game over is printed to the command prompt.  
* The highest record is saved in a file. 
  * Displayed on the windows title.
  * After the game terminated the new score is stored, and compared to the latest high score, if it is higher a congratulation message is displayed. 
* Diff good types are added. 
  * snacks: with purple color, adds 1 to the score. 
  * booster: with green color, adds 10 to the score.
  * poison: with red color, it is displayed for 5 seconds, an disappered if it was avoided by the player,
            if the snake it, it will die.

## Addressed Rubric items. 
* 3.1 The project demonstrates an understanding of C++ functions and control structures:
  * This can be obviously seen in all of the new introduced implementation. 
* 3.2 The project reads data from an external file or writes data to a file as part of the necessary operation of the program :
  * This point is satisfied by the new feature of saving and retrieving the highest score.
* 3.3 The project accepts user input and processes the input:
  * This point is satisfied by pause/resume feature. 
* 4.1 The project code is organized into classes with class attributes to hold the data, and class methods to perform tasks.
 * This point is satisfied by the new feature (class) Scores (score.cpp, score.h) which is used to read,write & save the highest score
 * also it is satisfied by the new food types.
* 4.2 Classes use appropriate access specifiers for class members.
 * In the new Score class & food classes, the data is kept private and proper setters and getters are implemented. 
* 4.3 Class constructors utilize member initialization lists. 
 * new classes for Scores & snake food, are initialized with initialization lists.
* 4.4 Classes abstract implementation details from their interfaces.
 * This point is satisfied by the new classes for High score & snake food types.
* 4.5 Classes encapsulate behavior.
 * This point is satisfied by the new classes for High score & snake food types.
* 4.6 Overloaded functions allow the same function to operate on different parameters.
 * This is satisfied by the SnakeFood class which is inherited by 3 child classes for the food types 
   SnakeSnacks, SnakeBooster & SnakePoison class.



## Dependencies for Running Locally
* cmake >= 3.7
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* SDL2 >= 2.0
  * All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
  >Note that for Linux, an `apt` or `apt-get` installation is preferred to building from source. 
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./SnakeGame`.


## CC Attribution-ShareAlike 4.0 International


Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
