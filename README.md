<!-- 3reo TV - Home Page Layout -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SYNC with 3REO</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <div class="logo">
      <img src="https://i.imgur.com/KToebw4.jpg" alt="3reo Logo">
    </div>
    <div class="time-display">
      <span class="time-minus-30">[CT - 30]</span>
      <span class="current-time">[CURRENT TIME]</span>
      <span class="time-plus-30">[CT + 30]</span>
    </div>
    <h1>3reo.com</h1>
  </header>

  <main>
    <div class="tv-player-fixed">
      <iframe id="tv-embed" src="https://www.youtube.com/embed/[videoID]" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>

    <div class="channel-list">
      <h2>Free Live Cable TV Channels & Movies</h2>
      <table class="channel-grid">
        <thead>
          <tr>
            <th>Logo</th>
            <th>#Channel</th>
            <th>#C</th>
            <th>Now Playing</th>
            <th>AC</th>
          </tr>
        </thead>
        <tbody>
          <!-- Dynamic Channel Rows Populated by Node.js Server -->
        </tbody>
      </table>
    </div>
  </main>

  <footer>
    <div class="global-chat">
      <iframe src="https://toonreboot.chat/embed" frameborder="0"></iframe>
    </div>
  </footer>

  <script src="client.js"></script>
</body>
</html>

/* CLIENT.JS */
// Hotkey bindings
window.addEventListener('keydown', function(e) {
  switch(e.key) {
    case 'ArrowUp':
      // Increase volume
      break;
    case 'ArrowDown':
      // Decrease volume
      break;
    case 'ArrowLeft':
      // Previous channel
      break;
    case 'ArrowRight':
      // Next channel
      break;
  }
});
