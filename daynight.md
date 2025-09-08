<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Day/Night Toggle Switch</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Arial', sans-serif;
            transition: background 0.8s ease;
            background: linear-gradient(135deg, #87CEEB 0%, #98D8E8 50%, #F0F8FF 100%);
        }
        body.night-mode {
            background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
        }
        .toggle-container {
            position: relative;
            display: inline-block;
        }
        .toggle-switch {
            width: 80px;
            height: 40px;
            background: linear-gradient(145deg, #e6e6e6, #ffffff);
            border-radius: 50px;
            position: relative;
            cursor: pointer;
            box-shadow: 
                inset 2px 2px 5px rgba(0,0,0,0.1),
                inset -2px -2px 5px rgba(255,255,255,0.8),
                2px 2px 10px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            border: 2px solid #ddd;
        }
        .toggle-switch.active {
            background: linear-gradient(145deg, #2c3e50, #34495e);
            border-color: #34495e;
            box-shadow: 
                inset 2px 2px 5px rgba(0,0,0,0.3),
                inset -2px -2px 5px rgba(255,255,255,0.1),
                2px 2px 15px rgba(0,0,0,0.2);
        }
        .toggle-slider {
            width: 32px;
            height: 32px;
            background: linear-gradient(145deg, #ffffff, #f0f0f0);
            border-radius: 50%;
            position: absolute;
            top: 2px;
            left: 2px;
            transition: all 0.4s cubic-bezier(0.68, -0.55, 0.265, 1.55);
            box-shadow: 
                2px 2px 8px rgba(0,0,0,0.2),
                inset 1px 1px 3px rgba(255,255,255,0.8),
                inset -1px -1px 3px rgba(0,0,0,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }
        .toggle-switch.active .toggle-slider {
            transform: translateX(40px);
            background: linear-gradient(145deg, #f39c12, #e67e22);
            box-shadow: 
                2px 2px 12px rgba(243, 156, 18, 0.4),
                inset 1px 1px 3px rgba(255,255,255,0.3),
                inset -1px -1px 3px rgba(0,0,0,0.2);
        }
        .icon {
            font-size: 16px;
            transition: all 0.3s ease;
            position: absolute;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .sun-icon {
            color: #f39c12;
            transform: rotate(0deg);
            opacity: 1;
        }
        .moon-icon {
            color: #bdc3c7;
            transform: rotate(180deg);
            opacity: 0;
        }
        .toggle-switch.active .sun-icon {
            transform: rotate(180deg);
            opacity: 0;
        }
        .toggle-switch.active .moon-icon {
            transform: rotate(0deg);
            opacity: 1;
        }
        /* Stars animation for night mode */
        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            opacity: 0;
            transition: opacity 0.8s ease;
        }
        body.night-mode .stars {
            opacity: 1;
        }
        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: white;
            border-radius: 50%;
            animation: twinkle 2s infinite alternate;
        }
        @keyframes twinkle {
            0% { opacity: 0.3; }
            100% { opacity: 1; }
        }
        /* Clouds for day mode */
        .clouds {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            opacity: 1;
            transition: opacity 0.8s ease;
        }
        body.night-mode .clouds {
            opacity: 0;
        }
        .cloud {
            position: absolute;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 50px;
            animation: float 20s infinite linear;
        }
        .cloud::before,
        .cloud::after {
            content: '';
            position: absolute;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 50px;
        }
        .cloud1 {
            width: 80px;
            height: 40px;
            top: 20%;
            left: -100px;
            animation-duration: 25s;
        }
        .cloud1::before {
            width: 50px;
            height: 50px;
            top: -25px;
            left: 10px;
        }
        .cloud1::after {
            width: 60px;
            height: 40px;
            top: -15px;
            right: 10px;
        }
        .cloud2 {
            width: 60px;
            height: 30px;
            top: 40%;
            left: -80px;
            animation-duration: 30s;
            animation-delay: -10s;
        }
        .cloud2::before {
            width: 40px;
            height: 40px;
            top: -20px;
            left: 5px;
        }
        .cloud2::after {
            width: 45px;
            height: 30px;
            top: -10px;
            right: 5px;
        }
        @keyframes float {
            0% { transform: translateX(-100px); }
            100% { transform: translateX(calc(100vw + 100px)); }
        }
        /* Demo text */
        .demo-text {
            position: absolute;
            top: 70%;
            left: 50%;
            transform: translateX(-50%);
            color: #333;
            font-size: 18px;
            font-weight: 500;
            transition: color 0.8s ease;
            text-shadow: 1px 1px 3px rgba(255,255,255,0.8);
        }
        body.night-mode .demo-text {
            color: #ecf0f1;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.8);
        }
    </style>
</head>
<body>
    <!-- Background elements -->
    <div class="stars"></div>
    <div class="clouds">
        <div class="cloud cloud1"></div>
        <div class="cloud cloud2"></div>
    </div>
    <!-- Toggle Switch -->
    <div class="toggle-container">
        <div class="toggle-switch" id="themeToggle">
            <div class="toggle-slider">
                <div class="icon sun-icon">☀️</div>
                <div class="icon moon-icon">🌙</div>
            </div>
        </div>
    </div>
<div class="container">
    <header>
        <a class="no-underline" href="./" >
        <h1 class='xzor-ascii-banner'>██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██╗███████╗&nbsp;&nbsp;&nbsp;██████╗&nbsp;&nbsp;&nbsp;██████╗&nbsp;&nbsp;&nbsp;<br>
             ╚██╗██╔╝╚══███╔╝██╔═══██╗██╔══██╗<br>
              &nbsp;&nbsp;&nbsp;╚███╔╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██████╔╝<br>
            &nbsp;&nbsp;&nbsp;██╔██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██╔══██╗<br>
           ██╔╝&nbsp;&nbsp;&nbsp;██╗███████╗╚██████╔╝██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║<br>
            ╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝╚══════╝&nbsp;&nbsp;&nbsp;╚═════╝&nbsp;&nbsp;&nbsp;╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝</h1></a><br>
        <p class="subtitle">Gaming Enthusiast & Digital Warrior</p>
        <p class="tagline">Exploring the cosmos, one game at a time</p>
    </header>
     <div class="profile-section">
        <h2 class="section-title centered-title alt">Filler Test Text</h2>
        <p class="about-text">
           This is just some filler testing text. Yay. 😃
        </p>
    </div>
</div>    <script>
        const toggle = document.getElementById('themeToggle');
        const body = document.body;
        const stars = document.querySelector('.stars');
        // Create stars
        function createStars() {
            stars.innerHTML = '';
            for (let i = 0; i < 100; i++) {
                const star = document.createElement('div');
                star.className = 'star';
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.animationDelay = Math.random() * 2 + 's';
                stars.appendChild(star);
            }
        }
        createStars();
        // Toggle functionality
        toggle.addEventListener('click', function() {
            toggle.classList.toggle('active');
            body.classList.toggle('night-mode');
        });
        // Optional: Add keyboard support
        toggle.addEventListener('keydown', function(e) {
            if (e.key === 'Enter' || e.key === ' ') {
                e.preventDefault();
                toggle.click();
            }
        });
        // Make toggle focusable
        toggle.setAttribute('tabindex', '0');
    </script>
</body>
