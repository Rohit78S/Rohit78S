<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rohit - Deep Learning Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f5f5f5;
        }

        .header-container {
            position: relative;
            width: 100%;
            height: 400px;
            background: url('https://i.pinimg.com/originals/3e/1a/8d/3e1a8de85eda4b7f38bee4b4b4da4c0b.gif') center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .header-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.4);
            z-index: 1;
        }

        .text-container {
            position: relative;
            z-index: 2;
            text-align: center;
            height: 150px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .animated-text {
            font-size: 60px;
            font-weight: bold;
            color: white;
            text-shadow: 3px 3px 15px rgba(0, 0, 0, 0.7);
            min-height: 80px;
            letter-spacing: 2px;
        }

        .word {
            display: inline-block;
            opacity: 0;
            animation: fadeInUp 0.6s ease-out forwards;
            margin: 0 10px;
        }

        .word:nth-child(1) {
            animation-delay: 0.2s;
        }

        .word:nth-child(2) {
            animation-delay: 0.8s;
        }

        .word:nth-child(3) {
            animation-delay: 1.4s;
        }

        .word:nth-child(4) {
            animation-delay: 2.0s;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .wave {
            animation: wave 0.6s ease-in-out;
            display: inline-block;
            transform-origin: bottom;
        }

        @keyframes wave {
            0%, 100% {
                transform: rotate(0deg);
            }
            25% {
                transform: rotate(20deg);
            }
            50% {
                transform: rotate(-20deg);
            }
            75% {
                transform: rotate(10deg);
            }
        }

        .content {
            max-width: 900px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .section-title {
            font-size: 24px;
            font-weight: bold;
            color: #333;
            margin-top: 30px;
            margin-bottom: 15px;
            border-bottom: 3px solid #0099ff;
            padding-bottom: 10px;
            display: inline-block;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-link {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            background: #0099ff;
            border-radius: 50%;
            text-decoration: none;
            color: white;
            font-size: 24px;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            transform: scale(1.1);
            background: #0077cc;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .skill-badge {
            background: #f0f0f0;
            border: 2px solid #0099ff;
            border-radius: 8px;
            padding: 12px;
            text-align: center;
            font-weight: 600;
            color: #0099ff;
            transition: all 0.3s ease;
        }

        .skill-badge:hover {
            background: #0099ff;
            color: white;
            transform: translateY(-3px);
        }

        .info-text {
            color: #666;
            line-height: 1.8;
            margin-top: 20px;
            font-size: 16px;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 30px;
            background: #f9f9f9;
            padding: 20px;
            border-radius: 8px;
        }

        .stat-item {
            text-align: center;
        }

        .stat-number {
            font-size: 32px;
            font-weight: bold;
            color: #0099ff;
        }

        .stat-label {
            color: #666;
            margin-top: 5px;
        }

        @media (max-width: 768px) {
            .header-container {
                height: 300px;
            }

            .animated-text {
                font-size: 40px;
            }

            .stats {
                grid-template-columns: 1fr;
            }

            .word {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>
    <!-- Animated Header -->
    <div class="header-container">
        <div class="header-overlay"></div>
        <div class="text-container">
            <div class="animated-text">
                <span class="word">
                    <span class="wave">👋</span>
                </span>
                <span class="word">Hey</span>
                <span class="word">I'm</span>
                <span class="word">Rohit</span>
            </div>
        </div>
    </div>

    <!-- Main Content -->
    <div class="content">
        <h2 class="section-title">💻 Deep Learning / Neural Networks (Machine Learning)</h2>
        
        <div class="info-text">
            <p>Learning Deep Learning and Machine Learning using Python and NumPy. Passionate about building Neural Networks and exploring AI.</p>
        </div>

        <h2 class="section-title">🤝 Connect with me:</h2>
        <div class="social-links">
            <a href="https://instagram.com/rohit_samanta10" class="social-link" title="Instagram">📷</a>
            <a href="https://github.com/rohit78s" class="social-link" title="GitHub">🐙</a>
        </div>

        <h2 class="section-title">💻 Languages and Tools:</h2>
        <div class="skills-grid">
            <div class="skill-badge">🐍 Python</div>
            <div class="skill-badge">📊 NumPy</div>
            <div class="skill-badge">🌐 HTML</div>
            <div class="skill-badge">🎨 CSS</div>
            <div class="skill-badge">✨ JavaScript</div>
        </div>

        <h2 class="section-title">📈 My Stats:</h2>
        <div class="stats">
            <div class="stat-item">
                <div class="stat-number">9</div>
                <div class="stat-label">Repositories</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">33</div>
                <div class="stat-label">Commits</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">🚀</div>
                <div class="stat-label">Learning</div>
            </div>
        </div>

        <h2 class="section-title">📌 About Me:</h2>
        <div class="info-text">
            <p><strong>Currently working on:</strong></p>
            <p>🧠 Neural Network projects<br>
            📊 Data analysis with NumPy<br>
            🌐 Web development basics</p>
            <p style="margin-top: 20px;"><strong>Let's connect and learn together! 🚀</strong></p>
        </div>
    </div>
</body>
</html>
