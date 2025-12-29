Hangman (Java)

A command-line Hangman game built with 1D arrays, StdIn, and StdOut.
The program reads a list of words from an input file, selects one at random, and runs a playable hangman loop with up to 6 incorrect guesses. At the end, it writes game stats to an output file.

Features
	•	Random word selection from an input file
	•	Letter validation (accepts uppercase, converts to lowercase)
	•	Tracks previously guessed letters (prevents duplicate guesses)
	•	Updates the visible word state using underscores _
	•	ASCII hangman drawing that progresses with wrong guesses
	•	Exports game results to an output file

Requirements
	•	Java (compatible with the course StdIn, StdOut, StdRandom libraries)
	•	Input file formatted correctly (see below)
