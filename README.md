# Bulls and Cows Game with Entropy

A Python implementation of the Bulls and Cows number guessing game that includes entropy calculation to measure information gain during gameplay.

## Features

- Implementation of classic Bulls and Cows gameplay
- Entropy calculation for each guess
- Real-time visualization of entropy reduction
- Input validation for 4-digit numbers
- Tracking of possible remaining numbers
- Interactive plotting using matplotlib

## Requirements

- Python 3.x
- NumPy
- Matplotlib

## Game Rules

1. The computer generates a random 4-digit number with unique digits
2. Player guesses a 4-digit number with unique digits
3. For each guess, the game returns:
   - Bulls: Correct digits in correct positions
   - Cows: Correct digits in wrong positions
4. Game continues until player gets 4 Bulls (correct answer)

## Entropy Features

- Calculates initial entropy based on all possible combinations (5040 possibilities)
- Updates entropy after each guess
- Visualizes entropy reduction over gameplay rounds
- Provides information about remaining possible numbers

## Usage

Run the main script to start the game:

```python
python bulls_and_cows.py
```

The game will:
1. Generate a random target number
2. Accept player guesses
3. Display Bulls/Cows feedback
4. Show entropy calculations
5. Plot entropy reduction
6. Allow multiple games

## Functions

- `get_all_valid_numbers()`: Generates all possible valid number combinations
- `random_num()`: Generates random target number
- `user_num()`: Handles user input with validation
- `check_num(num, user)`: Calculates Bulls and Cows
- `entropy(a,b)`: Calculates entropy based on Bulls and Cows
- `plot_entropy(entropy_history, rounds)`: Visualizes entropy reduction

## Author

Kuan-Chen Chen
