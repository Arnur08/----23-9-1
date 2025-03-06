<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>8 Наурыз Құттықтау</title>
    <style>
        body {
            background-color: #87CEEB;
            color: #333;
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 20px;
        }
        h1 {
            color: blue;
        }
        .container {
            background-color: #4a6d7c;
            color: white;
            padding: 20px;
            border-radius: 10px;
            display: inline-block;
        }
        .firework {
            position: absolute;
            width: 5px;
            height: 5px;
            background-color: yellow;
            border-radius: 50%;
            animation: explode 1.5s ease-out infinite;
        }
        @keyframes explode {
            0% { transform: scale(1); opacity: 1; }
            100% { transform: scale(10); opacity: 0; }
        }
        .truck {
            width: 100px;
            position: absolute;
            bottom: 10px;
            left: -120px;
            animation: drive 5s linear infinite;
        }
        @keyframes drive {
            0% { left: -120px; }
            100% { left: 100%; }
        }
    </style>
</head>
<body>

    <h1>---- 23-9-1</h1>

    <div class="container">
        <p>Құрметті Ақсезім, Ақниет, Аружан, Ақмаржан, Аяулым, Аиназым, Береке, Жібек, Жанерке, Жансая, Жаннұр, Памбук, Ұлдана, Іңкәр, Закя және құрметті Фатима!</p>
        <p>Сіздерді 8 Наурыз - Халықаралық әйелдер күнімен шын жүректен құттықтаймыз!</p>
        <p>Сіздерге мықты денсаулық, шексіз бақыт және өмірлеріңіз жарқын болуын тілейміз!</p>
    </div>

    <img src="https://cdn-icons-png.flaticon.com/512/742/742751.png" class="truck" alt="Грузовик">

    <script>
        function createFirework() {
            let firework = document.createElement("div");
            firework.className = "firework";
            document.body.appendChild(firework);

            let x = Math.random() * window.innerWidth;
            let y = Math.random() * window.innerHeight;

            firework.style.left = x + "px";
            firework.style.top = y + "px";

            setTimeout(() => firework.remove(), 1500);
        }

        setInterval(createFirework, 300);
    </script>

</body>
</html>
