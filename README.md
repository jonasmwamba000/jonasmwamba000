# 👋 Hi, I'm Jonas Mwamba

Welcome to my GitHub profile!

## 🚀 About Me
I'm a passionate developer and technology enthusiast, always learning and building cool stuff.  
I love programming, solving problems, and collaborating with others.[index.html](https://github.com/user-attachments/files/22445014/index.html)<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub CV Background</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            background-size: 400% 400%;
            animation: smartGradient 8s ease-in-out infinite;
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }

        /* Smart animated background overlay */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 80%, rgba(120, 119, 198, 0.3) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 119, 198, 0.3) 0%, transparent 50%),
                radial-gradient(circle at 40% 40%, rgba(120, 219, 226, 0.3) 0%, transparent 50%);
            animation: smartOverlay 12s ease-in-out infinite;
            pointer-events: none;
            z-index: 1;
        }

        /* Smart gradient animation */
        @keyframes smartGradient {
            0% {
                background-position: 0% 50%;
                background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            }
            25% {
                background-position: 100% 50%;
                background: linear-gradient(135deg, #4facfe 0%, #00f2fe 50%, #43e97b 100%);
            }
            50% {
                background-position: 100% 100%;
                background: linear-gradient(135deg, #fa709a 0%, #fee140 50%, #667eea 100%);
            }
            75% {
                background-position: 50% 100%;
                background: linear-gradient(135deg, #a8edea 0%, #fed6e3 50%, #ff9a9e 100%);
            }
            100% {
                background-position: 0% 50%;
                background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            }
        }

        /* Smart overlay animation */
        @keyframes smartOverlay {
            0%, 100% {
                opacity: 0.6;
                transform: scale(1) rotate(0deg);
            }
            33% {
                opacity: 0.8;
                transform: scale(1.1) rotate(120deg);
            }
            66% {
                opacity: 0.4;
                transform: scale(0.9) rotate(240deg);
            }
        }

        .container {
            position: relative;
            z-index: 10;
            padding: 50px 20px;
            text-align: center;
            color: white;
        }

        /* Smart floating orbs */
        .smart-orb {
            position: absolute;
            border-radius: 50%;
            background: linear-gradient(45deg, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0.05));
            backdrop-filter: blur(10px);
            animation: orbFloat 20s linear infinite;
            pointer-events: none;
            z-index: 2;
        }

        .smart-orb:nth-child(1) { 
            width: 100px; height: 100px; 
            background: radial-gradient(circle, rgba(255, 107, 107, 0.4), rgba(255, 107, 107, 0.1));
            animation-duration: 25s;
        }
        .smart-orb:nth-child(2) { 
            width: 150px; height: 150px; 
            background: radial-gradient(circle, rgba(78, 205, 196, 0.4), rgba(78, 205, 196, 0.1));
            animation-duration: 30s;
            animation-delay: -5s;
        }
        .smart-orb:nth-child(3) { 
            width: 80px; height: 80px; 
            background: radial-gradient(circle, rgba(69, 183, 209, 0.4), rgba(69, 183, 209, 0.1));
            animation-duration: 22s;
            animation-delay: -10s;
        }
        .smart-orb:nth-child(4) { 
            width: 120px; height: 120px; 
            background: radial-gradient(circle, rgba(150, 206, 180, 0.4), rgba(150, 206, 180, 0.1));
            animation-duration: 28s;
            animation-delay: -15s;
        }

        @keyframes orbFloat {
            0% {
                transform: translate(0px, 100vh) scale(0);
                opacity: 0;
            }
            10% {
                opacity: 1;
                transform: translate(20px, 90vh) scale(1);
            }
            25% {
                transform: translate(-30px, 70vh) scale(1.2);
            }
            50% {
                transform: translate(40px, 40vh) scale(0.8);
            }
            75% {
                transform: translate(-20px, 20vh) scale(1.1);
            }
            90% {
                opacity: 1;
                transform: translate(10px, 5vh) scale(0.9);
            }
            100% {
                transform: translate(0px, -10vh) scale(0);
                opacity: 0;
            }
        }

        .header {
            margin-bottom: 30px;
            animation: fadeInUp 1s ease-out;
        }

        .header h1 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 10px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 4s ease-in-out infinite;
        }

        .subtitle {
            font-size: 1.5rem;
            color: #e0e6ed;
            margin-bottom: 40px;
            animation: fadeInUp 1s ease-out 0.3s both;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: 0 auto;
            animation: fadeInUp 1s ease-out 0.6s both;
        }

        .skill-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .skill-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
        }

        .skill-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s ease;
        }

        .skill-card:hover::before {
            left: 100%;
        }

        .skill-icon {
            font-size: 3rem;
            margin-bottom: 15px;
            display: block;
        }

        .skill-title {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 10px;
            color: #ffffff;
        }

        .skill-description {
            color: #e0e6ed;
            line-height: 1.5;
        }

        /* Flying Elements Animation */
        .flying-element {
            position: absolute;
            pointer-events: none;
            opacity: 0.6;
            animation: float 20s linear infinite;
        }

        .flying-element:nth-child(odd) {
            animation-duration: 25s;
        }

        .flying-element:nth-child(even) {
            animation-duration: 30s;
        }

        /* Flying Programming Symbols */
        .flying-symbol {
            position: absolute;
            pointer-events: none;
            opacity: 0.8;
            animation: symbolFloat 20s linear infinite;
            font-family: 'Courier New', monospace;
            font-weight: bold;
            text-shadow: 0 0 10px currentColor;
            z-index: 5;
        }

        .flying-symbol:nth-child(odd) {
            animation: symbolFloat 24s linear infinite;
        }

        .flying-symbol:nth-child(even) {
            animation: symbolBounce 26s linear infinite;
        }

        .flying-symbol:nth-child(3n) {
            animation: symbolFloat 22s linear infinite;
        }

        .flying-symbol:nth-child(4n) {
            animation: symbolBounce 28s linear infinite;
        }

        .flying-symbol:nth-child(5n) {
            animation: symbolFloat 25s linear infinite;
        }

        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.6;
            }
            90% {
                opacity: 0.6;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }

        @keyframes symbolFloat {
            0% {
                transform: translateY(-10vh) translateX(0px) rotate(0deg) scale(0.5);
                opacity: 0;
            }
            10% {
                opacity: 0.8;
                transform: translateY(10vh) translateX(15px) rotate(45deg) scale(1);
            }
            25% {
                transform: translateY(40vh) translateX(-25px) rotate(90deg) scale(1.1);
            }
            50% {
                transform: translateY(80vh) translateX(20px) rotate(180deg) scale(0.9);
            }
            65% {
                transform: translateY(95vh) translateX(-10px) rotate(225deg) scale(1.2);
            }
            75% {
                transform: translateY(85vh) translateX(30px) rotate(270deg) scale(1);
            }
            85% {
                transform: translateY(60vh) translateX(-20px) rotate(315deg) scale(1.1);
            }
            95% {
                opacity: 0.8;
                transform: translateY(20vh) translateX(10px) rotate(360deg) scale(0.8);
            }
            100% {
                transform: translateY(-5vh) translateX(0px) rotate(405deg) scale(0.3);
                opacity: 0;
            }
        }

        /* Alternative up-down animation for variety */
        @keyframes symbolBounce {
            0% {
                transform: translateY(110vh) translateX(0px) rotate(0deg) scale(0.8);
                opacity: 0;
            }
            15% {
                opacity: 0.9;
                transform: translateY(80vh) translateX(-20px) rotate(60deg) scale(1.2);
            }
            30% {
                transform: translateY(30vh) translateX(25px) rotate(120deg) scale(0.9);
            }
            45% {
                transform: translateY(60vh) translateX(-15px) rotate(180deg) scale(1.3);
            }
            60% {
                transform: translateY(15vh) translateX(30px) rotate(240deg) scale(1);
            }
            75% {
                transform: translateY(45vh) translateX(-25px) rotate(300deg) scale(1.1);
            }
            90% {
                opacity: 0.9;
                transform: translateY(5vh) translateX(20px) rotate(360deg) scale(0.7);
            }
            100% {
                transform: translateY(-15vh) translateX(0px) rotate(420deg) scale(0.4);
                opacity: 0;
            }
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
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

        /* Floating particles background */
        .particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 1;
        }

        .particle {
            position: absolute;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 50%;
            animation: particleFloat 15s linear infinite;
        }

        /* Rain Effect */
        .rain-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 3;
            overflow: hidden;
        }

        .rain-drop {
            position: absolute;
            background: linear-gradient(to bottom, rgba(255, 255, 255, 0.6), rgba(174, 194, 224, 0.3));
            width: 2px;
            height: 15px;
            border-radius: 0px 0px 2px 2px;
            animation: rainFall linear infinite;
            opacity: 0.7;
        }

        .rain-drop:nth-child(odd) {
            background: linear-gradient(to bottom, rgba(135, 206, 235, 0.5), rgba(100, 149, 237, 0.2));
            animation-duration: 1s;
        }

        .rain-drop:nth-child(even) {
            background: linear-gradient(to bottom, rgba(173, 216, 230, 0.6), rgba(176, 196, 222, 0.3));
            animation-duration: 1.2s;
        }

        .rain-drop:nth-child(3n) {
            background: linear-gradient(to bottom, rgba(240, 248, 255, 0.5), rgba(230, 230, 250, 0.2));
            animation-duration: 0.8s;
            width: 1px;
            height: 20px;
        }

        .rain-drop:nth-child(4n) {
            background: linear-gradient(to bottom, rgba(176, 224, 230, 0.6), rgba(175, 238, 238, 0.3));
            animation-duration: 1.4s;
            width: 3px;
            height: 12px;
        }

        .rain-drop:nth-child(5n) {
            background: linear-gradient(to bottom, rgba(255, 255, 255, 0.7), rgba(245, 245, 245, 0.4));
            animation-duration: 0.9s;
            width: 1.5px;
            height: 18px;
        }

        @keyframes rainFall {
            0% {
                transform: translateY(-100px);
                opacity: 0;
            }
            5% {
                opacity: 0.7;
            }
            95% {
                opacity: 0.7;
            }
            100% {
                transform: translateY(100vh);
                opacity: 0;
            }
        }

        /* Heavy rain drops */
        .rain-drop.heavy {
            width: 3px;
            height: 25px;
            background: linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(173, 216, 230, 0.5));
            animation-duration: 0.6s;
        }

        /* Light rain drops */
        .rain-drop.light {
            width: 1px;
            height: 10px;
            background: linear-gradient(to bottom, rgba(255, 255, 255, 0.4), rgba(240, 248, 255, 0.2));
            animation-duration: 1.6s;
        }

        @keyframes particleFloat {
            0% {
                transform: translateY(100vh) translateX(0px);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) translateX(100px);
                opacity: 0;
            }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2.5rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .skills-grid {
                grid-template-columns: 1fr;
                gap: 15px;
            }
            
            .container {
                padding: 30px 15px;
            }
        }

        /* GitHub Stats Section */
        .github-stats {
            margin-top: 50px;
            animation: fadeInUp 1s ease-out 0.9s both;
        }

        .stats-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 10px;
            padding: 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            min-width: 200px;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #4ecdc4;
        }

        .stat-label {
            color: #e0e6ed;
            margin-top: 5px;
        }

        /* Subscribe Button Styles */
        .subscribe-container {
            margin-top: 30px;
            display: flex;
            justify-content: center;
        }

        .subscribe-btn {
            position: relative;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            border: none;
            border-radius: 50px;
            padding: 15px 40px;
            font-size: 1.2rem;
            font-weight: bold;
            color: white;
            cursor: pointer;
            overflow: hidden;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            min-width: 180px;
            height: 60px;
        }

        .subscribe-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            background: linear-gradient(45deg, #ff5252, #26c6da);
        }

        .subscribe-btn:active {
            transform: translateY(0px);
        }

        .btn-text {
            display: inline-block;
            transition: all 0.3s ease;
        }

        .loading-spinner {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 24px;
            height: 24px;
            border: 3px solid rgba(255, 255, 255, 0.3);
            border-top: 3px solid white;
            border-radius: 50%;
            animation: spin 1s linear infinite;
            opacity: 0;
            visibility: hidden;
        }

        .success-icon {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 1.5rem;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }

        /* Button States */
        .subscribe-btn.loading .btn-text {
            opacity: 0;
            visibility: hidden;
        }

        .subscribe-btn.loading .loading-spinner {
            opacity: 1;
            visibility: visible;
        }

        .subscribe-btn.success {
            background: linear-gradient(45deg, #00b894, #00cec9);
        }

        .subscribe-btn.success .btn-text,
        .subscribe-btn.success .loading-spinner {
            opacity: 0;
            visibility: hidden;
        }

        .subscribe-btn.success .success-icon {
            opacity: 1;
            visibility: visible;
            animation: successPop 0.6s ease-out;
        }

        @keyframes spin {
            0% { transform: translate(-50%, -50%) rotate(0deg); }
            100% { transform: translate(-50%, -50%) rotate(360deg); }
        }

        @keyframes successPop {
            0% { 
                transform: translate(-50%, -50%) scale(0);
                opacity: 0;
            }
            50% { 
                transform: translate(-50%, -50%) scale(1.3);
                opacity: 1;
            }
            100% { 
                transform: translate(-50%, -50%) scale(1);
                opacity: 1;
            }
        }

        /* Button Glow Effect */
        .subscribe-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
            transition: left 0.5s ease;
        }

        .subscribe-btn:hover::before {
            left: 100%;
        }
    </style>
</head>
<body>
    <!-- Floating Particles Background -->
    <div class="particles" id="particles"></div>

    <!-- Rain Effect -->
    <div class="rain-container" id="rainContainer"></div>

    <!-- Smart Floating Orbs -->
    <div class="smart-orb" style="left: 10%;"></div>
    <div class="smart-orb" style="left: 70%;"></div>
    <div class="smart-orb" style="left: 30%;"></div>
    <div class="smart-orb" style="left: 80%;"></div>
    <div class="smart-orb" style="left: 50%;"></div>
    <div class="smart-orb" style="left: 20%;"></div>

    <!-- Flying Elements -->
    <div class="flying-element" style="left: 10%; font-size: 2rem;">💻</div>
    <div class="flying-element" style="left: 20%; font-size: 1.5rem;">🚀</div>
    <div class="flying-element" style="left: 30%; font-size: 2.5rem;">⭐</div>
    <div class="flying-element" style="left: 40%; font-size: 1.8rem;">🎯</div>
    <div class="flying-element" style="left: 50%; font-size: 2.2rem;">🔥</div>
    <div class="flying-element" style="left: 60%; font-size: 1.6rem;">💡</div>
    <div class="flying-element" style="left: 70%; font-size: 2rem;">🎨</div>
    <div class="flying-element" style="left: 80%; font-size: 1.7rem;">⚡</div>
    <div class="flying-element" style="left: 90%; font-size: 2.3rem;">🌟</div>

    <!-- Flying Programming Symbols -->
    <div class="flying-symbol" style="left: 5%; font-size: 3rem; color: #ff6b6b;">%</div>
    <div class="flying-symbol" style="left: 15%; font-size: 2.5rem; color: #4ecdc4;">}</div>
    <div class="flying-symbol" style="left: 25%; font-size: 2.8rem; color: #45b7d1;">]</div>
    <div class="flying-symbol" style="left: 35%; font-size: 2.2rem; color: #96ceb4;">+</div>
    <div class="flying-symbol" style="left: 45%; font-size: 2.6rem; color: #ffeaa7;">=</div>
    <div class="flying-symbol" style="left: 55%; font-size: 2.4rem; color: #fd79a8;">)</div>
    <div class="flying-symbol" style="left: 65%; font-size: 2.7rem; color: #fdcb6e;">*</div>
    <div class="flying-symbol" style="left: 75%; font-size: 2.3rem; color: #6c5ce7;">$</div>
    <div class="flying-symbol" style="left: 85%; font-size: 2.5rem; color: #a29bfe;">@</div>
    <div class="flying-symbol" style="left: 95%; font-size: 2.1rem; color: #fd79a8;">jonas</div>

    <!-- Additional Symbol Layer -->
    <div class="flying-symbol" style="left: 3%; font-size: 1.8rem; color: #00cec9; animation-delay: 3s;">}</div>
    <div class="flying-symbol" style="left: 13%; font-size: 2rem; color: #e17055; animation-delay: 1.5s;">%</div>
    <div class="flying-symbol" style="left: 23%; font-size: 2.4rem; color: #81ecec; animation-delay: 4s;">+</div>
    <div class="flying-symbol" style="left: 33%; font-size: 2.1rem; color: #fab1a0; animation-delay: 2s;">*</div>
    <div class="flying-symbol" style="left: 43%; font-size: 1.9rem; color: #ff7675; animation-delay: 5s;">]</div>
    <div class="flying-symbol" style="left: 53%; font-size: 2.3rem; color: #74b9ff; animation-delay: 0.5s;">$</div>
    <div class="flying-symbol" style="left: 63%; font-size: 2rem; color: #55a3ff; animation-delay: 2.8s;">@</div>
    <div class="flying-symbol" style="left: 73%; font-size: 2.5rem; color: #00b894; animation-delay: 1.2s;">)</div>
    <div class="flying-symbol" style="left: 83%; font-size: 1.7rem; color: #e84393; animation-delay: 3.5s;">=</div>
    <div class="flying-symbol" style="left: 93%; font-size: 2.2rem; color: #00cec9; animation-delay: 4.5s;">jonas</div>

    <!-- Extra Dense Layer for More Effect -->
    <div class="flying-symbol" style="left: 8%; font-size: 1.5rem; color: #dda0dd; animation-delay: 6s;">%</div>
    <div class="flying-symbol" style="left: 18%; font-size: 1.8rem; color: #98fb98; animation-delay: 7s;">}</div>
    <div class="flying-symbol" style="left: 28%; font-size: 1.6rem; color: #f0e68c; animation-delay: 8s;">+</div>
    <div class="flying-symbol" style="left: 38%; font-size: 1.9rem; color: #ffa07a; animation-delay: 9s;">*</div>
    <div class="flying-symbol" style="left: 48%; font-size: 1.7rem; color: #20b2aa; animation-delay: 10s;">]</div>
    <div class="flying-symbol" style="left: 58%; font-size: 2.1rem; color: #87ceeb; animation-delay: 11s;">$</div>
    <div class="flying-symbol" style="left: 68%; font-size: 1.4rem; color: #daa520; animation-delay: 12s;">@</div>
    <div class="flying-symbol" style="left: 78%; font-size: 1.6rem; color: #cd5c5c; animation-delay: 13s;">)</div>
    <div class="flying-symbol" style="left: 88%; font-size: 1.8rem; color: #4682b4; animation-delay: 14s;">=</div>
    <div class="flying-symbol" style="left: 98%; font-size: 1.5rem; color: #32cd32; animation-delay: 15s;">jonas</div>

    <div class="container">
        <div class="header">
            <h1>Artificial Technology Development</h1>
            <p class="subtitle">Passionate Developer | Problem Solver | Tech Enthusiast</p>
            
            <!-- Subscribe Button -->
            <div class="subscribe-container">
                <button class="subscribe-btn" id="subscribeBtn">
                    <span class="btn-text">Subscribe</span>
                    <span class="loading-spinner"></span>
                    <span class="success-icon">✓</span>
                </button>
            </div>
        </div>

        <div class="skills-grid">
            <div class="skill-card">
                <div class="skill-icon">🖥️</div>
                <h3 class="skill-title">Programming Languages</h3>
                <p class="skill-description">Python, JavaScript, Java, C++, HTML/CSS, SQL</p>
            </div>

            <div class="skill-card">
                <div class="skill-icon">🌐</div>
                <h3 class="skill-title">Web Development</h3>
                <p class="skill-description">React, Node.js, Express, MongoDB, RESTful APIs</p>
            </div>

            <div class="skill-card">
                <div class="skill-icon">📱</div>
                <h3 class="skill-title">Mobile Development</h3>
                <p class="skill-description">React Native, Flutter, Android Studio</p>
            </div>

            <div class="skill-card">
                <div class="skill-icon">🤖</div>
                <h3 class="skill-title">Data Science & AI</h3>
                <p class="skill-description">Machine Learning, TensorFlow, pandas, NumPy</p>
            </div>

            <div class="skill-card">
                <div class="skill-icon">☁️</div>
                <h3 class="skill-title">Cloud & DevOps</h3>
                <p class="skill-description">AWS, Docker, Git, CI/CD, Linux</p>
            </div>

            <div class="skill-card">
                <div class="skill-icon">🗄️</div>
                <h3 class="skill-title">Databases</h3>
                <p class="skill-description">MySQL, PostgreSQL, MongoDB, Firebase</p>
            </div>
        </div>

        <div class="github-stats">
            <h2 style="margin-bottom: 20px; color: #ffffff;">GitHub Statistics</h2>
            <div class="stats-container">
                <div class="stat-card">
                    <div class="stat-number">50+</div>
                    <div class="stat-label">Projects Completed</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">1000+</div>
                    <div class="stat-label">Commits This Year</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">15+</div>
                    <div class="stat-label">Technologies Mastered</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">3.9</div>
                    <div class="stat-label">GPA</div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Create floating particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;

            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                
                // Random size
                const size = Math.random() * 4 + 2;
                particle.style.width = size + 'px';
                particle.style.height = size + 'px';
                
                // Random position
                particle.style.left = Math.random() * 100 + '%';
                
                // Random animation delay
                particle.style.animationDelay = Math.random() * 15 + 's';
                
                // Random animation duration
                particle.style.animationDuration = (Math.random() * 10 + 15) + 's';
                
                particlesContainer.appendChild(particle);
            }
        }

        // Add random delays to flying elements and symbols
        function animateFlyingElements() {
            const flyingElements = document.querySelectorAll('.flying-element');
            const flyingSymbols = document.querySelectorAll('.flying-symbol');
            
            flyingElements.forEach((element, index) => {
                element.style.animationDelay = (Math.random() * 10) + 's';
                
                // Add random horizontal movement
                const randomX = Math.random() * 100 - 50;
                element.style.setProperty('--random-x', randomX + 'px');
            });

            flyingSymbols.forEach((symbol, index) => {
                symbol.style.animationDelay = (Math.random() * 15) + 's';
                
                // Add random properties for more variety
                const randomScale = 0.8 + Math.random() * 0.4;
                symbol.style.transform = `scale(${randomScale})`;
                
                // Random glow effect
                const glowIntensity = Math.random() * 15 + 5;
                symbol.style.textShadow = `0 0 ${glowIntensity}px currentColor`;
            });
        }

        // Add subscribe button functionality
        function addSubscribeButton() {
            const subscribeBtn = document.getElementById('subscribeBtn');
            
            subscribeBtn.addEventListener('click', function() {
                // Prevent multiple clicks
                if (subscribeBtn.classList.contains('loading') || subscribeBtn.classList.contains('success')) {
                    return;
                }

                // Add loading state
                subscribeBtn.classList.add('loading');
                subscribeBtn.style.pointerEvents = 'none';

                // Simulate loading time (2 seconds)
                setTimeout(() => {
                    subscribeBtn.classList.remove('loading');
                    subscribeBtn.classList.add('success');
                    
                    // Show success state for 2 seconds, then reset
                    setTimeout(() => {
                        subscribeBtn.classList.remove('success');
                        subscribeBtn.style.pointerEvents = 'auto';
                    }, 2000);
                }, 2000);
            });
        }

        // Add subscribe button functionality
        function addSubscribeButton() {
            const subscribeBtn = document.getElementById('subscribeBtn');
            
            subscribeBtn.addEventListener('click', function() {
                // Prevent multiple clicks
                if (subscribeBtn.classList.contains('loading') || subscribeBtn.classList.contains('success')) {
                    return;
                }

                // Add loading state
                subscribeBtn.classList.add('loading');
                subscribeBtn.style.pointerEvents = 'none';

                // Simulate loading time (2 seconds)
                setTimeout(() => {
                    subscribeBtn.classList.remove('loading');
                    subscribeBtn.classList.add('success');
                    
                    // Show success state for 2 seconds, then reset
                    setTimeout(() => {
                        subscribeBtn.classList.remove('success');
                        subscribeBtn.style.pointerEvents = 'auto';
                    }, 2000);
                }, 2000);
            });
        }
            const skillCards = document.querySelectorAll('.skill-card');
            
            skillCards.forEach(card => {
                card.addEventListener('mousemove', (e) => {
                    const rect = card.getBoundingClientRect();
                    const x = e.clientX - rect.left;
                    const y = e.clientY - rect.top;
                    
                    const centerX = rect.width / 2;
                    const centerY = rect.height / 2;
                    
                    const rotateX = (y - centerY) / 10;
                    const rotateY = (centerX - x) / 10;
                    
                    card.style.transform = `perspective(1000px) rotateX(${rotateX}deg) rotateY(${rotateY}deg) translateY(-10px)`;
                });
                
                card.addEventListener('mouseleave', () => {
                    card.style.transform = 'perspective(1000px) rotateX(0deg) rotateY(0deg) translateY(0px)';
                });
            });
        }

        // Initialize animations
        document.addEventListener('DOMContentLoaded', () => {
            createParticles();
            animateFlyingElements();
            addInteractiveEffects();
            addSubscribeButton();
            addDynamicColors();
            createSmartOrbs();
            createRain();
        });

        // Add dynamic color changing with more variety
        function addDynamicColors() {
            const colorSets = [
                ['#667eea', '#764ba2', '#f093fb'],
                ['#4facfe', '#00f2fe', '#43e97b'],
                ['#fa709a', '#fee140', '#667eea'],
                ['#a8edea', '#fed6e3', '#ff9a9e'],
                ['#ffecd2', '#fcb69f', '#ff8a80'],
                ['#89f7fe', '#66a6ff', '#667eea']
            ];
            
            let currentSet = 0;
            
            setInterval(() => {
                currentSet = (currentSet + 1) % colorSets.length;
                const colors = colorSets[currentSet];
                document.body.style.background = `linear-gradient(135deg, ${colors[0]} 0%, ${colors[1]} 50%, ${colors[2]} 100%)`;
            }, 8000);
        }

        // Create realistic rain effect
        function createRain() {
            const rainContainer = document.getElementById('rainContainer');
            const rainDropCount = 150; // Number of rain drops
            
            for (let i = 0; i < rainDropCount; i++) {
                const rainDrop = document.createElement('div');
                rainDrop.className = 'rain-drop';
                
                // Random positioning across the width
                rainDrop.style.left = Math.random() * 100 + '%';
                
                // Random animation delay for natural effect
                rainDrop.style.animationDelay = Math.random() * 2 + 's';
                
                // Random duration for variety
                const duration = Math.random() * 0.8 + 0.6; // 0.6s to 1.4s
                rainDrop.style.animationDuration = duration + 's';
                
                // Add variety classes randomly
                const randomClass = Math.random();
                if (randomClass < 0.1) {
                    rainDrop.classList.add('heavy');
                } else if (randomClass < 0.3) {
                    rainDrop.classList.add('light');
                }
                
                rainContainer.appendChild(rainDrop);
            }
            
            // Create continuous rain by adding new drops
            setInterval(() => {
                if (rainContainer.children.length < rainDropCount * 1.5) {
                    for (let i = 0; i < 20; i++) {
                        const newDrop = document.createElement('div');
                        newDrop.className = 'rain-drop';
                        newDrop.style.left = Math.random() * 100 + '%';
                        newDrop.style.animationDelay = '0s';
                        newDrop.style.animationDuration = (Math.random() * 0.8 + 0.6) + 's';
                        
                        const randomClass = Math.random();
                        if (randomClass < 0.1) {
                            newDrop.classList.add('heavy');
                        } else if (randomClass < 0.3) {
                            newDrop.classList.add('light');
                        }
                        
                        rainContainer.appendChild(newDrop);
                        
                        // Remove drop after animation
                        setTimeout(() => {
                            if (newDrop.parentNode) {
                                newDrop.parentNode.removeChild(newDrop);
                            }
                        }, 2000);
                    }
                }
            }, 200); // Add new drops every 200ms
        }
            const colors = [
                'rgba(255, 107, 107, 0.3)',
                'rgba(78, 205, 196, 0.3)', 
                'rgba(69, 183, 209, 0.3)',
                'rgba(150, 206, 180, 0.3)',
                'rgba(255, 195, 113, 0.3)',
                'rgba(196, 113, 237, 0.3)'
            ];
            
            for (let i = 0; i < 8; i++) {
                const orb = document.createElement('div');
                orb.className = 'smart-orb';
                orb.style.left = Math.random() * 100 + '%';
                orb.style.width = (Math.random() * 100 + 50) + 'px';
                orb.style.height = orb.style.width;
                orb.style.background = `radial-gradient(circle, ${colors[Math.floor(Math.random() * colors.length)]}, transparent)`;
                orb.style.animationDelay = (Math.random() * 20) + 's';
                orb.style.animationDuration = (Math.random() * 10 + 20) + 's';
                document.body.appendChild(orb);
            }
        }
    </script>
</body>
</html>


## 🛠️ Skills
- HTML, CSS, JavaScript
- Python, C++
- Git & GitHub
- Visual Studio & VS Code

## 📂 Projects
Here are some of my top repositories:
- [My-First-work-](https://github.com/jonasmwamba000/My-First-work-)
- [Jonas-](https://github.com/jonasmwamba000/Jonas-)
- [ATD](https://github.com/jonasmwamba000/ATD)

## 🌐 Connect with Me
- [Email](mailto:youremail@example.com)
- [LinkedIn](https://www.linkedin.com)

---

> “Code is like humor. When you have to explain it, it’s bad.” – Cory House
