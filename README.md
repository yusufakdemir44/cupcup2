<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>İlaç</title>
  <style>
    body {
      font-family: sans-serif;
      background: linear-gradient(135deg, #ffeaea, #ffd6d6);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      text-align: center;
      margin: 0;
    }
    h1 {
      font-size: 26px;
      color: #333;
      margin-bottom: 20px;
    }
    button {
      padding: 14px 28px;
      font-size: 18px;
      background-color: #ff5e78;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Şu an ihtiyacın olan şey: <strong>İlaç</strong></h1>
  <button onclick="playSong()">Başlat</button>

  <audio id="music" src="kenan-dogulu-ara-beni.mp3"></audio>

  <script>
    function playSong() {
      const audio = document.getElementById("music");
      audio.play().catch(error => {
        alert("Ses oynatılamadı. Tarayıcı izin vermiyor olabilir.");
        console.error(error);
      });
    }
  </script>
</body>
</html>
