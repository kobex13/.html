<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>RPG Travel Map</title>
  <style>
    body { font-family: 'Arial', sans-serif; background: #1a1a1a; color: #fff; text-align: center; padding: 50px; }
    .map { display: flex; justify-content: center; align-items: center; flex-direction: column; gap: 40px; }
    .station { cursor: pointer; transition: transform 0.3s; }
    .station:hover { transform: scale(1.2); }
    .line { width: 4px; height: 40px; background: #fff; margin: 0 auto; }
    .info { margin-top: 20px; font-size: 1.2em; color: #0f0; }
  </style>
</head>
<body>
  <h1>RPG Travel Map</h1>
  <div class="map">
    <div class="station" onclick="showInfo('Village | $5 | 5min')">🏠</div>
    <div class="line"></div>
    <div class="station" onclick="showInfo('Forest | $10 | 10min')">🌲</div>
    <div class="line"></div>
    <div class="station" onclick="showInfo('River | $15 | 15min')">🌊</div>
    <div class="line"></div>
    <div class="station" onclick="showInfo('Castle | $20 | 20min')">🏰</div>
  </div>

  <div class="info" id="info">Select a location...</div>

  <script>
    function showInfo(text) {
      document.getElementById('info').innerText = text;
    }
  </script>
</body>
</html>
# .html
