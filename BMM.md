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
        <h2 class="section-title centered-title alt">Filler Test Text</h2>
         <div id="question" class="question-text">Is the BMM in development?</div>
        <div id="answer" class="answer-text">NO</div>
        <div id="emoji" class="emoji-text">😡</div>
         <div class="counter-container">
        <h1 class="title">Time Since</h1>
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
    <footer>
        <p>&copy; 2025 Xzor • Created and maintained by Xzor • See you in the 'verse! ✨ </p><p id="myParagraph">π</p>
        <script>document.getElementById('myParagraph').addEventListener('mousedown', function(event) {if (event.ctrlKey && event.shiftKey && event.button === 0) {window.open('https://www.youtube.com/watch?v=EKuwyH1UeYw', '_blank');}});</script>
    </footer>
</div>
         
    
<style>
.question-text {
    font-size: 4rem;
    font-weight: bold;
    text-align: center;
    opacity: 1;
    animation: fadeOut 5s ease-in-out forwards;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    white-space: nowrap;
}

.answer-text {
    font-size: 8rem;
    font-weight: bold;
    text-align: center;
    color: #ff4444;
    opacity: 0;
    animation: fadeIn 2s ease-in-out 4s forwards;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-shadow: 3px 3px 6px rgba(255, 68, 68, 0.5);
}

.emoji-text {
    font-size: 4rem;
    text-align: center;
    opacity: 0;
    animation: emojiPop 1.5s ease-out 6.5s forwards;
    position: absolute;
    top: 65%;
    left: 50%;
    transform: translate(-50%, -50%);
    filter: drop-shadow(2px 2px 4px rgba(0, 0, 0, 0.3));
}
.container-lg, h1, a {
    background: transparent !important;
    border: none !important;
    box-shadow: none !important;
    padding: 0 !important;
    margin: 0 !important;
    max-width: none !important;
    width: 100% !important;
    height: 100vh !important;
    position: relative !important;
}
a {
    display: none;
}
@keyframes fadeOut {
    0% {
        opacity: 1;
    }
    70% {
        opacity: 1;
    }
    100% {
        opacity: 0;
    }
}

@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: translate(-50%, -50%) scale(0.8);
    }
    100% {
        opacity: 1;
        transform: translate(-50%, -50%) scale(1);
    }
}

@keyframes emojiPop {
    0% {
        opacity: 0;
        transform: translate(-50%, -50%) scale(0.3) rotate(-10deg);
    }
    50% {
        opacity: 1;
        transform: translate(-50%, -50%) scale(1.3) rotate(5deg);
    }
    70% {
        transform: translate(-50%, -50%) scale(0.9) rotate(-2deg);
    }
    85% {
        transform: translate(-50%, -50%) scale(1.1) rotate(1deg);
    }
    100% {
        opacity: 1;
        transform: translate(-50%, -50%) scale(1) rotate(0deg);
        animation: emojiWiggle 2s ease-in-out 0.5s infinite;
    }
}

@keyframes emojiWiggle {
    0%, 100% {
        transform: translate(-50%, -50%) rotate(0deg) scale(1);
    }
    25% {
        transform: translate(-50%, -50%) rotate(-3deg) scale(1.05);
    }
    75% {
        transform: translate(-50%, -50%) rotate(3deg) scale(1.05);
    }
}

@media (max-width: 768px) {
    .question-text {
        font-size: 2.5rem;
    }
    .answer-text {
        font-size: 5rem;
    }
    .emoji-text {
        font-size: 3rem;
    }
}

@media (max-width: 480px) {
    .question-text {
        font-size: 1.8rem;
    }
    .answer-text {
        font-size: 3.5rem;
    }
    .emoji-text {
        font-size: 2.5rem;
    }
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
