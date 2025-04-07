# 2-player-game-hub
<!DOCTYPE html>
<html>
<head>
  <title>2 Player Game Hub</title>
  <style>
    body {
      font-family: sans-serif;
      background: #f0f0f0;
      text-align: center;
    }
    h1 {
      color: #333;
    }
    .game-list {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .game-card {
      background: white;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      transition: transform 0.2s;
    }
    .game-card:hover {
      transform: scale(1.05);
      cursor: pointer;
    }
    iframe {
      width: 100%;
      height: 400px;
      border: none;
    }
    .game-display {
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <h1>2 Player Game Hub</h1>
  <div class="game-list" id="gameList"></div>
  <div class="game-display">
    <iframe id="gameFrame" src=""></iframe>
  </div>

  <script>
    const games = [
      { name: "Tap Race", url: "https://2pgame.netlify.app/game1" },
      { name: "Key Duel", url: "https://2pgame.netlify.app/game2" },
      { name: "Ping Pong", url: "https://2pgame.netlify.app/game3" },
      { name: "Tank Battle", url: "https://2pgame.netlify.app/game4" },
      { name: "Basket Shoot", url: "https://2pgame.netlify.app/game5" },
      { name: "Fencing Match", url: "https://2pgame.netlify.app/game6" },
      { name: "Memory War", url: "https://2pgame.netlify.app/game7" },
      { name: "Dino Dash", url: "https://2pgame.netlify.app/game8" },
      { name: "Fruit Chop", url: "https://2pgame.netlify.app/game9" },
      { name: "Word Fight", url: "https://2pgame.netlify.app/game10" },
      { name: "Math Race", url: "https://2pgame.netlify.app/game11" },
      { name: "Typing War", url: "https://2pgame.netlify.app/game12" },
      { name: "Jetpack Jump", url: "https://2pgame.netlify.app/game13" },
      { name: "Ball Balance", url: "https://2pgame.netlify.app/game14" },
      { name: "Rocket Escape", url: "https://2pgame.netlify.app/game15" },
      { name: "Emoji Battle", url: "https://2pgame.netlify.app/game16" },
      { name: "Mirror Duel", url: "https://2pgame.netlify.app/game17" },
      { name: "Light Speed", url: "https://2pgame.netlify.app/game18" },
      { name: "Arrow Clash", url: "https://2pgame.netlify.app/game19" },
      { name: "Tic Tac Pro", url: "https://2pgame.netlify.app/game20" },
      { name: "Code Breaker", url: "https://2pgame.netlify.app/game21" },
      { name: "Slide War", url: "https://2pgame.netlify.app/game22" },
      { name: "Bounce Fight", url: "https://2pgame.netlify.app/game23" },
      { name: "Snowball Duel", url: "https://2pgame.netlify.app/game24" },
      { name: "Maze Race", url: "https://2pgame.netlify.app/game25" },
      { name: "Flip Challenge", url: "https://2pgame.netlify.app/game26" },
      { name: "Stack Tower", url: "https://2pgame.netlify.app/game27" },
      { name: "Jump Clash", url: "https://2pgame.netlify.app/game28" },
      { name: "Aim & Shoot", url: "https://2pgame.netlify.app/game29" },
      { name: "Speed Tap", url: "https://2pgame.netlify.app/game30" }
    ];

    const gameList = document.getElementById('gameList');
    const gameFrame = document.getElementById('gameFrame');

    games.forEach(game => {
      const div = document.createElement('div');
      div.className = 'game-card';
      div.innerText = game.name;
      div.onclick = () => {
        gameFrame.src = game.url;
      };
      gameList.appendChild(div);
    });
  </script>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>2 Player Game Hub</title>
  <style>
    body {
      font-family: sans-serif;
      background: #f0f0f0;
      text-align: center;
    }
    h1 {
      color: #333;
    }
    .game-list {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .game-card {
      background: white;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      transition: transform 0.2s;
    }
    .game-card:hover {
      transform: scale(1.05);
      cursor: pointer;
    }
    iframe {
      width: 100%;
      height: 400px;
      border: none;
    }
    .game-display {
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <h1>2 Player Game Hub</h1>
  <div class="game-list" id="gameList"></div>
  <div class="game-display">
    <iframe id="gameFrame" src=""></iframe>
  </div>

  <script>
    const games = [
      { name: "Tap Race", url: "https://2pgame.netlify.app/game1" },
      { name: "Key Duel", url: "https://2pgame.netlify.app/game2" },
      { name: "Ping Pong", url: "https://2pgame.netlify.app/game3" },
      { name: "Tank Battle", url: "https://2pgame.netlify.app/game4" },
      { name: "Basket Shoot", url: "https://2pgame.netlify.app/game5" },
      { name: "Fencing Match", url: "https://2pgame.netlify.app/game6" },
      { name: "Memory War", url: "https://2pgame.netlify.app/game7" },
      { name: "Dino Dash", url: "https://2pgame.netlify.app/game8" },
      { name: "Fruit Chop", url: "https://2pgame.netlify.app/game9" },
      { name: "Word Fight", url: "https://2pgame.netlify.app/game10" },
      { name: "Math Race", url: "https://2pgame.netlify.app/game11" },
      { name: "Typing War", url: "https://2pgame.netlify.app/game12" },
      { name: "Jetpack Jump", url: "https://2pgame.netlify.app/game13" },
      { name: "Ball Balance", url: "https://2pgame.netlify.app/game14" },
      { name: "Rocket Escape", url: "https://2pgame.netlify.app/game15" },
      { name: "Emoji Battle", url: "https://2pgame.netlify.app/game16" },
      { name: "Mirror Duel", url: "https://2pgame.netlify.app/game17" },
      { name: "Light Speed", url: "https://2pgame.netlify.app/game18" },
      { name: "Arrow Clash", url: "https://2pgame.netlify.app/game19" },
      { name: "Tic Tac Pro", url: "https://2pgame.netlify.app/game20" },
      { name: "Code Breaker", url: "https://2pgame.netlify.app/game21" },
      { name: "Slide War", url: "https://2pgame.netlify.app/game22" },
      { name: "Bounce Fight", url: "https://2pgame.netlify.app/game23" },
      { name: "Snowball Duel", url: "https://2pgame.netlify.app/game24" },
      { name: "Maze Race", url: "https://2pgame.netlify.app/game25" },
      { name: "Flip Challenge", url: "https://2pgame.netlify.app/game26" },
      { name: "Stack Tower", url: "https://2pgame.netlify.app/game27" },
      { name: "Jump Clash", url: "https://2pgame.netlify.app/game28" },
      { name: "Aim & Shoot", url: "https://2pgame.netlify.app/game29" },
      { name: "Speed Tap", url: "https://2pgame.netlify.app/game30" }
    ];

    const gameList = document.getElementById('gameList');
    const gameFrame = document.getElementById('gameFrame');

    games.forEach(game => {
      const div = document.createElement('div');
      div.className = 'game-card';
      div.innerText = game.name;
      div.onclick = () => {
        gameFrame.src = game.url;
      };
      gameList.appendChild(div);
    });
  </script>
</body>
</html>
