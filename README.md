<!DOCTYPE html>
<html>
<head>
    <title>Google Drive</title> <!-- Tab Cloak Name -->
    <link rel="icon" href="https://ssl.gstatic.com"> <!-- Google Drive Icon -->
    <style>
        body { background: #121212; color: white; font-family: sans-serif; text-align: center; }
        .game-card { border: 1px solid #444; padding: 10px; margin: 10px; display: inline-block; cursor: pointer; }
        iframe { width: 100%; height: 600px; border: none; display: none; }
    </style>
</head>
<body>
    <h1>My Private Projects</h1>
    <div id="gallery">
        <div class="game-card" onclick="play('https://michuscrypt.github.io')">Game Portal 1</div>
        <div class="game-card" onclick="play('https://algebra.icu')">Math Practice (Games)</div>
    </div>
    <iframe id="player"></iframe>

    <script>
        function play(url) {
            document.getElementById('gallery').style.display = 'none';
            let f = document.getElementById('player');
            f.style.display = 'block';
            f.src = url;
        }
    </script>
</body>
</html>
