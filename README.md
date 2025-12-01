# Cyphers & Letters

“Numbers and Letters” is a TV game show played over a set number of rounds (e.g., 10), alternating between two subgames:

- **Letter rounds**: 10 letters are generated. Each participant must propose the longest valid word that can be formed using only those letters (no letter can be used more times than it appears).
- **Number rounds**: 6 numbers and a random target are generated. Using basic arithmetic operations (+, −, ×, ÷), the participant tries to reach the target exactly or as close as possible.

Both players attempt to find the best solution under the given constraints and score points accordingly. The player with the most points at the end wins.

In this project, the human player must be able to play against the computer (CPU). The game must be playable in either Spanish or Catalan (professors will provide letter distributions and dictionaries of valid words for each language).

This is the final project for Programming – Informatics I (20302) at the University of the Balearic Islands for the 2025-2026 course.

## 🎯 Objectives

### 1. Play a Game
- **Play against the computer (CPU)**  
  - A player enters their name (the computer is named “CPU”).  
  - N rounds are played (N ≥ 2; N must be even), alternating between numbers and letters.  
  - Both players compete in each round. Restrictions (numbers and target, or letters) must be displayed, solutions obtained, and scores accumulated.  
  - The computer must attempt to find the best possible solution.  
  - The winner is displayed at the end.  
  - A record of the game is saved.  

- **Play against another human (Optional)**  
  - Both players enter their names.  
  - N rounds are played (N ≥ 2; N must be even).  
  - The winner is displayed at the end.  
  - A record of the game is saved.  

### 2. Records
- **Show results of games played**  
  - Display recorded data of all games: date, type of game (vs CPU or vs human), names of players, CPU level (if implemented), number of rounds, scores, and winner.  

- **Show statistics of a player (Optional)**  
  - Display summary statistics: total games played, won, win percentage, average score per game.  

### 3. Options (Optional)
- Configure number of rounds, number of letters/numbers, language, etc.  

### 4. Exit
- The program must run through a menu, allowing multiple games or record consultations until the user chooses to exit.  

## 🧩 Game Specification

### Letter Rounds
- Generate 10 letters randomly from a distribution file provided by professors.  
- A word is valid if:  
  - It uses only available letters without exceeding multiplicity.  
  - It exists in the dictionary of valid words.  
- Player enters a word. CPU searches dictionary for the best possible word.  
- **Scoring**: word length = points. Invalid word = 0 points.  

### Number Rounds
- Generate 6 numbers randomly from a distribution file (numbers 1–10 twice, and 25, 50, 75, 100 once).  
- Generate a random target between 100 and 999.  
- Rules: use each number at most once, only integer results, max 5 operations.  
- CPU strategy: random search with limited attempts, keeping the best solution found.  
- **Scoring**:  
  - Exact result: 10 points  
  - Difference 1–5: 7 points  
  - Difference 6–10: 5 points  
  - Difference >10: 0 points  

## 🚫 Restrictions
- Must have the option to play vs CPU.  
- Must show previous games results.  
- Must use provided files (letters, dictionary, numbers).  
- Must use object-oriented programming.  
- String methods (like `charAt`, `split`, `substring`, etc.) are prohibited except for input/output.  
- No advanced techniques (recursion, backtracking, regex, dynamic structures like ArrayList).  
- Must use LT class for keyboard input.  
- Must be implemented in Java, NetBeans Ant project.  
- Must include a short report (3–6 pages).  

## ✅ Evaluation
- Mandatory objectives must be implemented.  
- Report must include: objectives, design, data structures, algorithms, user manual, conclusions, references (including explicit mention of generative AI use).  
- Code must be clear, well-structured, object-oriented, with meaningful identifiers, proper indentation, comments, and modular design.  
- User interface must be clear and consistent.  
- Passing requires meeting restrictions and mandatory objectives.
