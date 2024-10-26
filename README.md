<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Światmetina.pl</title>
    <style>
        /* Import czcionek z Google Fonts */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@700&family=Roboto:wght@400;500&family=Orbitron:wght@400;700&display=swap');

        /* Podstawowe style */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #fff;
        }

        /* Stylowanie nagłówka */
        header {
            position: relative;
            background-color: #1a1a1a;
            color: white;
            text-align: center;
            padding: 2rem 0;
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.8);
            border-bottom: 5px solid #000;
            animation: slideDown 0.5s ease-in-out;
        }

        @keyframes slideDown {
            0% { transform: translateY(-50px); opacity: 0; }
            100% { transform: translateY(0); opacity: 1; }
        }

        header h1 {
            font-family: 'Poppins', sans-serif;
            font-size: 2.5rem;
            margin: 0;
            text-transform: uppercase;
            color: #ff4500;
            background: linear-gradient(90deg, #ff4500, #ff6347);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            letter-spacing: 2px;
            text-shadow: 0px 5px 10px rgba(255, 69, 0, 0.5), 0 0 20px rgba(255, 0, 0, 0.7);
        }

        header p {
            font-size: 1.2rem;
            color: #ccc;
            margin-top: 1rem;
        }

        /* Sekcja nawigacji w nagłówku */
        .nav {
            display: flex;
            justify-content: center;
            margin: 2rem 0;
        }

        .nav a {
            color: #ffffff;
            text-decoration: none;
            font-size: 1.5rem;
            font-family: 'Orbitron', sans-serif;
            padding: 1rem 2rem;
            margin: 0 40px;
            background-color: rgba(255, 69, 0, 0.9);
            border-radius: 20px;
            transition: background-color 0.3s ease, box-shadow 0.3s ease, transform 0.3s ease;
            box-shadow: 0px 5px 10px rgba(255, 69, 0, 0.7);
        }

        .nav a:hover {
            background-color: #ff6347;
            box-shadow: 0px 10px 20px rgba(255, 69, 0, 0.9);
            transform: translateY(-5px);
        }

        /* Główna treść */
        .content {
            text-align: center;
            padding: 3rem;
        }

        .content h2 {
            font-size: 2rem;
            color: #ff4500;
            background: linear-gradient(90deg, #ff4500, #ff6347);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0px 5px 10px rgba(255, 69, 0, 0.5), 0 0 20px rgba(255, 0, 0, 0.7);
        }

        /* Zaokrąglony dół dla nagłówka */
        .wave {
            position: relative;
            top: 0;
            width: 100%;
            height: 100px;
            background-color: #121212;
            border-bottom-left-radius: 100% 50px;
            border-bottom-right-radius: 100% 50px;
        }

        /* Reszta stylów zostaje bez zmian */
    </style>
</head>
<body>
    <header>
        <h1>Światmetina.pl</h1>
        <p>Najświeższe informacje o Metin2</p>
        <div class="nav">
            <a href="#news">Filmy</a>
            <a href="#updates">Aktualności</a>
            <a href="#support">Wsparcie</a>
            <a href="#partners">Partnerzy</a>
            <a href="#contact">Kontakt</a>
        </div>
        <div class="wave"></div> <!-- Zaokrąglony dół dla nagłówka -->
    </header>

    <div class="content">
        <h2 id="news">Aktualności</h2>
        <!-- Sekcje z aktualizacjami i treścią -->
    </div>

    <footer>
        <p>&copy; 2024 Światmetina. Wszystkie prawa zastrzeżone.</p>
    </footer>
</body>
</html>
