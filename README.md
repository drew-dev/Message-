<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }
        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        main {
            flex: 1;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
        .button-container {
            margin: 20px;
        }
        button {
            margin: 5px;
            padding: 10px;
            font-size: 16px;
        }
        #image-container {
            margin-top: 20px;
        }
        img {
            max-width: 100%;
            height: auto;
        }
    </style>
    <script>
        function displayImage(number) {
            // Hide the main button menu
            document.getElementById('button-container').style.display = 'none';

            // Display the image
            var imageContainer = document.getElementById('image-container');
            imageContainer.innerHTML = '<img src="image' + number + '.jpg" alt="Image ' + number + '">';
        }
    </script>
</head>
<body>
    <header>
        <h1>Welcome to Our Landing Page</h1>
    </header>
    <main>
        <div id="button-container" class="button-container">
            <button onclick="displayImage(1)">1</button>
            <button onclick="displayImage(2)">2</button>
            <button onclick="displayImage(3)">3</button>
            <button onclick="displayImage(4)">4</button>
            <button onclick="displayImage(5)">5</button>
            <button onclick="displayImage(6)">6</button>
            <button onclick="displayImage(7)">7</button>
        </div>
        <div id="image-container">
            <!-- The image will be displayed here -->
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Your Company. All rights reserved.</p>
    </footer>
</body>
</html>
