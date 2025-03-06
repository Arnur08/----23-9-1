<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>8 Наурыз Құттықтау</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            overflow: hidden;
            font-family: Arial, sans-serif;
        }

        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: red;
            border-radius: 50%;
            opacity: 0.7;
            animation: fall linear infinite;
        }

        @keyframes fall {
            0% { transform: translateY(-10vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }

        .message-box {
            display: none;
            padding: 20px;
            background-color: #ff69b4;
            color: white;
            text-align: center;
            font-size: 1.5em;
            border-radius: 10px;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
            width: 80%;
            max-width: 600px;
        }

        h1 {
            color: #ff1493;
            text-align: center;
            font-size: 2em;
        }
    </style>
</head>
<body>

    <h1>Құрметті ханымдар!</h1>

    <script>
        function createConfetti() {
            for (let i = 0; i < 100; i++) {
                let confetti = document.createElement("div");
                confetti.className = "confetti";
                confetti.style.left = Math.random() * 100 + "vw";
                confetti.style.animationDuration = (Math.random() * 3 + 2) + "s";
                confetti.style.backgroundColor = Math.random() < 0.5 ? "red" : "pink";
                document.body.appendChild(confetti);

                setTimeout(() => {
                    confetti.remove();
                }, 5000);
            }
        }

        function showMessage() {
            let messageBox = document.createElement("div");
            messageBox.className = "message-box";
            messageBox.innerHTML = `
                <p><b>Құрметті арулар!</b></p>
                <p>Сіздерді 8 Наурыз - Халықаралық әйелдер күнімен шын жүректен құттықтаймыз!</p>
                <p>Сіздерге мықты денсаулық, шексіз бақыт және өмірлеріңіз жарқын болуын тілейміз!</p>
            `;
            document.body.appendChild(messageBox);
            messageBox.style.display = "block";
        }

        setTimeout(createConfetti, 500);
        setTimeout(showMessage, 4000);
    </script>

</body>
</html>
