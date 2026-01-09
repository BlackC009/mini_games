[Uploading index.html…]()
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>小游戏集合</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background: 
                radial-gradient(ellipse at 20% 20%, rgba(102, 126, 234, 0.15) 0%, transparent 50%),
                radial-gradient(ellipse at 80% 80%, rgba(118, 75, 162, 0.15) 0%, transparent 50%),
                linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
            color: #fff;
            padding: 20px;
        }

        h1 {
            font-size: clamp(1.5rem, 5vw, 2.5rem);
            font-weight: 300;
            letter-spacing: 4px;
            margin-bottom: 40px;
            text-align: center;
            background: linear-gradient(90deg, #fff, #a0a0ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .games-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
            gap: clamp(12px, 4vw, 24px);
            max-width: min(90vw, 500px);
            width: 100%;
        }

        .game-card {
            aspect-ratio: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background: rgba(255, 255, 255, 0.08);
            border-radius: clamp(12px, 3vw, 20px);
            cursor: pointer;
            transition: all 0.3s ease;
            border: 2px solid rgba(255, 255, 255, 0.1);
            text-decoration: none;
            color: #fff;
        }

        .game-card:hover {
            background: rgba(102, 126, 234, 0.25);
            border-color: #667eea;
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 40px rgba(102, 126, 234, 0.4);
        }

        .game-card .icon {
            font-size: clamp(2rem, 8vw, 3.5rem);
            margin-bottom: clamp(8px, 2vw, 12px);
        }

        .game-card .name {
            font-size: clamp(0.9rem, 3vw, 1.2rem);
            font-weight: 500;
            letter-spacing: 2px;
        }

        .footer {
            margin-top: 50px;
            font-size: 0.8rem;
            opacity: 0.5;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>小游戏集合</h1>

    <div class="games-grid">
        <a href="tictactoe.html" class="game-card">
            <span class="icon">❌⭕</span>
            <span class="name">井字棋-轮回</span>
        </a>
        
        <!-- 后续游戏添加位置 -->
    </div>

    <div class="footer">
        更多游戏陆续开发中...
    </div>
</body>
</html>
