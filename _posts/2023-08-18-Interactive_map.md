---
toc: true
comments: false
layout: post
title: game
description: 
type: hacks
courses: { compsci: {week: 3} }
---
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Guess the Number Game</title>
    <style>
        /* Add your CSS styles here */
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        h1 {
            color: #0074e4;
        }
        #message {
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Guess the Number Game</h1>
    <p>Guess a number between 1 and 100:</p>
    <input type="number" id="guess" min="1" max="100">
    <button id="submit">Submit Guess</button>
    <p id="message"></p>

    <script>
        // JavaScript code for the interactive game
        const randomNumber = Math.floor(Math.random() * 100) + 1; // Generate a random number between 1 and 100
        let attempts = 0;

        document.addEventListener("DOMContentLoaded", function () {
            const guessInput = document.getElementById("guess");
            const submitButton = document.getElementById("submit");
            const message = document.getElementById("message");

            submitButton.addEventListener("click", function () {
                const userGuess = parseInt(guessInput.value);
                if (isNaN(userGuess) || userGuess < 1 || userGuess > 100) {
                    message.textContent = "Please enter a valid number between 1 and 100.";
                    return;
                }

                attempts++;

                if (userGuess === randomNumber) {
                    message.textContent = `Congratulations! You guessed the number ${randomNumber} in ${attempts} attempts.`;
                    guessInput.disabled = true;
                    submitButton.disabled = true;
                } else if (userGuess < randomNumber) {
                    message.textContent = "Try a higher number.";
                } else {
                    message.textContent = "Try a lower number.";
                }
            });
        });
    </script>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>White Cursive Font on Purple Background</title>
    <style>
        body {
            background-color: light orange; /* Set background color to purple */
            color: black; /* Set text color to white */
            font-family: cursive; /* Use cursive font-family */
            font-size: 18px; /* Set the font size (adjust as needed) */
        }
    </style>