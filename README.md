<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>8 Наурыз Құтты Болсын!</title>
    <style>
        body {
            background-color: #87CEEB;
            text-align: center;
            font-family: Arial, sans-serif;
            overflow: hidden;
        }
        .truck {
            width: 200px;
            position: absolute;
            left: -250px;
            bottom: 50px;
            animation: drive 4s ease-out forwards;
        }
        @keyframes drive {
            to {
                left: 50%;
                transform: translateX(-50%);
            }
        }
        .message {
            opacity: 0;
            font-size: 24px;
            color: white;
            background: rgba(0, 0, 0, 0.5);
            display: inline-block;
            padding: 15px;
            border-radius: 10px;
            margin-top: 50px;
            animation: fadeIn 2s ease-in 4s forwards;
        }
        @keyframes fadeIn {
            to {
                opacity: 1;
            }
        }
        .lights {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
            opacity: 0;
            animation: fadeIn 2s ease-in 3s forwards;
        }
        .light {
            width: 20px;
            height: 20px;
            background: yellow;
            border-radius: 50%;
            box-shadow: 0 0 10px yellow;
        }
    </style>
</head>
<body>

    <img src="https://i.imgur.com/F5oNnvO.png" alt="Truck" class="truck">
    
    <div class="lights">
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
    </div>

    <div class="message">
        <p>Құрметті Ақсезім, Ақниет, Аружан, Ақмаржан, Аяулым, Аиназым, Береке, Жібек, Жанерке, Жансая, Жаннұр, Памбух, Ұлдана, Іңкәр, Закия және құрметті Фатима!</p>
        <p>Сіздерді 8 Наурыз - Халықаралық әйелдер күнімен шын жүректен құттықтаймыз!</p>
        <p>Сіздерге мықты денсаулық, шексіз бақыт және өмірлеріңіз жарқын болуын тілейміз!</p>
    </div>

</body>
</html>
