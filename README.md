<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Hello My Love! ❤️</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #fff;
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            text-align: center;
            transition: background-color 0.5s; 
        }
        .container {
            max-width: 400px;
            padding: 20px;
        }
        img.main-image {
            max-width: 100%;
            height: auto;
            margin-bottom: 20px;
        }
        h2 {
            font-size: 2em;
            color: #C0392B; 
            margin-bottom: 30px;
        }
        h3.sad-text { /* Style baru untuk teks sedih */
            font-size: 1.5em;
            color: #C0392B; 
            margin-top: 20px;
            margin-bottom: 40px;
        }
        .button-group {
            margin-top: 30px;
        }
        .button-group button {
            background: none;
            border: 2px solid #C0392B;
            color: #C0392B;
            padding: 10px 25px;
            border-radius: 25px;
            font-size: 1em;
            font-weight: bold;
            cursor: pointer;
            margin: 0 10px;
            transition: background-color 0.3s, color 0.3s;
        }
        .button-group button:hover {
            background-color: #C0392B;
            color: #fff;
        }

        /* Styling untuk Tampilan "NO THANKS" */
        #sad-message {
            display: none; 
            background-color: #fff;
            padding: 20px;
        }
        #sad-message button {
            background: #C0392B;
            color: #fff;
            border: none;
        }
        #sad-message button:hover {
            background: #A93226;
        }
        
    </style>
</head>
<body>

    <div class="container">
        <div id="initial-prompt">
            
            <img src="79b321227c39e63cf7c816e21ac6df38.jpg" alt="Hello My Love!" class="main-image"/> 
            
            <h2>Yahoooo My Pokiee!<br>Do you want to see your gift?</h2>
            
            <div class="button-group">
                <button onclick="redirectToHBD()">YES PLEASE</button>
                <button onclick="showSadMessage()">NO THANKS</button>
            </div>
        </div>

        <div id="sad-message">
            
            <img src="5294fcd14c8330faa37082d32e963bfc.jpg" alt="Karakter Sedih" class="main-image"/> 
            
            <h3 class="sad-text">I promise you'll like it 😢</h3>
            
            <div class="button-group">
                <button onclick="showInitialPrompt()">TRY AGAIN</button>
            </div>
        </div>
    </div>

    <script>
        function redirectToHBD() {
            // Mengarahkan ke halaman utama ulang tahun
            window.location.href = "HBD.html"; 
        }

        function showSadMessage() {
            // Menampilkan pesan sedih dan menyembunyikan prompt awal
            document.getElementById('initial-prompt').style.display = 'none';
            document.getElementById('sad-message').style.display = 'block';
        }

        function showInitialPrompt() {
            // Menampilkan prompt awal kembali dan menyembunyikan pesan sedih
            document.getElementById('sad-message').style.display = 'none';
            document.getElementById('initial-prompt').style.display = 'block';
        }
    </script>
</body>
</html>
