<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pure Leaf Contest</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
            background-color: #f4f4f4;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            max-width: 400px;
            margin: auto;
        }
        input {
            width: 80%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background: green;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        .message {
            margin-top: 20px;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Enter Your Winning Code</h2>
        <input type="text" id="codeInput" placeholder="Enter code here...">
        <br>
        <button onclick="checkCode()">Submit</button>
        <p class="message" id="message"></p>
    </div>

    <script>
        function checkCode() {
            const correctCode = "PUREWIN2025";
            const userCode = document.getElementById("codeInput").value;
            const messageElement = document.getElementById("message");
            
            if (userCode === correctCode) {
                messageElement.style.color = "green";
                messageElement.textContent = "Congratulations! You've won a year's supply of Pure Leaf tea!";
            } else {
                messageElement.style.color = "red";
                messageElement.textContent = "Invalid code. Please try again.";
            }
        }
    </script>
</body>
</html>
