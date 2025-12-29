# Hangman (Java)

A command-line Hangman game implemented in Java using 1D arrays, StdIn, and StdOut. The program selects a random word from an input file, allows the user to guess letters, displays a hangman figure as incorrect guesses are made, and exports final game statistics to an output file.

## Features
- Random word selection from input file
- Letter validation (uppercase supported, converted to lowercase)
- Prevents duplicate guesses
- Tracks total and incorrect guesses
- ASCII hangman visualization
- Win/loss detection
- Exports game statistics to an output file

## Requirements
- Java
- Course-provided StdIn, StdOut, and StdRandom libraries
- Properly formatted input file

## Compile
javac Hangman.java

## Run
java Hangman inputFileName outputFileName

Example:
java Hangman input1.in stats.out

## Input File Format
The input file must contain:
- An integer n (number of words)
- n words (space or newline separated)

Example:
5
apple
banana
orange
grape
melon

## Game Rules
- The user guesses letters one at a time
- Invalid characters are rejected
- Repeated guesses are not counted
- Correct guesses reveal letters in the word
- Incorrect guesses increase the hangman stage
- The game ends when:
  - The word is fully guessed (win)
  - 6 incorrect guesses are made (loss)
  - The user enters 0 to quit (no stats exported)

## Scoring
If the user wins:
Points = 100 - ((incorrect guesses / total guesses) × 100)

If the user loses:
Points = 0

## Output File Format
You won / You lost
Points: <points>
The word was: <word>
Total guesses: <total guesses>
Incorrect guesses: <incorrect guesses
