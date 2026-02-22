Terminal Yahtzee (C-Based Dice Game)

    A classic implementation of the Yahtzee dice game, developed as a Year 1 Semester 1 (Y1S1) programming project. This is a command-line interface (CLI)                application where a human player competes against a computer opponent over 13 rounds of strategic dice rolling.

🎮 Game Overview

     Yahtzee is a game of luck and strategy. The goal is to score points by rolling five dice to make specific combinations. Each combination has different scoring       rules, and once a category is used, it cannot be used again for the rest of the game.

Features

    Human vs. Computer: Play against an automated opponent.
    Smart Computer AI: The computer evaluates its hand to decide which dice to keep and which scoring category is optimal.
    Complete Scoring Rules: Includes all standard categories:
    Upper Section: Ones through Sixes.
    Lower Section: Three of a Kind, Four of a Kind, Full House, Small Straight, Large Straight, Yahtzee, and Chance.
    Interactive CLI: Uses ANSI escape codes for colored round headers to improve readability in the terminal.

🛠️ Technical Details

    The game is written in C and demonstrates several fundamental programming concepts:
    Arrays: Used for managing dice values, scorecards, and tracking chosen categories.
    Control Flow: Implementation of switch-case logic for round management and scoring rules.
    Modular Design: Divided into distinct functions for rolling, scoring, and AI decision-making.
    Randomization: Utilizes stdlib.h and time.h to ensure truly random dice rolls.

🚀 How to Run
    Requirement: You need a C compiler (like gcc) installed on your system.

    Clone the repository:

    Bash
    
    git clone https://github.com/your-username/yahtzee-c-project.git
    cd yahtzee-c-project
    
    Compile the code:

    Bash
    gcc game2.c -o yahtzee
    Run the game:

    Bash
    ./yahtzee
    
🕹️ How to Play

    On your turn, the dice will roll automatically.
    You can choose to keep specific dice (1 for yes, 0 for no) and re-roll the rest.
    You have a maximum of 3 rolls per turn.
    After rolling, select an available scoring category (0-12) based on the prompt.
    The game ends after 13 rounds, and the player with the highest total score wins!

📝 Project Reflection

    This project was developed to practice structured programming in C. Key challenges included implementing the logic for "Straights" and "Full House" scoring, as well as creating a basic "Evaluate" function to give the computer player a competitive strategy.
