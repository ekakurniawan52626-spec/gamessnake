<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snake Game</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            color: white;
            overflow: hidden;
        }
        
        .container {
            width: 100%;
            max-width: 600px;
            text-align: center;
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        .game-info {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            padding: 15px;
            background-color: rgba(0, 0, 0, 0.3);
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .score-container {
            font-size: 1.2rem;
            font-weight: bold;
        }
        
        button {
            background: linear-gradient(to right, #4facfe 0%, #00f2fe 100%);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 50px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }
        
        .game-container {
            position: relative;
            margin: 0 auto;
            width: 400px;
            height: 400px;
        }
        
        canvas {
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
        }
        
        .controls {
            margin-top: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .desktop-controls {
            margin-bottom: 20px;
        }
        
        .mobile-controls {
            display: none;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: repeat(3, 1fr);
            gap: 10px;
            width: 200px;
            height: 200px;
            margin-top: 20px;
        }
        
        .control-btn {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.2);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            user-select: none;
        }
        
        .up-btn {
            grid-column: 2;
            grid-row: 1;
        }
        
        .left-btn {
            grid-column: 1;
            grid-row: 2;
        }
        
        .right-btn {
            grid-column: 3;
            grid-row: 2;
        }
        
        .down-btn {
            grid-column: 2;
            grid-row: 3;
        }
        
        .game-over {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border-radius: 10px;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.5s ease;
        }
        
        .game-over.show {
            opacity: 1;
            pointer-events: all;
        }
        
        .game-over h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .game-over p {
            font-size: 1.5rem;
            margin-bottom: 30px;
        }
        
        @media (max-width: 500px) {
            .game-container {
                width: 320px;
                height: 320px;
            }
            
            h1 {
                font-size: 2.5rem;
            }
            
            .desktop-controls {
                display: none;
            }
            
            .mobile-controls {
                display: grid;
            }
        }
    </style>
</head>
<body>
    <a href="http://localhost/xpplgekabercode/new/uyuyu/cv/gamebot.php"><mark>HOME</mark></a>
    <div class="container">
        <h1>GAME ULAR MUDAH</h1>
        
        <div class="game-info">
            <div class="score-container">
                Score: <span id="score">0</span>
            </div>
            <button id="start-btn">MULAI!</button>
        </div>
        
        <div class="game-container">
            <canvas id="game-canvas" width="400" height="400"></canvas>
            
            <div class="game-over" id="game-over">
                <h2>Yah cupu!</h2>
                <p>Dikit Banget: <span id="final-score">0</span></p>
                <button id="restart-btn">Play Again</button>
            </div>
        </div>
        
        <div class="controls">
            <div class="desktop-controls">
                <p>gunain tanda panah di keyboard buat kendaliin ular!</p>
            </div>
            
            <div class="mobile-controls">
                <div class="control-btn up-btn" id="up-btn">↑</div>
                <div class="control-btn left-btn" id="left-btn">←</div>
                <div class="control-btn right-btn" id="right-btn">→</div>
                <div class="control-btn down-btn" id="down-btn">↓</div>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const canvas = document.getElementById('game-canvas');
            const ctx = canvas.getContext('2d');
            const scoreElement = document.getElementById('score');
            const finalScoreElement = document.getElementById('final-score');
            const startButton = document.getElementById('start-btn');
            const restartButton = document.getElementById('restart-btn');
            const gameOverScreen = document.getElementById('game-over');
            
            // Mobile control buttons
            const upButton = document.getElementById('up-btn');
            const leftButton = document.getElementById('left-btn');
            const rightButton = document.getElementById('right-btn');
            const downButton = document.getElementById('down-btn');
            
            // Game variables
            const gridSize = 20;
            const gridWidth = canvas.width / gridSize;
            const gridHeight = canvas.height / gridSize;
            
            let snake = [];
            let food = {};
            let direction = 'right';
            let nextDirection = 'right';
            let score = 0;
            let gameSpeed = 150;
            let gameRunning = false;
            let gameLoop;
            
            // Initialize game
            function initGame() {
                snake = [
                    {x: 5, y: 10},
                    {x: 4, y: 10},
                    {x: 3, y: 10}
                ];
                
                generateFood();
                score = 0;
                scoreElement.textContent = score;
                direction = 'right';
                nextDirection = 'right';
                gameSpeed = 150;
                gameOverScreen.classList.remove('show');
            }
            
            // Generate food at random position
            function generateFood() {
                food = {
                    x: Math.floor(Math.random() * gridWidth),
                    y: Math.floor(Math.random() * gridHeight)
                };
                
                // Make sure food doesn't spawn on snake
                for (let i = 0; i < snake.length; i++) {
                    if (snake[i].x === food.x && snake[i].y === food.y) {
                        return generateFood();
                    }
                }
            }
            
            // Draw game elements
            function draw() {
                // Clear canvas
                ctx.fillStyle = 'rgba(0, 0, 0, 0.7)';
                ctx.fillRect(0, 0, canvas.width, canvas.height);
                
                // Draw snake
                snake.forEach((segment, index) => {
                    if (index === 0) {
                        ctx.fillStyle = '#4facfe'; // Head color
                    } else {
                        ctx.fillStyle = '#00f2fe'; // Body color
                    }
                    ctx.fillRect(segment.x * gridSize, segment.y * gridSize, gridSize, gridSize);
                    
                    // Add eyes to the head
                    if (index === 0) {
                        ctx.fillStyle = 'white';
                        
                        // Position eyes based on direction
                        if (direction === 'right') {
                            ctx.fillRect(segment.x * gridSize + 14, segment.y * gridSize + 5, 4, 4);
                            ctx.fillRect(segment.x * gridSize + 14, segment.y * gridSize + 11, 4, 4);
                        } else if (direction === 'left') {
                            ctx.fillRect(segment.x * gridSize + 2, segment.y * gridSize + 5, 4, 4);
                            ctx.fillRect(segment.x * gridSize + 2, segment.y * gridSize + 11, 4, 4);
                        } else if (direction === 'up') {
                            ctx.fillRect(segment.x * gridSize + 5, segment.y * gridSize + 2, 4, 4);
                            ctx.fillRect(segment.x * gridSize + 11, segment.y * gridSize + 2, 4, 4);
                        } else if (direction === 'down') {
                            ctx.fillRect(segment.x * gridSize + 5, segment.y * gridSize + 14, 4, 4);
                            ctx.fillRect(segment.x * gridSize + 11, segment.y * gridSize + 14, 4, 4);
                        }
                    }
                });
                
                // Draw food
                ctx.fillStyle = '#ff5252';
                ctx.beginPath();
                ctx.arc(
                    food.x * gridSize + gridSize / 2,
                    food.y * gridSize + gridSize / 2,
                    gridSize / 2,
                    0,
                    Math.PI * 2
                );
                ctx.fill();
            }
            
            // Update game state
            function update() {
                // Update direction
                direction = nextDirection;
                
                // Calculate new head position
                const head = {...snake[0]};
                
                switch (direction) {
                    case 'right':
                        head.x++;
                        break;
                    case 'left':
                        head.x--;
                        break;
                    case 'up':
                        head.y--;
                        break;
                    case 'down':
                        head.y++;
                        break;
                }
                
                // Check for collision with walls
                if (head.x < 0 || head.x >= gridWidth || head.y < 0 || head.y >= gridHeight) {
                    gameOver();
                    return;
                }
                
                // Check for collision with self
                for (let i = 0; i < snake.length; i++) {
                    if (snake[i].x === head.x && snake[i].y === head.y) {
                        gameOver();
                        return;
                    }
                }
                
                // Add new head
                snake.unshift(head);
                
                // Check for food collision
                if (head.x === food.x && head.y === food.y) {
                    score += 10;
                    scoreElement.textContent = score;
                    
                    // Increase speed slightly with each food
                    if (gameSpeed > 50) {
                        gameSpeed -= 2;
                    }
                    
                    generateFood();
                } else {
                    // Remove tail if no food was eaten
                    snake.pop();
                }
            }
            
            // Game loop
            function gameStep() {
                update();
                draw();
                
                if (gameRunning) {
                    gameLoop = setTimeout(gameStep, gameSpeed);
                }
            }
            
            // Game over
            function gameOver() {
                gameRunning = false;
                clearTimeout(gameLoop);
                finalScoreElement.textContent = score;
                gameOverScreen.classList.add('show');
            }
            
            // Start game
            function startGame() {
                if (!gameRunning) {
                    initGame();
                    gameRunning = true;
                    gameStep();
                    startButton.textContent = "Pause Game";
                } else {
                    gameRunning = false;
                    clearTimeout(gameLoop);
                    startButton.textContent = "Resume Game";
                }
            }
            
            // Handle keyboard input
            function handleKeydown(e) {
                if (!gameRunning) return;
                
                switch (e.key) {
                    case 'ArrowUp':
                        if (direction !== 'down') nextDirection = 'up';
                        break;
                    case 'ArrowDown':
                        if (direction !== 'up') nextDirection = 'down';
                        break;
                    case 'ArrowLeft':
                        if (direction !== 'right') nextDirection = 'left';
                        break;
                    case 'ArrowRight':
                        if (direction !== 'left') nextDirection = 'right';
                        break;
                }
            }
            
            // Mobile controls
            upButton.addEventListener('click', () => {
                if (direction !== 'down') nextDirection = 'up';
            });
            
            downButton.addEventListener('click', () => {
                if (direction !== 'up') nextDirection = 'down';
            });
            
            leftButton.addEventListener('click', () => {
                if (direction !== 'right') nextDirection = 'left';
            });
            
            rightButton.addEventListener('click', () => {
                if (direction !== 'left') nextDirection = 'right';
            });
            
            // Touch controls for swipe
            let touchStartX = 0;
            let touchStartY = 0;
            
            canvas.addEventListener('touchstart', (e) => {
                touchStartX = e.touches[0].clientX;
                touchStartY = e.touches[0].clientY;
                e.preventDefault();
            });
            
            canvas.addEventListener('touchmove', (e) => {
                e.preventDefault();
            });
            
            canvas.addEventListener('touchend', (e) => {
                if (!gameRunning) return;
                
                const touchEndX = e.changedTouches[0].clientX;
                const touchEndY = e.changedTouches[0].clientY;
                
                const dx = touchEndX - touchStartX;
                const dy = touchEndY - touchStartY;
                
                // Minimum swipe distance
                if (Math.max(Math.abs(dx), Math.abs(dy)) < 20) return;
                
                if (Math.abs(dx) > Math.abs(dy)) {
                    // Horizontal swipe
                    if (dx > 0 && direction !== 'left') {
                        nextDirection = 'right';
                    } else if (dx < 0 && direction !== 'right') {
                        nextDirection = 'left';
                    }
                } else {
                    // Vertical swipe
                    if (dy > 0 && direction !== 'up') {
                        nextDirection = 'down';
                    } else if (dy < 0 && direction !== 'down') {
                        nextDirection = 'up';
                    }
                }
                
                e.preventDefault();
            });
            
            // Event listeners
            startButton.addEventListener('click', startGame);
            restartButton.addEventListener('click', startGame);
            document.addEventListener('keydown', handleKeydown);
            
            // Initial draw
            initGame();
            draw();
        });
    </script>
</body>
</html>
