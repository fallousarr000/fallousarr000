- 👋 Hi, I’m @fallousarr000
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!--<!DOCTYPE html>
<html>
<head>
    <title>Mini Jeu de Voiture</title>
    <style>
        canvas {
            display: block;
            margin: auto;
            background: #f3f3f3;
            border: 1px solid #d3d3d3;
        }
    </style>
</head>
<body>
    <canvas id="gameCanvas" width="400" height="600"></canvas>
    <script>
        const canvas = document.getElementById('gameCanvas');
        const context = canvas.getContext('2d');

        const carWidth = 50;
        const carHeight = 100;
        const roadWidth = canvas.width;
        const roadHeight = canvas.height;

        let carX = (roadWidth - carWidth) / 2;
        const carY = roadHeight - carHeight - 10;
        const carSpeed = 5;

        let obstacles = [];
        const obstacleWidth = 50;
        const obstacleHeight = 100;
        const obstacleSpeed = 2;

        document.addEventListener('keydown', function(event) {
            if (event.key === 'ArrowLeft' && carX > 0) {
                carX -= carSpeed;
            } else if (event.key === 'ArrowRight' && carX < roadWidth - carWidth) {
                carX += carSpeed;
            }
        });

        function drawCar() {
            context.fillStyle = 'blue';
            context.fillRect(carX, carY, carWidth, carHeight);
        }

        function drawObstacle(x, y) {
            context.fillStyle = 'red';
            context.fillRect(x, y, obstacleWidth, obstacleHeight);
        }

        function updateObstacles() {
            for (let i = 0; i < obstacles.length; i++) {
                obstacles[i].y += obstacleSpeed;
                if (obstacles[i].y > roadHeight) {
                    obstacles.splice(i, 1);
                    i--;
                }
            }
        }

        function checkCollision() {
            for (let obstacle of obstacles) {
                if (carX < obstacle.x + obstacleWidth &&
                    carX + carWidth > obstacle.x &&
                    carY < obstacle.y + obstacleHeight &&
                    carY + carHeight > obstacle.y) {
                    alert('Game Over');
                    document.location.reload();
                }
            }
        }

        function gameLoop() {
            context.clearRect(0, 0, roadWidth, roadHeight);

            if (Math.random() < 0.02) {
                let obstacleX = Math.random() * (roadWidth - obstacleWidth);
                obstacles.push({ x: obstacleX, y: -obstacleHeight });
            }

            drawCar();
            for (let obstacle of obstacles) {
                drawObstacle(obstacle.x, obstacle.y);
            }

            updateObstacles();
            checkCollision();

            requestAnimationFrame(gameLoop);
        }

        gameLoop();
    </script>
</body>
</html>-
fallousarr000/fallousarr000 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
