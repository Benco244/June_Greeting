<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy New Month - June 2025</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow-x: hidden;
        }
        
        .greeting-container {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border-radius: 30px;
            padding: 60px 40px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            max-width: 800px;
            width: 90%;
            position: relative;
            overflow: hidden;
            animation: fadeInUp 1s ease-out, celebrationBounce 3s ease-in-out infinite;
        }
        
        @keyframes celebrationBounce {
            0%, 100% { transform: translateY(0px) scale(1); }
            50% { transform: translateY(-5px) scale(1.02); }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .sun-icon {
            width: 100px;
            height: 100px;
            margin: 0 auto 30px;
            position: relative;
            animation: rotate 20s linear infinite;
        }
        
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .sun-center {
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, #FFD700, #FFA500);
            border-radius: 50%;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.6);
        }
        
        .sun-ray {
            position: absolute;
            width: 4px;
            height: 20px;
            background: linear-gradient(135deg, #FFD700, #FFA500);
            border-radius: 2px;
            top: 10px;
            left: 50%;
            transform-origin: 50% 40px;
        }
        
        .sun-ray:nth-child(2) { transform: translateX(-50%) rotate(45deg); }
        .sun-ray:nth-child(3) { transform: translateX(-50%) rotate(90deg); }
        .sun-ray:nth-child(4) { transform: translateX(-50%) rotate(135deg); }
        .sun-ray:nth-child(5) { transform: translateX(-50%) rotate(180deg); }
        .sun-ray:nth-child(6) { transform: translateX(-50%) rotate(225deg); }
        .sun-ray:nth-child(7) { transform: translateX(-50%) rotate(270deg); }
        .sun-ray:nth-child(8) { transform: translateX(-50%) rotate(315deg); }
        
        .main-greeting {
            color: white;
            font-size: 3.2rem;
            font-weight: 700;
            margin-bottom: 20px;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3);
            animation: glow 2s ease-in-out infinite alternate, celebrationWobble 4s ease-in-out infinite;
        }
        
        @keyframes celebrationWobble {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(1deg); }
            75% { transform: rotate(-1deg); }
        }
        
        @keyframes glow {
            from { text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3), 0 0 20px rgba(255, 255, 255, 0.2); }
            to { text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3), 0 0 30px rgba(255, 255, 255, 0.4); }
        }
        
        .sub-greeting {
            color: rgba(255, 255, 255, 0.9);
            font-size: 1.4rem;
            font-weight: 400;
            margin-bottom: 40px;
            line-height: 1.6;
        }
        
        .highlight {
            color: #FFD700;
            font-weight: 600;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }
        
        .feature-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 25px 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
            animation: slideIn 1s ease-out;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.15);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        
        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        .feature-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
            display: block;
        }
        
        .feature-title {
            color: white;
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 8px;
        }
        
        .feature-desc {
            color: rgba(255, 255, 255, 0.8);
            font-size: 0.9rem;
            line-height: 1.4;
        }
        
        .brand-signature {
            margin-top: 50px;
            color: rgba(255, 255, 255, 0.7);
            font-size: 1.1rem;
            font-weight: 300;
        }
        
        .brand-name {
            color: #FFD700;
            font-weight: 600;
            font-size: 1.3rem;
        }
        
        .floating-particles {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
            overflow: hidden;
        }
        
        .particle {
            position: absolute;
            width: 6px;
            height: 6px;
            background: rgba(255, 215, 0, 0.6);
            border-radius: 50%;
            animation: float 8s infinite ease-in-out;
        }
        
        .particle:nth-child(1) { left: 10%; animation-delay: 0s; }
        .particle:nth-child(2) { left: 20%; animation-delay: 1s; }
        .particle:nth-child(3) { left: 80%; animation-delay: 2s; }
        .particle:nth-child(4) { left: 90%; animation-delay: 3s; }
        .particle:nth-child(5) { left: 50%; animation-delay: 4s; }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); opacity: 0.7; }
            50% { transform: translateY(-30px) rotate(180deg); opacity: 1; }
        }
        
        /* Balloon Effects */
        .balloons-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            overflow: hidden;
        }
        
        .balloon {
            position: absolute;
            width: 30px;
            height: 40px;
            border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
            animation: balloonFloat 6s infinite ease-in-out;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .balloon::after {
            content: '';
            position: absolute;
            width: 1px;
            height: 20px;
            background: rgba(255, 255, 255, 0.5);
            bottom: -20px;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .balloon-1 {
            background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
            top: 20%;
            left: 15%;
            animation-delay: 0s;
        }
        
        .balloon-2 {
            background: linear-gradient(135deg, #4ecdc4, #45b7b8);
            top: 30%;
            right: 12%;
            animation-delay: 1s;
        }
        
        .balloon-3 {
            background: linear-gradient(135deg, #ffe66d, #ffda4d);
            top: 15%;
            left: 50%;
            animation-delay: 2s;
        }
        
        .balloon-4 {
            background: linear-gradient(135deg, #ff9ff3, #f368e0);
            top: 25%;
            right: 30%;
            animation-delay: 3s;
        }
        
        .balloon-5 {
            background: linear-gradient(135deg, #54a0ff, #2e86de);
            top: 35%;
            left: 25%;
            animation-delay: 4s;
        }
        
        @keyframes balloonFloat {
            0%, 100% {
                transform: translateY(0px) rotate(-2deg);
            }
            50% {
                transform: translateY(-20px) rotate(2deg);
            }
        }
        
        /* Confetti Effects */
        .confetti-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            overflow: hidden;
        }
        
        .confetti {
            position: absolute;
            width: 8px;
            height: 8px;
            animation: confettiFall 3s infinite linear;
        }
        
        .confetti:nth-child(odd) {
            background: #ff6b6b;
            border-radius: 50%;
        }
        
        .confetti:nth-child(even) {
            background: #4ecdc4;
            transform: rotate(45deg);
        }
        
        .confetti:nth-child(3n) {
            background: #ffe66d;
            border-radius: 2px;
            width: 6px;
            height: 12px;
        }
        
        .confetti-1 { left: 10%; animation-delay: 0s; }
        .confetti-2 { left: 20%; animation-delay: 0.5s; }
        .confetti-3 { left: 30%; animation-delay: 1s; }
        .confetti-4 { left: 40%; animation-delay: 1.5s; }
        .confetti-5 { left: 50%; animation-delay: 2s; }
        .confetti-6 { left: 60%; animation-delay: 2.5s; }
        .confetti-7 { left: 70%; animation-delay: 3s; }
        .confetti-8 { left: 80%; animation-delay: 3.5s; }
        .confetti-9 { left: 90%; animation-delay: 4s; }
        
        @keyframes confettiFall {
            0% {
                transform: translateY(-100vh) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(100vh) rotate(720deg);
                opacity: 0;
            }
        }
        
        /* Celebration Burst Effect */
        .celebration-burst {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
            top: 0;
            left: 0;
        }
        
        .burst-particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: #FFD700;
            border-radius: 50%;
            top: 50%;
            left: 50%;
            animation: burstOut 2s infinite ease-out;
        }
        
        .burst-particle:nth-child(1) { animation-delay: 0s; transform: rotate(0deg); }
        .burst-particle:nth-child(2) { animation-delay: 0.1s; transform: rotate(45deg); }
        .burst-particle:nth-child(3) { animation-delay: 0.2s; transform: rotate(90deg); }
        .burst-particle:nth-child(4) { animation-delay: 0.3s; transform: rotate(135deg); }
        .burst-particle:nth-child(5) { animation-delay: 0.4s; transform: rotate(180deg); }
        .burst-particle:nth-child(6) { animation-delay: 0.5s; transform: rotate(225deg); }
        .burst-particle:nth-child(7) { animation-delay: 0.6s; transform: rotate(270deg); }
        .burst-particle:nth-child(8) { animation-delay: 0.7s; transform: rotate(315deg); }
        
        @keyframes burstOut {
            0% {
                transform: translateX(0) translateY(0) scale(0);
                opacity: 1;
            }
            50% {
                transform: translateX(60px) translateY(-60px) scale(1);
                opacity: 0.8;
            }
            100% {
                transform: translateX(120px) translateY(-120px) scale(0);
                opacity: 0;
            }
        }
        
        /* Sparkle Effects */
        .sparkles {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
            top: 0;
            left: 0;
        }
        
        .sparkle {
            position: absolute;
            width: 6px;
            height: 6px;
            background: white;
            clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
            animation: sparkleShine 2s infinite ease-in-out;
        }
        
        .sparkle:nth-child(1) { top: 20%; left: 20%; animation-delay: 0s; }
        .sparkle:nth-child(2) { top: 30%; right: 25%; animation-delay: 0.5s; }
        .sparkle:nth-child(3) { top: 60%; left: 15%; animation-delay: 1s; }
        .sparkle:nth-child(4) { top: 70%; right: 20%; animation-delay: 1.5s; }
        .sparkle:nth-child(5) { top: 40%; left: 80%; animation-delay: 2s; }
        
        @keyframes sparkleShine {
            0%, 100% {
                opacity: 0;
                transform: scale(0.5) rotate(0deg);
            }
            50% {
                opacity: 1;
                transform: scale(1.2) rotate(180deg);
            }
        }
        
        @media (max-width: 768px) {
            .greeting-container {
                padding: 40px 25px;
                margin: 20px;
            }
            
            .main-greeting {
                font-size: 2.2rem;
            }
            
            .sub-greeting {
                font-size: 1.2rem;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
                gap: 15px;
            }
        }
    </style>
</head>
<body>
    <div class="greeting-container">
        <div class="floating-particles">
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
        </div>
        
        <!-- Balloons -->
        <div class="balloons-container">
            <div class="balloon balloon-1"></div>
            <div class="balloon balloon-2"></div>
            <div class="balloon balloon-3"></div>
            <div class="balloon balloon-4"></div>
            <div class="balloon balloon-5"></div>
        </div>
        
        <!-- Confetti -->
        <div class="confetti-container">
            <div class="confetti confetti-1"></div>
            <div class="confetti confetti-2"></div>
            <div class="confetti confetti-3"></div>
            <div class="confetti confetti-4"></div>
            <div class="confetti confetti-5"></div>
            <div class="confetti confetti-6"></div>
            <div class="confetti confetti-7"></div>
            <div class="confetti confetti-8"></div>
            <div class="confetti confetti-9"></div>
        </div>
        
        <!-- Celebration Burst -->
        <div class="celebration-burst">
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
            <div class="burst-particle"></div>
        </div>
        
        <!-- Sparkles -->
        <div class="sparkles">
            <div class="sparkle"></div>
            <div class="sparkle"></div>
            <div class="sparkle"></div>
            <div class="sparkle"></div>
            <div class="sparkle"></div>
        </div>
        
        <div class="sun-icon">
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-ray"></div>
            <div class="sun-center"></div>
        </div>
        
        <h1 class="main-greeting">Happy New Month!</h1>
        <p class="sub-greeting">
            Welcome to <span class="highlight">June 2025</span> – the month when Britain basks in its <span class="highlight">longest days</span> and celebrates the magic of <span class="highlight">midsummer</span>! 
            As we approach the Summer Solstice on June 21st, let this season of extended daylight illuminate new opportunities and endless possibilities.
        </p>
        
        <div class="features-grid">
            <div class="feature-card">
                <span class="feature-icon">☀️</span>
                <div class="feature-title">Longest Days</div>
                <div class="feature-desc">Nearly 17 hours of daylight to fuel your ambitions</div>
            </div>
            
            <div class="feature-card">
                <span class="feature-icon">🎭</span>
                <div class="feature-title">Festival Season</div>
                <div class="feature-desc">Peak time for celebrations and cultural experiences</div>
            </div>
            
            <div class="feature-card">
                <span class="feature-icon">🌟</span>
                <div class="feature-title">Midsummer Magic</div>
                <div class="feature-desc">Ancient traditions meet modern possibilities</div>
            </div>
            
            <div class="feature-card">
                <span class="feature-icon">👨‍👩‍👧‍👦</span>
                <div class="feature-title">Connection Time</div>
                <div class="feature-desc">Father's Day brings families closer together</div>
            </div>
        </div>
        
        <div class="brand-signature">
            May this June bring you abundant light, growth, and community connection.<br>
            From all of us at <span class="brand-name">Stucommunify</span> ✨
        </div>
    </div>
</body>
</html>
