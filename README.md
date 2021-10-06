# TIC_TAC_TOE

In this project, the pygame library is used to take care of the user interface part of the project and make an effort to make the game board as attractive as possible.
For the actual code of the game it is traversed through the rows, columns and diagonals after every move to check whether any player has won.

## What is TIC_TAC_TOE?

Tic Tac Toe is one of the most played games and is the best time killer game that you can play anywhere with just a pen and paper. If you don’t know how to play this game don’t worry let us first understand that.
The game is played by two individuals. First, we draw a board with a 3×3 square grid. 
The first player chooses ‘X’ and draws it on any of the square grid, then it’s the chance of the second player to draw ‘O’ on the available spaces.
Like this, the players draw ‘X’ and ‘O’ alternatively on the empty spaces until a player succeeds in drawing 3 consecutive marks either in the horizontal, vertical or diagonal way. 
Then the player wins the game otherwise the game draws when all spots are filled.

Running the project locally
Steps to be followed:
First, let’s check the steps to build Tic Tac Toe program in Python:
●	Create the display window for our game.
●	Draw the grid on the canvas where we will play Tic Tac Toe.
●	When a player manages to win the game, we draw a winning line to indicate the same.
●	When someone wins the game or the game is a draw then the players can reset the game by pressing the “R” key on their keyboard.
We need to run our game inside an infinite loop. 
It will continuously look for events and when a user presses the mouse button on the grid we will first get the X and Y coordinates of the mouse.
Then we will check which square the user has clicked.
Then we will draw the appropriate ‘X’ or ‘O’ image on the canvas. 
So that is basically what we will do in this Python project idea.

## Installation

import pygame
import sys
import numpy as np
pygame.init()


    ## Color Reference
    
    # CONSTANTS
WIDTH = 600
HEIGHT = 600
LINEWID= 15
WINLINEWID= 15
BOARDROW= 3
BOARDCOL = 3
SQSIZE = 200
CIRCRAD = 60
CIRCWIDTH = 15
CROSSWID = 25
SPACE = 55


BGCOLOR = (28, 170, 156)
LNCOLOR = (23, 145, 135)
CIRCCOLOR = (239, 231, 200)
CROSSCOLOR = (66, 66, 66)# CONSTANTS
WIDTH = 600
HEIGHT = 600
LINEWID= 15
WINLINEWID= 15
BOARDROW= 3
BOARDCOL = 3
SQSIZE = 200
CIRCRAD = 60
CIRCWIDTH = 15
CROSSWID = 25
SPACE = 55


BGCOLOR = (28, 170, 156)
LNCOLOR = (23, 145, 135)
CIRCCOLOR = (239, 231, 200)
CROSSCOLOR = (66, 66, 66)
  
## Deployment

# SCREEN
screen = pygame.display.set_mode( (WIDTH, HEIGHT) )
pygame.display.set_caption( 'TIC TAC TOE' )
screen.fill( BGCOLOR )

def drawfigures():
    for row in range(BOARDROW):
        for col in range(BOARDCOL):
            if board[row][col] == 1:
                pygame.draw.circle( screen, CIRCCOLOR, (int( col * SQSIZE + SQSIZE//2 ), int( row * SQSIZE + SQSIZE//2 )), CIRCRAD, CIRCWIDTH )
            elif board[row][col] == 2:
                pygame.draw.line( screen, CROSSCOLOR, (col * SQSIZE + SPACE, row * SQSIZE + SQSIZE - SPACE), (col * SQSIZE + SQSIZE - SPACE, row * SQSIZE + SPACE), CROSSWID )
                pygame.draw.line( screen, CROSSCOLOR, (col * SQSIZE + SPACE, row * SQSIZE + SPACE), (col * SQSIZE + SQSIZE - SPACE, row * SQSIZE + SQSIZE - SPACE), CROSSWID )

  
## Screenshots

https://github.com/sagnik4516/TIC_TAC_TOE-/blob/main/Screenshot%20(60).png

  
## Tech Stack

**Client:** VsCode, Python3, 

**Server:** Pygame

  
## Features

- User Friendly GUI
- Live previews
- Fullscreen mode
- Cross platform
- Smooth running API

  

