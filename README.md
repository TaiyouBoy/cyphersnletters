# cyphersNletters
Universitat de les Illes Balears

Programming – Informatics I (GEIN, GTTT) Final Project Statement. Course 2025–2026
Academic Objective

The academic objective of the final project is to consolidate the knowledge acquired in class. Specifically, students must demonstrate, through the development of a complete project, the use of the following concepts: algorithmic design, data types, code clarity, control structures, sequential processing, subprograms, data structures, object-oriented programming, text files, top-down design, and keyboard interface. In addition, they must work on the generic competencies of the subject: analysis and synthesis, organization and decision-making, and written communication of computer science concepts.

The project must be solved using the same tools used during the course: the Java programming language, the NetBeans integrated development environment (Java Ant project), the LT class, and other tools and classes used during the course or developed specifically for this project. Solutions using advanced concepts not covered in class will not be accepted.

The project may be done individually or in pairs (students from the same practice group).
Academic Integrity

According to the regulations on academic fraud at the University of the Balearic Islands (Normative Agreement 154181), academic fraud includes:

    Including content from any source (external works, websites, generative AI, etc.) in individual or group projects and presenting it as one’s own without proper citation.

    Submitting or copying parts of a project delivered by another student, in the same year or previous years, and presenting it as new work.

    Outsourcing the completion of a project to third parties.

Sanctions apply to all students involved in committing academic fraud. Practices will be automatically reviewed with anti-plagiarism software designed to detect copied code.
Project Statement
Introduction

“Numbers and Letters” is a TV game show played over a set number of rounds (e.g., 10), alternating between two subgames:

    Letter rounds: 10 letters are generated. Each participant must propose the longest valid word that can be formed using only those letters (no letter can be used more times than it appears).

    Number rounds: 6 numbers and a random target are generated. Using basic arithmetic operations (+, −, ×, ÷), the participant tries to reach the target exactly or as close as possible.

Both players attempt to find the best solution under the given constraints and score points accordingly. The player with the most points at the end wins.

In this project, the human player must be able to play against the computer (CPU). The game must be playable in either Spanish or Catalan (professors will provide letter distributions and dictionaries of valid words for each language).
Objectives
1. Play a Game [mandatory]

    Play against the computer (CPU) [mandatory]

        A player enters their name (the computer is named “CPU”).

        N rounds are played (N ≥ 2; N must be even), alternating between numbers and letters. Both players compete in each round. Restrictions (numbers and target, or letters) must be displayed, solutions obtained, and scores accumulated.

        The computer must attempt to find the best possible solution.

        The winner is displayed at the end.

        A record of the game is saved.

    Play against another human [optional]

        Both players enter their names.

        N rounds are played (N ≥ 2; N must be even).

        The winner is displayed at the end.

        A record of the game is saved.

2. Records [mandatory]

    Show results of games played [mandatory]

        Display recorded data of all games: date, type of game (vs CPU or vs human), names of players, CPU level (if implemented), number of rounds, scores, and winner.

    Show statistics of a player [optional]

        Display summary statistics: total games played, won, win percentage, average score per game.

3. Options [optional]

    Configure number of rounds, number of letters/numbers, language, etc.

4. Exit [mandatory]

    The program must run through a menu, allowing multiple games or record consultations until the user chooses to exit.

Game Specification
Letter Rounds

    Generate 10 letters randomly from a distribution file provided by professors.

    A word is valid if:

        It uses only available letters without exceeding multiplicity.

        It exists in the dictionary of valid words.

    Player enters a word. CPU searches dictionary for the best possible word.

    Scoring: word length = points. Invalid word = 0 points.

Number Rounds

    Generate 6 numbers randomly from a distribution file (numbers 1–10 twice, and 25, 50, 75, 100 once).

    Generate a random target between 100 and 999.

    Rules: use each number at most once, only integer results, max 5 operations.

    CPU strategy: random search with limited attempts, keeping the best solution found.

    Scoring:

        Exact result: 10 points

        Difference 1–5: 7 points

        Difference 6–10: 5 points

        Difference >10: 0 points

Files

    letters_es.txt / letters_ca.txt: letter distributions for Spanish/Catalan.

    numbers.txt: number distribution.

    dictionary files: valid words for each language.

    results.txt: record of games played.

Restrictions

    Must implement at least:

        Play vs CPU

        Show game results

        Exit option

    Must use provided files (letters, dictionary, numbers).

    Must use object-oriented programming.

    String methods (like charAt, split, substring, etc.) are prohibited except for input/output.

    No advanced techniques (recursion, backtracking, regex, dynamic structures like ArrayList).

    Must use LT class for keyboard input.

    Must be implemented in Java, NetBeans Ant project.

    Must include a short report (3–6 pages).

Evaluation

    Mandatory objectives must be implemented.

    Report must include: objectives, design, data structures, algorithms, user manual, conclusions, references (including explicit mention of generative AI use).

    Code must be clear, well-structured, object-oriented, with meaningful identifiers, proper indentation, comments, and modular design.

    User interface must be clear and consistent.

    Passing requires meeting restrictions and mandatory objectives.

