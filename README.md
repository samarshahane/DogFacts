# DogFacts
The Website states 10 funny facts of dogs
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Funny Dog Facts</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            color: #333;
            text-align: center;
            padding: 50px;
        }
        #fact {
            font-size: 1.5em;
            margin: 20px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #fff;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            background-color: #09df10;
            color: rgb(0, 0, 0);
        }
        button:hover {
            background-color: #00ff11;
        }
    </style>
</head>
<body>

    <h1>Funny Dog Facts</h1>
    <div id="fact">Click the button to see a funny dog fact!</div>
    <button onclick="showFact()">Show Fact</button>

    <script>
        const facts = [
            "Dogs can smell your feelings. So if you're sad, they might just bring you their favorite toy to cheer you up!",
            "A dog's favorite game is 'fetch,' but they often forget what they were fetching halfway through.",
            "Dogs have a unique talent for making you feel guilty when you leave the house, even if it's just for a minute.",
            "Your dog thinks you're a superhero because you can open cans and doors with ease!",
            "Dogs will always choose the most inconvenient spot to lay down, especially if it's right in front of the fridge.",
            "If you ever need a personal trainer, just get a dog. They’ll make sure you get your daily exercise by chasing them around!",
            "Dogs have a sixth sense for knowing when you're about to eat something delicious and will magically appear by your side.",
            "Your dog believes that every time you leave the house, you're going on an adventure without them.",
            "Dogs can turn any mundane object into a toy, including your favorite pair of shoes!",
            "When you talk to your dog, they might not understand the words, but they definitely understand the tone and will respond accordingly."
        ];

        let currentFactIndex = 0;

        function showFact() {
            if (currentFactIndex < facts.length) {
                document.getElementById('fact').innerText = facts[currentFactIndex];
                currentFactIndex++;
            } else {
                document.getElementById('fact').innerText = "No more facts available!";
            }
        }
    </script>

</body>
</html>
  
