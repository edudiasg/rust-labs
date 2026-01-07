# Guessing Game

Command-line number guessing game written in Rust. The program picks a random
number between 1 and 100 and keeps asking until you guess it.

## Requirements

- Rust toolchain (edition 2024)

## Build and run

Package name: `guessing-game`.

```bash
cargo run
```

## How it works

- A random secret number is generated in the range `1..=100`.
- You enter guesses on stdin until you win.
- Non-numeric input is ignored and the prompt repeats.
- The program compares each guess and prints whether it is too small, too big,
  or correct (and then exits).

## Example session

```text
$ cargo run
Guess the number!
The secret number is: 42
Please input your guess.
50
You guessed: 50
Too big!
Please input your guess.
42
You guessed: 42
You win!
```

## Notes

- The current version prints the secret number to stdout for debugging.
  Remove that line if you want a real guessing game.
