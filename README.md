<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine Proposal</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            margin-top: 100px;
        }
        #question {
            font-size: 24px;
            margin-bottom: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1 id="question">WILL YOU BE MY VALENTINE Aryan? ❤️</h1>
    <button onclick="yesResponse()">Yes</button>
    <button id="noButton" onclick="noResponse()">No</button>

    <script>
        let noCount = 0;
        function noResponse() {
            noCount++;
            if (noCount === 1) {
                document.getElementById('question').innerText = "Please My Teddy 🙏";
            } else if (noCount === 2) {
                document.getElementById('question').innerText = "Please na baby, I love you ❤️";
            } else if (noCount === 3) {
                document.getElementById('question').innerText = "Shut up, you will be 😤❤️";
                document.getElementById('noButton').remove();
            }
        }
        function yesResponse() {
            document.getElementById('question').innerText = "Yay! I love you 😘❤️";
            document.getElementById('noButton').remove();
        }
    </script>
</body>
</html>
