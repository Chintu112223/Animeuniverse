<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>My Anime Site</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>MyAnime</h1>
    <input type="text" id="searchInput" placeholder="Search anime...">
  </header>

  <main id="animeList">
    <!-- Anime Cards -->
    <div class="anime-card" data-title="Naruto">
      <img src="assets/naruto.jpg" alt="Naruto">
      <h3>Naruto</h3>
      <button onclick="playVideo('assets/naruto-ep1.mp4')">Watch</button>
    </div>
    <div class="anime-card" data-title="One Piece">
      <img src="assets/onepiece.jpg" alt="One Piece">
      <h3>One Piece</h3>
      <button onclick="playVideo('assets/onepiece-ep1.mp4')">Watch</button>
    </div>
    <!-- Add more anime here -->
  </main>

  <section id="videoPlayerSection" class="hidden">
    <video id="videoPlayer" controls></video>
    <button onclick="closePlayer()">Close</button>
  </section>

  <script src="script.js"></script>
</body>
</html>
