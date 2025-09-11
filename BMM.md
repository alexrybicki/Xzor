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
            <div id="question" class="question-text">Is the BMM in development?</div>
            <div id="answer" class="answer-text">NO</div>
            <div id="emoji" class="emoji-text">😡</div>
        </div>
         <div class="counter-container">
        <h2 class="section-title centered-title alt">Time Since</h2>
        <div class="date">November 11, 2013</div>
        <div class="time-display">
            <div class="time-unit">
                <span class="time-number" id="years">0</span>
                <span class="time-label">Years</span>
            </div>
            <div class="time-unit">
                <span class="time-number" id="months">0</span>
                <span class="time-label">Months</span>
            </div>
            <div class="time-unit">
                <span class="time-number" id="days">0</span>
                <span class="time-label">Days</span>
            </div>
        </div>
        <div class="total-days">
            <div>Total Days: <span class="total-days-number" id="totalDays">0</span></div>
     </div>
</div>
</div>
    <footer>
        <p>&copy; 2025 Xzor • Created and maintained by Xzor • See you in the 'verse! ✨ </p><p id="myParagraph">π</p>
        <script>document.getElementById('myParagraph').addEventListener('mousedown', function(event) {if (event.ctrlKey && event.shiftKey && event.button === 0) {window.open('https://www.youtube.com/watch?v=EKuwyH1UeYw', '_blank');}});</script>
    </footer>

         
    
<style>
  body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            margin: 0;
            padding: 0;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .counter-container {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            text-align: center;
            max-width: 600px;
            width: 90%;
        }
        
        .title {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #333;
            font-weight: 300;
        }
        
        .date {
            font-size: 1.2rem;
            color: #666;
            margin-bottom: 40px;
            font-style: italic;
        }
        
        .time-display {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .time-unit {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            border-radius: 15px;
            padding: 20px;
            color: white;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            transform: translateY(0);
            transition: transform 0.3s ease;
        }
        
        .time-unit:hover {
            transform: translateY(-5px);
        }
        
        .time-number {
            font-size: 2.5rem;
            font-weight: bold;
            display: block;
            margin-bottom: 5px;
        }
        
        .time-label {
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            opacity: 0.9;
        }
        
        .total-days {
            margin-top: 30px;
            padding: 20px;
            background: rgba(102, 126, 234, 0.1);
            border-radius: 10px;
            border-left: 4px solid #667eea;
        }
        
        .total-days-number {
            font-size: 2rem;
            font-weight: bold;
            color: #667eea;
        }
</style>
<script>

document.addEventListener('DOMContentLoaded', function() {
    const question = document.getElementById('question');
    const answer = document.getElementById('answer');
    const emoji = document.getElementById('emoji');
    // Reset animations if page is refreshed
    question.style.animation = 'none';
    answer.style.animation = 'none';
    emoji.style.animation = 'none';
    // Trigger animations with a small delay
    setTimeout(() => {
        question.style.animation = 'fadeOut 5s ease-in-out forwards';
        answer.style.animation = 'fadeIn 2s ease-in-out 4s forwards';
        emoji.style.animation = 'emojiPop 1.5s ease-out 6.5s forwards';
        // Add continuous wiggle after the pop animation
        setTimeout(() => {
            emoji.style.animation += ', emojiWiggle 2s ease-in-out 0.5s infinite';
        }, 8000); // 6.5s delay + 1.5s pop duration
    }, 100);
    // Time Since Announced
     function calculateTimeSince() {
            // Target date: November 11, 2013
            const targetDate = new Date('2013-11-11T00:00:00');
            const currentDate = new Date();            
            // Calculate total days
            const totalMilliseconds = currentDate - targetDate;
            const totalDays = Math.floor(totalMilliseconds / (1000 * 60 * 60 * 24));            
            // Calculate years, months, and remaining days
            let years = currentDate.getFullYear() - targetDate.getFullYear();
            let months = currentDate.getMonth() - targetDate.getMonth();
            let days = currentDate.getDate() - targetDate.getDate();            
            // Adjust for negative days
            if (days < 0) {
                months--;
                const lastMonth = new Date(currentDate.getFullYear(), currentDate.getMonth(), 0);
                days += lastMonth.getDate();
            }            
            // Adjust for negative months
            if (months < 0) {
                years--;
                months += 12;
            }            
            // Update the display
            document.getElementById('years').textContent = years;
            document.getElementById('months').textContent = months;
            document.getElementById('days').textContent = days;
            document.getElementById('totalDays').textContent = totalDays.toLocaleString();
        }        
        // Calculate immediately when page loads
        calculateTimeSince();        
        // Update every second
        setInterval(calculateTimeSince, 1000);
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
        // Ensure the animation works properly when the page loads
});
    </script>
</body>
