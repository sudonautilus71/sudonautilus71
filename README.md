<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Web</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }

        header {
            background-color: #0078d7;
            color: white;
            padding: 1em 0;
            text-align: center;
        }

        main {
            padding: 2em;
            text-align: center;
        }

        button {
            background-color: #0078d7;
            color: white;
            border: none;
            padding: 0.5em 1em;
            font-size: 1em;
            cursor: pointer;
            border-radius: 5px;
        }

        button:hover {
            background-color: #005bb5;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Simple Web</h1>
    </header>
    <main>
        <p id="welcome-message">This is a simple website with HTML, CSS, and JavaScript.</p>
        <button id="change-text-btn">Change Text</button>
    </main>
    <footer>
        <p>&copy; 2024 Simple Web</p>
    </footer>
    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const button = document.getElementById("change-text-btn");
            const message = document.getElementById("welcome-message");

            button.addEventListener("click", () => {
                message.textContent = "You clicked the button!";
            });
        });
    </script>
</body>
</html>
