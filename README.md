<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Streaming Drama Korea - Study Group</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f0f0;
      margin: 0;
      padding: 20px;
      text-align: center;
    }
    h1 {
      color: #333;
    }
    .video-container {
      max-width: 720px;
      margin: auto;
    }
    iframe {
      width: 100%;
      height: 400px;
      border: none;
    }
    .episode-buttons {
      margin-top: 20px;
    }
    .episode-buttons button {
      padding: 10px 20px;
      margin: 5px;
      font-weight: bold;
      cursor: pointer;
      background-color: #ffcc00;
      border: none;
      border-radius: 5px;
    }
    .episode-buttons button:hover {
      background-color: #ffaa00;
    }
  </style>
</head>
<body>

  <h1>Drama Korea: Study Group</h1>

  <div class="video-container">
    <iframe id="player" src="https://gdriveplayer.to/embed2.php?link=LINK_EPISODE_1"></iframe>
  </div>

  <div class="episode-buttons">
    <button onclick="gantiEpisode('LINK_EPISODE_1')">Episode 1</button>
    <button onclick="gantiEpisode('LINK_EPISODE_2')">Episode 2</button>
    <button onclick="gantiEpisode('LINK_EPISODE_3')">Episode 3</button>
  </div>

  <script>
    function gantiEpisode(link) {
      document.getElementById("player").src = "https://gdriveplayer.to/embed2.php?link=" + link;
    }
  </script>

</body>
</html>
