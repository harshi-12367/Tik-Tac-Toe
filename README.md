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

