<body>
    <style>
        table {
            width: 100%;
            max-width: 1000px;
            margin: 0 auto;
            border-collapse: collapse;
            /* background-color: white; */
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        th {
            /* background-color: #b8cce4; */
            color: #fff;
            padding: 12px;
            text-align: left;
            font-weight: bold;
            border: 1px solid #999;
        }
        td {
            padding: 12px;
            border: 1px solid #999;
        }
        tr:nth-child(even) {
            /* background-color: #dce6f1; */
        }
        tr:nth-child(odd) {
            /* background-color: #fff; */
        }
        .free-fly-yes {
            background-color: #1d4b26;
            text-align: center;
            font-weight: bold;
        }
        .free-fly-no {
            /* background-color: #fff; */
        }
</style>
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
        <a class="no-underline" href="./" >
        <h1 id='xzor-ascii-banner' class='xzor-ascii-banner'>██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██╗███████╗&nbsp;&nbsp;&nbsp;██████╗&nbsp;&nbsp;&nbsp;██████╗&nbsp;&nbsp;&nbsp;<br>
             ╚██╗██╔╝╚══███╔╝██╔═══██╗██╔══██╗<br>
              &nbsp;&nbsp;&nbsp;╚███╔╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██████╔╝<br>
            &nbsp;&nbsp;&nbsp;██╔██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██╔══██╗<br>
           ██╔╝&nbsp;&nbsp;&nbsp;██╗███████╗╚██████╔╝██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║<br>
            ╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝╚══════╝&nbsp;&nbsp;&nbsp;╚═════╝&nbsp;&nbsp;&nbsp;╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝</h1></a><br>
        <p class="subtitle theme-sensitive">Gaming Enthusiast & Digital Warrior</p>
        <p class="tagline">Exploring the cosmos, one game at a time</p>
    </header>
     <div class="profile-section">
        <h2 class="section-title centered-title alt theme-sensitive">Star Citizen Event Calendar</h2>
    <table class="theme-sensitive dark-mode">
        <thead>
            <tr>
                <th>MONTH</th>
                <th>EVENT</th>
                <th>FREE FLY</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>January</td>
                <td>Red Festival (Lunar New Year) 🧧</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>February</td>
                <td>Coramor (Valentine's Day) ❤️</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>March</td>
                <td>Stella Fortuna (St. Patrick's Day) 🍀</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>April</td>
                <td>Triggerfish (April Fools' Day)</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>May</td>
                <td>Invictus Launch Week</td>
                <td class="free-fly-yes">YES</td>
            </tr>
            <tr>
                <td>June</td>
                <td>Alien Week 👽</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>July</td>
                <td>Foundation Festival</td>
                <td class="free-fly-yes">YES</td>
            </tr>
            <tr>
                <a class="no-underline" href="https://play.sc/shipshowdown" >
                <td>August</td>
                <td>Ship Showdown 🚀</td>
                <td class="free-fly-yes">YES</td>
                </a>
            </tr>
            <tr>
                <td>September</td>
                <td>Pirate Week 🏴‍☠️</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>October</td>
                <td>Citizen Con &nbsp;&nbsp;&nbsp;&nbsp; Day of the Vara (Halloween) 🎃</td>
                <td class="free-fly-no"></td>
            </tr>
            <tr>
                <td>November</td>
                <td>Intergalactic Aerospace Expo</td>
                <td class="free-fly-yes">YES</td>
            </tr>
            <tr>
                <td>December</td>
                <td>Luminalia (X-Mas) 🎄</td>
                <td class="free-fly-no"></td>
            </tr>
        </tbody>
    </table>
    </div>
    <footer>
        <p>&copy; 2025 Xzor • Created and maintained by Xzor • See you in the 'verse! ✨<span id="tms">π<script>document.getElementById('tms').addEventListener('mousedown', function(event) {if (event.ctrlKey && event.shiftKey && event.button === 0) {window.open('https://www.youtube.com/watch?v=EKuwyH1UeYw', '_blank');}});</script></span></p>
    </footer>
</div>
    <script>
                        // Scroll to hide
        function initScrollHide() {
            const toggleContainer = document.getElementById('toggle-container');    
            if (toggleContainer) {
                // Get the original transform value from CSS
                const computedStyle = getComputedStyle(toggleContainer);
                const originalTransform = computedStyle.transform;
                // console.log('Original transform:', originalTransform);        
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
            for (let i = 0; i <300; i++) {
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
