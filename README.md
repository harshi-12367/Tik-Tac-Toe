<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Itim&display=swap" rel="stylesheet">
    <script src="./index.js"></script>
    <title>Tic Tac Toe</title>
</head>
<body>
    <main class="background">
        <section class="title">
            <h1>Tic Tac Toe</h1>
        </section>
        <section class="display">
            Player <span class="display-player playerX">X</span>'s turn
        </section>
        <section class="container">
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
            <div class="tile"></div>
        </section>
        <section class="display announcer hide"></section>
        <section class="controls">
            <button id="reset">Reset</button>
        </section>
    </main>
</body>
</html>
/* Reset default browser styles */
* {
    padding: 0;
    margin: 0;
    font-family: 'Itim', cursive;
}

/* Style for the board using CSS grid */
.container {
    display: grid;
    grid-template-columns: repeat(3, 33%);
    grid-template-rows: repeat(3, 33%);
    gap: 2px;
}

.tile {
    border: 2px solid #000;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 24px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.tile:hover {
    background-color: #f0f0f0;
}

/* Other styling as needed */
/* ... */
// Add your game logic here
// You'll need to handle player turns, check for wins, and update the display
// Example: When a tile is clicked, update the board and check for a winner

// Example event listener for a tile click:
document.querySelectorAll('.tile').forEach(tile => {
    tile.addEventListener('click', () => {
        // Handle tile click logic
        // Update the display, check for wins, etc.
    });
});

// Example reset button functionality:
document.getElementById('reset').addEventListener('click', () => {
    // Reset the game state
    // Clear the board, reset player turns, etc.
});


