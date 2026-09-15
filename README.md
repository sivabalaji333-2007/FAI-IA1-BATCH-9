# FAI-IA1-BATCH-9
# CHECKERS MINI AI

## 1. ABSTRACT

Checkers Mini AI is an artificial intelligence-based game application that uses adversarial search to make intelligent decisions. The system represents the game as a state-space problem in which two players compete against each other. The AI uses the Minimax algorithm with Alpha-Beta pruning to select the best possible move. Legal moves and mandatory capture rules are implemented according to the rules of Checkers. An evaluation function is used to estimate the strength of a game position when the search reaches its depth limit. The project demonstrates how adversarial search can be applied to a two-player competitive game.

## 2. INTRODUCTION

Artificial Intelligence can be used to create computer players capable of making decisions in competitive games. Checkers is a suitable example because each player's objective is to defeat the opponent by capturing their pieces or preventing them from making legal moves.

In this project, a Checkers AI agent is developed using adversarial search. The AI considers possible moves of both players and searches through the resulting game states. Alpha-Beta pruning is used to eliminate unnecessary branches of the search tree and improve the efficiency of the Minimax algorithm.

## 3. PROBLEM STATEMENT

To design and implement a Checkers AI agent that can play against a human player using adversarial search techniques.

The system must:

Generate legal moves.
Implement mandatory capture rules.
Handle normal moves and captures.
Use an evaluation function.
Apply Minimax/adversarial search.
Use Alpha-Beta pruning.
Select an intelligent move for the AI.
Determine the winning or losing condition.


## 4. SYSTEM REQUIREMENTS
Hardware Requirements
Computer/Laptop
Minimum 4 GB RAM
Keyboard and monitor
Software Requirements
Python 3.x
Visual Studio Code / PyCharm
Windows/Linux/macOS
Python standard libraries

## 5. TECHNOLOGIES USED
Programming Language: Python
Artificial Intelligence Technique: Adversarial Search
Search Algorithm: Minimax
Optimization: Alpha-Beta Pruning
Game Representation: 8 × 8 matrix
User Interface: Console-based interface

## 6. GAME REPRESENTATION

The Checkers board is represented using an 8 × 8 two-dimensional matrix.

The pieces are represented as:

B → Black piece
W → White piece
. → Empty position

Example:

. B . B . B . B
B . B . B . B .
. B . B . B . B
. . . . . . . .
. . . . . . . .
W . W . W . W .
. W . W . W . W
W . W . W . W .

The AI and human player are assigned different pieces.

## 7. AGENT COMPONENTS

The Checkers AI agent consists of the following components:

# 7.1 Initial State

The initial state contains the standard Checkers board with pieces positioned on their starting squares.

# 7.2 Actions

Actions represent all legal moves available to the current player.

# 7.3 Transition Model

The transition model describes the new board position after a player makes a move.

# 7.4 Goal Test

The goal test checks whether one player has won the game.

# 7.5 Utility Function

The utility function assigns a numerical value to a game state.

# 8.LEGAL MOVE GENERATION

The program checks the possible movement directions of each piece and generates valid moves.

A normal piece can move diagonally to an empty square.

A capture is possible when:

An opponent's piece is diagonally adjacent.
The square immediately behind the opponent's piece is empty.

The opponent's piece is then captured.

## 8.ADVERSARIAL SEARCH
Adversarial search is used for games where two players have competing objectives.

The AI assumes that:

It tries to maximize its score.
The opponent tries to minimize the AI's score.

 ## 9.ALPHA-BETA PRUNING
Alpha-Beta pruning improves Minimax by avoiding branches that cannot affect the final decision.

Two values are maintained:

Alpha → Best value found for MAX
Beta  → Best value found for MIN

When:

Alpha >= Beta

the remaining branches can be ignored.

This reduces the number of game states that need to be evaluated and makes the AI faster.


