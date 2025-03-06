# Hangman Game

## Overview
Welcome to the Hangman Game! This is a simple React-based game where you try to guess a randomly selected word before running out of lives.

## Features
- Random word selection
- Visual hangman updates as incorrect guesses are made
- Single-letter input for guessing
- Game win/loss detection
- Option to start a new game

## How to Play
1. Enter a single letter into the input box.
2. Click **Search** to guess.
3. Correct guesses will reveal letters.
4. Incorrect guesses will decrease lives and update the hangman image.
5. The game ends when you either:
   - Guess all the letters correctly (**You Win!** 🎉)
   - Run out of lives (**Game Over!** ❌)

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (Latest LTS recommended)
- [npm](https://www.npmjs.com/) (Comes with Node.js)

### Steps to Run Locally
1. **Clone the Repository**
   ```sh
   git clone <your-repository-link>
   cd hangman
   ```
2. **Install Dependencies**
   ```sh
   npm install
   ```
3. **Start the Game**
   ```sh
   npm start
   ```
4. Open `http://localhost:3000` in your browser to play!

## Project Structure
```
├── public/
│   ├── noose.png
│   ├── upperBody.png
│   ├── upperandlowerbody.png
│   ├── 1arm.png
│   ├── botharms.png
│   ├── Dead.png
├── src/
│   ├── App.js
│   ├── HangmanGame.js
│   ├── SingleLetterSearchBar.js
│   ├── LetterBox.js
│   ├── index.js
│   ├── styles.css
└── README.md
```

## Troubleshooting
### Image Not Displaying?
- Ensure all image files are in the `public/` folder.
- Try restarting the server with `npm start`.

### `this.props.onSearch` Error?
- Ensure `SingleLetterSearchbar` receives `onSearch` as a prop from `HangmanGame.js`:
  ```jsx
  <SingleLetterSearchbar onSearch={this.handleLetterGuess} />
  ```
