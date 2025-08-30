<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>နှလုံးသားနှင့်စာသား</title>
    <style>
        body {
            background-color: black;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .heart {
            position: relative;
            width: 100px;
            height: 90px;
            background-color: red;
            transform: rotate(-45deg);
            margin-right: 50px;
            animation: fade 2s infinite;
        }
        .heart:before,
        .heart:after {
            content: "";
            position: absolute;
            width: 100px;
            height: 90px;
            background-color: red;
            border-radius: 50%;
            animation: fade 2s infinite;
        }
        .heart:before {
            top: -50px;
            left: 0;
        }
        .heart:after {
            left: 50px;
            top: 0;
        }
        .text {
            color: red;
            font-family: Arial, sans-serif;
            font-size: 25px;
            font-style: italic;
            font-weight: bold;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
        @keyframes fade {
            0% { opacity: 1; }
            50% { opacity: 0; }
            100% { opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="heart"></div>
    <div class="text">I LOVE YOU</div>
</body>
</html>
