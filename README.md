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

        .content p {
            font-size: 1.1rem;
            color: #ddd;
        }

        /* Sekcja wideo */
        .video-section {
            text-align: center;
            margin: 2rem 0;
        }

        .video-section iframe {
            width: 70%;
            height: 400px;
            border-radius: 12px;
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.7);
        }

        /* Stopka */
        footer {
            background-color: #1a1a1a;
            color: #ff4500;
            padding: 2rem;
            text-align: center;
            box-shadow: 0px -10px 20px rgba(0, 0, 0, 0.5);
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

        /* Ramka dla aktualizacji */
        .update-box {
            background-color: #1a1a1a;
            border: 2px solid #ff4500;
            border-radius: 10px;
            padding: 2rem;
            margin: 1.5rem auto;
            width: 80%;
            max-width: 800px;
            animation: zoomIn 0.5s ease-in-out;
        }

        @keyframes zoomIn {
            0% { transform: scale(0.8); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }

        .reaction-buttons {
            margin-top: 1rem;
        }

        .reaction-button {
            background-color: #ff4500;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 0.5rem 1rem;
            cursor: pointer;
            margin: 0 0.5rem;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .reaction-button:hover {
            background-color: #ff6347;
            transform: translateY(-3px);
        }

        .reaction-count {
            margin-left: 0.5rem;
        }

        .contact-section form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .contact-section input, .contact-section textarea {
            width: 80%;
            padding: 1rem;
            margin: 0.5rem 0;
            border: 2px solid #ff4500;
            border-radius: 5px;
            background-color: #2a2a2a;
            color: white;
        }

        .contact-section button {
            background-color: #ff4500;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 1rem 2rem;
            cursor: pointer;
            margin-top: 1rem;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .contact-section button:hover {
            background-color: #ff6347;
            transform: translateY(-3px);
        }

    </style>
</head>
<body>
    <header>
        <h1>Światmetina.pl</h1>
        <p>Najświeższe informacje o Metin2</p>
        <div class="nav">
            <a href="#news">Aktualności</a>
            <a href="#support">Wsparcie</a>
            <a href="#partners">Partnerzy</a>
            <a href="#contact">Kontakt</a>
        </div>
        <div class="wave"></div>
    </header>

    <div class="content">
        <h2 id="news">Aktualności</h2>
        <div class="update-box">
            <h3>Nowa aktualizacja Metin2!</h3>
            <p>Dodano nowe misje oraz postacie do gry. Uaktualnij swój klient, aby uzyskać dostęp do nowych treści.</p>
            <div class="reaction-buttons">
                <button class="reaction-button">👍</button>
                <span class="reaction-count">3</span>
                <button class="reaction-button">❤️</button>
                <span class="reaction-count">5</span>
            </div>
        </div>
        
        <div class="video-section">
            <h2>Filmy</h2>
            <iframe src="https://www.youtube.com/embed/your-video-id" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>

        <h2 id="support">Wsparcie</h2>
        <p>Aby uzyskać pomoc, skontaktuj się z nami przez formularz poniżej.</p>
    </div>

    <footer>
        <p>&copy; 2024 Światmetina.pl - Wszystkie prawa zastrzeżone</p>
    </footer>
</body>
</html>
