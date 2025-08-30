<!DOCTYPE html>
<html>
<head>
    <title>Love Site</title>
    <style>
        .heart {
            position: absolute;
            width: 100px;
            height: 90px;
            background: red;
            transform: rotate(-45deg);
            animation: beat 1s infinite;
        }
        .heart:before,
        .heart:after {
            content: "";
            position: absolute;
            width: 100px;
            height: 90px;
            background: red;
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
        @keyframes beat {
            0% { transform: scale(1) rotate(-45deg); }
            50% { transform: scale(1.2) rotate(-45deg); }
            100% { transform: scale(1) rotate(-45deg); }
        }
    </style>
</head>
<body>
    <div class="heart"></div>
    <p>I Love You</p>
</body>
</html>
