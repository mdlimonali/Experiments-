<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quote Animation</title>
    <style>
        body {
            background-color: #1a1a1a;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: 'Arial', sans-serif;
        }

        .container {
            text-align: center;
            color: white;
            font-size: 32px;
            max-width: 80%;
        }

        #quote {
            font-size: 40px;
            line-height: 1.5;
            letter-spacing: 2px;
            color: lightgreen;
            opacity: 0;
            transform: translateY(50px);
            animation: fadeIn 1s forwards, scaleUp 1.5s ease-in-out infinite alternate;
        }

        /* Fade-in animation */
        @keyframes fadeIn {
            0% {
                opacity: 0;
                transform: translateY(50px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Scale-up effect for the quote */
        @keyframes scaleUp {
            0% {
                transform: scale(1);
            }
            100% {
                transform: scale(1.05);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1 id="quote"></h1>
    </div>

    <script>
        const quoteText = "You are your own worst enemy. You waste precious time by dreaming of the future instead of engaging yourself in the present. Since nothing seems urgent to you, you are just only half involved in what you do.";

        let index = 0;
        const quoteElement = document.getElementById('quote');

        // Function to type out the quote with delay
        function typeQuote() {
            if (index < quoteText.length) {
                quoteElement.textContent += quoteText.charAt(index);
                index++;
                setTimeout(typeQuote, 100); // Delay between characters
            }
        }

        window.onload = typeQuote;  // Trigger typing animation on page load
    </script>
</body>
</html>
