# Flashcard App

A simple flashcard application built with Python using the `tkinter` library. This app helps you learn and test your knowledge of French words by displaying flashcards with a French word on one side and its English translation on the other. You can mark words as "known" to remove them from your learning queue and save your progress.

## Features

- **Flashcards**: Displays French words with English translations.
- **Mark Known**: Mark words as "known" to remove them from the learning list.
- **Timed Flip**: Flashcards automatically flip after a set interval.
- **Progress Save**: Saves progress to `words_to_learn.csv`.

## Requirements

- Python 3.x
- `tkinter` (pre-installed with Python)
- `pandas` (install via `pip install pandas`)

## How to Run

1. Clone this repository or download the files to your local machine.
2. Install required dependencies (e.g., `pandas`).
3. Ensure you have the `french_words.csv` file for initial data.
4. Run the Python script:

    ```bash
    python flashcard_app.py
    ```

## File Structure

- `flashcard_app.py`: Main application file with flashcard logic.
- `french_words.csv`: Default CSV file with French-English words.
- `words_to_learn.csv`: Stores words you need to learn, updated as you mark words as "known."

## Code Explanation

### `next_card()`
This function:
- Loads a new random flashcard.
- Displays the French word on the front.
- Sets a timer to flip the card to the English word after 4 seconds.

### `flip_card()`
- Flips the flashcard to show the English translation after the timer expires.

### `is_known()`
- Marks the current word as known by removing it from `to_learn` and saves progress to `words_to_learn.csv`.

### `flip_timer`
- Tracks the interval for automatically flipping flashcards after a set time.


## Contributing

If you'd like to contribute, feel free to open issues or submit pull requests.
