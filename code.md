<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pirate Week 2025</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }

        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: white;
            border-radius: 50%;
            animation: twinkle 2s infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 1; }
        }

        .clouds {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 2;
        }

        .cloud {
            position: absolute;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 100px;
            animation: float 20s infinite linear;
        }

        @keyframes float {
            from { transform: translateX(-100%); }
            to { transform: translateX(100vw); }
        }

        .cloud1 { width: 100px; height: 40px; top: 10%; animation-duration: 25s; }
        .cloud2 { width: 150px; height: 50px; top: 20%; animation-duration: 30s; }
        .cloud3 { width: 120px; height: 45px; top: 30%; animation-duration: 28s; }
        .cloud4 { width: 80px; height: 35px; top: 50%; animation-duration: 22s; }
        .cloud5 { width: 110px; height: 42px; top: 60%; animation-duration: 26s; }
        .cloud6 { width: 90px; height: 38px; top: 75%; animation-duration: 24s; }

        .toggle-container {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 1000;
            transition: opacity 0.3s, transform 0.3s;
        }

        .toggle-switch {
            width: 80px;
            height: 40px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 20px;
            cursor: pointer;
            position: relative;
            transition: background 0.3s;
        }

        .toggle-slider {
            position: absolute;
            width: 36px;
            height: 36px;
            background: white;
            border-radius: 50%;
            top: 2px;
            left: 2px;
            transition: transform 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .toggle-switch.active .toggle-slider {
            transform: translateX(40px);
        }

        .icon {
            position: absolute;
            font-size: 20px;
        }

        .sun-icon {
            opacity: 1;
            transition: opacity 0.3s;
        }

        .moon-icon {
            opacity: 0;
            transition: opacity 0.3s;
        }

        .toggle-switch.active .sun-icon {
            opacity: 0;
        }

        .toggle-switch.active .moon-icon {
            opacity: 1;
        }

        body.night-mode {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
        }

        .container {
            position: relative;
            z-index: 10;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            text-align: center;
            color: white;
            padding: 40px 20px;
        }

        .xzor-ascii-banner {
            font-family: monospace;
            font-size: 1.2rem;
            line-height: 1.2;
            margin: 0;
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .no-underline {
            text-decoration: none;
        }

        .subtitle {
            font-size: 1.5rem;
            margin: 10px 0;
        }

        .tagline {
            font-size: 1rem;
            opacity: 0.8;
        }

        .profile-section {
            text-align: center;
        }

        :root {
            --size: 32px;
        }

        main {
            width: 100%;
            height: 100%;
            display: grid;
            place-items: center;
        }

        main button {
            font-size: var(--size);
            appearance: none;
            background: transparent;
            padding: 1em 2em;
            border-radius: 100px;
            border: 1px solid;
            color: white;
            position: relative;
            overflow: hidden;
            transition: color .40s ease;
            cursor: pointer;
        }

        main button:hover {
            color: black;
        }

        main button .btn-content {
            pointer-events: none;
            position: relative;
            z-index: 3;
        }

        main button .btn-cells {
            position: absolute;
            z-index: 2;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            display: grid;
            grid-template-columns: repeat(10, 1fr);
            grid-auto-rows: 1fr;
            overflow: hidden;
        }

        main button .btn-cells span {
            width: 100%;
            height: 100%;
            display: block;
            position: relative;
        }

        main button .btn-cells span:before {
            content: "";
            display: block;
            position: absolute;
            width: 50px;
            height: 50px;
            background: #ff69b4;
            background-image: linear-gradient(to right, #51F0ED, color-mix(in srgb, #51F0ED, white 50%));
            transition: transform .4s ease;
            transform: scale(0);
            border-radius: 100px;
        }

        main button .btn-cells span:hover:before {
            transform: scale(12);
        }

        main button .btn-cells span:hover ~ span:not(:hover) {
            pointer-events: none;
        }

        .paste-link {
            color: #007bff;
            text-decoration: none;
            font-size: 2.5rem;
            font-weight: 300;
            border-bottom: 1px solid #007bff;
            transition: color 0.3s;
        }

        .paste-link:hover {
            color: #0056b3;
        }

        .success-message {
            background: rgba(76, 175, 80, 0.3);
            color: white;
            padding: 15px;
            border-radius: 10px;
            border-left: 4px solid #4CAF50;
            opacity: 0;
            transition: opacity 0.3s;
        }

        .success-message.show {
            opacity: 1;
        }

        /* Button success state */
        main button.button-success {
            border-color: #4CAF50;
        }

        main button.button-success .btn-cells span:before {
            background: #4CAF50 !important;
            background-image: linear-gradient(to right, #4CAF50, #81C784) !important;
            transform: scale(12) !important;
        }

        .section-title {
            font-size: 2rem;
            color: white;
            margin: 20px 0;
        }

        .centered-title {
            text-align: center;
        }

        footer {
            text-align: center;
            color: white;
            padding: 20px;
            margin-top: 40px;
            opacity: 0.8;
        }
    </style>
</head>
<body>
    <!-- Background elements -->
    <div class="stars"></div>
    <div class="clouds">
        <div class="cloud cloud1"></div>
        <div class="cloud cloud2"></div>
        <div class="cloud cloud3"></div>
        <div class="cloud cloud4"></div>
        <div class="cloud cloud5"></div>
        <div class="cloud cloud6"></div>
    </div>
    
    <!-- Toggle Switch -->
    <div class="toggle-container" id="toggle-container" title="Toggle Day / Night Mode">
        <div class="toggle-switch" id="themeToggle">
            <div class="toggle-slider">
                <div class="icon sun-icon">☀️</div>
                <div class="icon moon-icon">🌙</div>
            </div>
        </div>
    </div>

    <div class="container">
        <header>
            <a class="no-underline" href="./">
                <h1 id='xzor-ascii-banner' class='xzor-ascii-banner'>██╗     ██╗███████╗   ██████╗   ██████╗   <br>
             ╚██╗██╔╝╚══███╔══███╔═══██╗██╔══██╗<br>
              &nbsp;&nbsp;&nbsp;╚███╔╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██████╔╝<br>
            &nbsp;&nbsp;&nbsp;██╔██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██╔══██╗<br>
           ██╔╝&nbsp;&nbsp;&nbsp;██╗███████╗╚██████╔╝██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║<br>
            ╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝╚══════╝&nbsp;&nbsp;&nbsp;╚═════╝&nbsp;&nbsp;&nbsp;╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝</h1>
            </a><br>
            <p class="subtitle theme-sensitive">Gaming Enthusiast & Digital Warrior</p>
            <p class="tagline">Exploring the cosmos, one game at a time</p>
        </header>
        
        <div class="profile-section">
            <h2 class="section-title centered-title alt">
                Pirate Week 2025 
            </h2>
            <div id="successMessage" class="success-message">Code copied to clipboard!</div>
            <br>
            <main>
                <button id="copyButton" onclick="copyCode()">
                    <div class="btn-cells">
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                    <span class="btn-content" id="btnContent">
                        Click here to copy code
                    </span>
                </button>
                <br><br><p style="color: white;">Then</p><br><br>
                <button onclick="window.open('https://robertsspaceindustries.com/en/comm-link/transmission/20733-Pirate-Week-2025#2addcbc3', '_blank', 'noopener, noreferrer')" class="paste-link">
                    <div class="btn-cells">
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                    <span class="btn-content">
                        Paste on this page
                    </span>
                </button>
            </main>
        </div>
        
        <footer>
            <p>&copy; 2025 Xzor • Created and maintained by Xzor • See you in the 'verse! ✨<span id="tms">π<script>document.getElementById('tms').addEventListener('mousedown', function(event) {if (event.ctrlKey && event.shiftKey && event.button === 0) {window.open('https://www.youtube.com/watch?v=EKuwyH1UeYw', '_blank');}});</script></span></p>
        </footer>
    </div>

    <script>
        //Copy Pasta Pirate Code
        const codeText = "M50-BT3480-7142-0059GM-ON-2-6-1STRD";
        
        function copyCode() {
            const copyButton = document.getElementById('copyButton');
            const btnContent = document.getElementById('btnContent');
            const originalText = btnContent.textContent;
            
            navigator.clipboard.writeText(codeText).then(function() {
                // Change button appearance
                copyButton.classList.add('button-success');
                btnContent.textContent = 'Code copied to clipboard!';
                
                const successMessage = document.getElementById('successMessage');
                successMessage.classList.add('show');
                
                setTimeout(function() {
                    successMessage.classList.remove('show');
                    copyButton.classList.remove('button-success');
                    btnContent.textContent = originalText;
                }, 2000);
            }).catch(function(err) {
                console.error('Failed to copy: ', err);
                // Fallback for older browsers
                const textArea = document.createElement('textarea');
                textArea.value = codeText;
                document.body.appendChild(textArea);
                textArea.select();
                document.execCommand('copy');
                document.body.removeChild(textArea);
                
                // Change button appearance
                copyButton.classList.add('button-success');
                btnContent.textContent = 'Code copied to clipboard!';
                
                const successMessage = document.getElementById('successMessage');
                successMessage.classList.add('show');
                
                setTimeout(function() {
                    successMessage.classList.remove('show');
                    copyButton.classList.remove('button-success');
                    btnContent.textContent = originalText;
                }, 2000);
            });
        }
        
        // Scroll to hide
        function initScrollHide() {
            const toggleContainer = document.getElementById('toggle-container');
            
            if (toggleContainer) {
                // Get the original transform value from CSS
                const computedStyle = getComputedStyle(toggleContainer);
                const originalTransform = computedStyle.transform;
                
                document.body.addEventListener('scroll', function() {
                    const scrollY = document.body.scrollTop || document.documentElement.scrollTop;
                    const maxScroll = 400;
                    
                    if (scrollY <= maxScroll) {
                        const opacity = Math.max(0, 1 - (scrollY / maxScroll));
                        const translateY = Math.min(scrollY * 0.5, 100);
                        
                        toggleContainer.style.opacity = opacity;
                        
                        // If there was an original transform, combine it with translateY
                        if (originalTransform && originalTransform !== 'none') {
                            toggleContainer.style.transform = `${originalTransform} translateY(-${translateY}%)`;
                        } else {
                            toggleContainer.style.transform = `translateY(-${translateY}%)`;
                        }
                    } else {
                        toggleContainer.style.opacity = '0';
                        
                        // Preserve original transform when fully hidden
                        if (originalTransform && originalTransform !== 'none') {
                            toggleContainer.style.transform = `${originalTransform} translateY(-100%)`;
                        } else {
                            toggleContainer.style.transform = 'translateY(-100%)';
                        }
                    }
                });
            }
        }
        
        initScrollHide();
        
        //end scroll to hide
        const toggle = document.getElementById('themeToggle');
        const body = document.body;
        const stars = document.querySelector('.stars');
        
        // Cookie utility functions
        function setCookie(name, value, days) {
            const expires = new Date();
            expires.setTime(expires.getTime() + (days * 24 * 60 * 60 * 1000));
            document.cookie = `${name}=${value};expires=${expires.toUTCString()};path=/`;
        }
        
        function getCookie(name) {
            const nameEQ = name + "=";
            const ca = document.cookie.split(';');
            for (let i = 0; i < ca.length; i++) {
                let c = ca[i];
                while (c.charAt(0) === ' ') c = c.substring(1, c.length);
                if (c.indexOf(nameEQ) === 0) return c.substring(nameEQ.length, c.length);
            }
            return null;
        }
        
        // Create stars
        function createStars() {
            stars.innerHTML = '';
            for (let i = 0; i < 300; i++) {
                const star = document.createElement('div');
                star.className = 'star';
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.animationDelay = Math.random() * 2 + 's';
                stars.appendChild(star);
            }
        }
        
        // Apply theme
        function applyTheme(isNightMode) {
            if (isNightMode) {
                toggle.classList.add('active');
                body.classList.add('night-mode');
            } else {
                toggle.classList.remove('active');
                body.classList.remove('night-mode');
            }
            
            // Update custom div classes
            updateCustomDivClasses(isNightMode);
        }
        
        // Function to update custom div classes
        function updateCustomDivClasses(isNightMode) {
            const xzorBannerDiv = document.getElementById('xzor-ascii-banner');
            
            if (xzorBannerDiv) {
                if (isNightMode) {
                    xzorBannerDiv.classList.remove('day-style');
                    xzorBannerDiv.classList.add('night-style');
                } else {
                    xzorBannerDiv.classList.remove('night-style');
                    xzorBannerDiv.classList.add('day-style');
                }
            }
            
            // Update multiple elements with a specific class
            const themeElements = document.querySelectorAll('.theme-sensitive');
            themeElements.forEach(element => {
                if (isNightMode) {
                    element.classList.add('dark-mode');
                    element.classList.remove('light-mode');
                } else {
                    element.classList.add('light-mode');
                    element.classList.remove('dark-mode');
                }
            });
        }
        
        // Initialize theme from cookie
        function initializeTheme() {
            const savedTheme = getCookie('themePreference');
            const isNightMode = savedTheme === 'night';
            applyTheme(isNightMode);
        }
        
        createStars();
        
        // Load saved theme on page load
        initializeTheme();
        
        // Toggle functionality
        toggle.addEventListener('click', function() {
            const willBeNightMode = !body.classList.contains('night-mode');
            applyTheme(willBeNightMode);
            
            // Save preference to cookie (expires in 365 days)
            setCookie('themePreference', willBeNightMode ? 'night' : 'day', 365);
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
</html>
