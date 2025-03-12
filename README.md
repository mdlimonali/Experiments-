<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heading Example</title>
    <style>
        body {
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .animated-heading {
            color: green;
            font-size: 50px;
            font-family: Arial, sans-serif;
            text-align: center;
            animation: zoomIn 3s ease-in-out infinite;
        }

        @keyframes zoomIn {
            0% {
                transform: scale(0);
                opacity: 0;
            }
            50% {
                transform: scale(1.1);
                opacity: 1;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <h1 class="animated-heading">HE WHO DOES NOTHING MAKES NO MISTAKE</h1>
</body>
</html>
<link rel="stylesheet" href="styles.css">
