<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Whack-a-Mole Style Game</title>
</head>
<body>
<canvas id="whackCanvas" width="600" height="400"></canvas>
<script>
const canvas = document.getElementById("whackCanvas");
const ctx = canvas.getContext("2d");

let flowers = [];
let score = 0;
let gameInterval, flowerInterval;

function spawnFlower() {
  const flower = {
    x: Math.random() * (canvas.width - 40),
    y: Math.random() * (canvas.height - 40),
    size: 30,
    timeout: Date.now() + 2000 // Each flower lasts 2 seconds
  };
  flowers.push(flower);
}

function drawFlowers() {
  ctx.clearRect(0, 0, canvas.width, canvas.height);
  ctx.font = "20px Arial";
  ctx.fillText("Score: " + score, 10, 20);

  const now = Date.now();
  flowers = flowers.filter(flower => now < flower.timeout); // Remove expired flowers

  flowers.forEach(flower => {
    ctx.beginPath();
    ctx.arc(flower.x, flower.y, flower.size, 0, Math.PI * 2);
    ctx.fillStyle = "pink";
    ctx.fill();
    ctx.closePath();
  });
}

function checkHit(x, y) {
  flowers.forEach((flower, index) => {
    const distance = Math.sqrt((x - flower.x) ** 2 + (y - flower.y) ** 2);
    if (distance < flower.size) {
      flowers.splice(index, 1); // Remove flower if hit
      score += 1;
    }
  });
}

canvas.addEventListener("click", (event) => {
  const rect = canvas.getBoundingClientRect();
  const x = event.clientX - rect.left;
  const y = event.clientY - rect.top;
  checkHit(x, y);
});

function startWhackGame() {
  score = 0;
  flowers = [];
  gameInterval = setInterval(drawFlowers, 100);
  flowerInterval = setInterval(spawnFlower, 1000);
}

function stopWhackGame() {
  clearInterval(gameInterval);
  clearInterval(flowerInterval);
  alert("Game over! Final score: " + score);
}

startWhackGame();
setTimeout(stopWhackGame, 30000); // Game lasts 30 seconds
</script>
</body>
</html>