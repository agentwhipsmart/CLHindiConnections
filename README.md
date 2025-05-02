
# Hindi Connections Game

A web-based implementation of a word categorization game in Hindi, inspired by the NYT Connections game. Players must group Hindi words into their correct categories while managing limited attempts.

## Features

- **Multiple Word Sets**: Over 23 unique Hindi word sets with various categories
- **Progressive Difficulty**: Categories are color-coded by difficulty:
  - Yellow (Easiest)
  - Green (Medium-Easy)
  - Blue (Difficult)
  - Purple (Most Difficult)
- **User Progress Tracking**: Tracks completion status, mistakes, and game duration
- **Statistics Dashboard**: View detailed game statistics for all players
- **Multiple Game Sessions**: Players can play multiple distinct games with different word sets

## How to Play

1. Register with your name, age, and profession
2. You'll see a 4x4 grid of Hindi words
3. Select four words that you think belong to the same category
4. Click "Submit Guess" to check if your grouping is correct
5. You have 4 attempts before game over
6. Complete the game by finding all four categories

## Technical Details

- Built with Flask (Python web framework)
- Uses session management for game state
- Responsive design with HTML/CSS
- Data persistence using CSV for statistics

## Game Rules

- Each game has exactly four categories
- Each category contains exactly four words
- Players get four attempts to find all categories
- A hint appears when 3 out of 4 selected words are from the same category
- Game ends when all categories are found or attempts are exhausted

## Routes

- `/`: Registration page
- `/game`: Main game interface
- `/stats`: Statistics dashboard
- `/submit_guess`: API endpoint for word submission

## Development

The project uses Poetry for dependency management. Main dependencies:
- Flask
- Flask-CORS
- Streamlit (for future features)

## Data Structure

Game data is stored in `categories.py` with multiple Hindi word sets, each containing four categories with four words each.

## Statistics Tracking

The game tracks:
- Player information
- Completion status
- Number of mistakes
- Game duration
- Accuracy percentage
- Total and correct guesses

  ## Files
  The Templates Folder contains index, stats and register HTML documents to collect data from the players.
  The main.py contains the main code for the game play. The categories.py file contains the dataset consisting of 23 puzzles.
  The game_data file contains the game-play data collected. 

Created by [Akankshya Mishra] on Replit
