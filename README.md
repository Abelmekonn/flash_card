# Flashy - Flashcard Learning App

Flashy is a Python-based flashcard learning application built using the Tkinter library. This application helps users learn French words through a simple and interactive graphical user interface.

## Features

- **Random Flashcards**: Presents French words randomly for enhanced learning.
- **Card Flip**: Automatically flips the card after 3 seconds to show the English translation.
- **Known/Unknown Tracking**: Users can mark words they know, and these words will be removed from the learning list.
- **Persistent Learning State**: Saves progress between sessions by storing the words to learn in a CSV file.

## Requirements

- Python 3.x
- pandas library
- Tkinter (usually included with Python installations)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/flashy.git
   cd flashy
   ```

2. Install the required libraries:
   ```bash
   pip install pandas
   ```

3. Ensure the following directory structure:
   ```
   flashy/
   ├── data/
   │   ├── french_words.csv
   │   └── word_to_learn.csv (optional, will be created after first run if not present)
   ├── images/
   │   ├── card_front.png
   │   ├── card_back.png
   │   ├── wrong.png
   │   └── right.png
   └── main.py
   ```

## Usage

Run the application:
```bash
python main.py
```

## Code Overview

The main components of the application are as follows:

### Global Variables
- `BACKGROUND_COLOR`: Background color for the app.
- `card_choice`: Currently selected card.
- `to_learn`: List of words to learn.

### Functions
- `next_card()`: Selects a new card randomly and displays the French word.
- `flip_card()`: Flips the card to show the English translation after a delay.
- `is_known()`: Removes the known card from the list and updates the CSV file.

### Main Application
- Initializes the main window.
- Sets up the canvas for card display.
- Configures buttons for marking words as known or unknown.
- Starts the application loop.

## Contribution

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For any inquiries or issues, please open an issue on GitHub or contact me at Abelmekonn9@gmail.com.

---

Enjoy learning French with Flashy!
