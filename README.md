<!DOCTYPE html>
<html>
<head>
    <title>Em andamento...</title>
    <style>
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        @keyframes typing {
            0% {
                content: "";
            }
            25% {
                content: ".";
            }
            50% {
                content: "..";
            }
            75% {
                content: "...";
            }
            100% {
                content: "";
            }
        }
        #typing-text {
            font-size: 48px;
            font-weight: bold;
        }
        #ellipsis::after {
            content: "";
            animation: typing 1s steps(4) infinite;
        }
    </style>
</head>
<body>
    <div id="typing-text">Em andamento<span id="ellipsis"></span></div>
</body>
</html>
