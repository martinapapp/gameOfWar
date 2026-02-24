# Game of War

![JS Badge](https://img.shields.io/badge/Learning-JavaScript-yellow)
![API Badge](https://img.shields.io/badge/API-Scrimba-blue)

This is a project I built to practice working with APIs. I learned how to manage state across multiple fetch calls and how to implement game logic based on data returned from a server.

## Index

- [About](#about)
- [Usage](#usage)
- [Development](#development)
- [Contrubution](#contribution)
- [License](#license)

---

## About
Game of War is a digital card game that pits the user against a computer. The main goal was to learn how to:

- Use fetch() to generate a new deck and retrieve a unique deck_id.
- Use template literals to inject dynamic image elements based on API data.
- Implement a scoring system by comparing indices of a custom value array.
- Handle game-over states by disabling buttons when the API reports zero cards remaining.

It's currently hooked up to the Scrimba Deck of Cards API to handle shuffling and drawing.


## Usage

### Installation
Since this project uses **Vite**, you'll need to install the dependencies first:

1. Clone the repo.
2. Run `npm install` to get Vite set up
3. Run `npm run dev` to start the local server
4. Click the link in your terminal (usually http://localhost:5173) to start the game

### Commands
I'm using Vite to make development faster. Here are the main scripts I use:

`npm run dev` - Starts the project so I can see changes live.

`npm run build` - Prepares the project for the real world (deployment).

`npm run preview` - Lets me check the build version locally.

## Development

 ### Pre-Requisites: 
 - text editor
 - browser

### File Structure

| No | File Name | What it does |
| ---- | ---------- | ------------- |
|1|index.html|The game board layout including score tracking.|
|2|index.css|Styles for card positioning and layout.|
|3|index.js| The logic for API calls, card comparison, and score tracking.|
|4|img/| Contains the background table image |


### Build
The app uses a global deckId variable to maintain the session. I created a helper function determineCardWinner that maps card values (like "JACK", "QUEEN") to an array index to calculate which card is higher. Once the remaining count from the API hits 0, the "Draw" button is disabled and a final winner is declared based on the total scores.

## Contribution
1. Found a bug? Open an issue and I'll try to fix it.
2. Advice? If you know a cleaner way to handle the tie-breaker ("War") logic, let me know!

### Guideline
I'm trying to keep this as "Vanilla" as possible—no frameworks allowed yet! I want to really understand the basics here.

## License
Feel free to use this for your own practice!  **MIT**  License.