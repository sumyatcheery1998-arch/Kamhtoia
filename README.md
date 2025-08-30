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
            flex-direction: column;
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
        }
        .heart:before,
        .heart:after {
            content: "";
            position: absolute;
            width: 100px;
            height: 90px;
            background-color: red;
            border-radius: 50%;
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
            margin-top: 20px; /* နှလုံးပုံနှင့် စာသားကြား အကွာအဝေး */
        }
    </style>
</head>
<body>
    <div class="heart"></div>
    <div class="text">I LOVE YOU</div>
</body>
</html>
