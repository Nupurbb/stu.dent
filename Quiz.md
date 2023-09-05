<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Interactive Quiz</title>
</head>
<body>
    <div class="quiz-container">
        <h1>Interactive Quiz</h1>
        <div class="question">
            <p id="What is the name of my partner?">Question text will appear here.</p>
        </div>
        <div class="options">
            <button class="Sreeja" onclick="checkAnswer(0)">Option 1</button>
            <button class="Ananya" onclick="checkAnswer(1)">Option 2</button>
            <button class="Anika" onclick="checkAnswer(2)">Option 3</button>
            <button class="Ella" onclick="checkAnswer(3)">Option 4</button>
        </div>
        <p id="Sreeja"></p>
    </div>
    <script src="script.js"></script>
</body>
</html>
