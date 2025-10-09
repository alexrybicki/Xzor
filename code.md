
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
  <style> 
        .profile-section {
          text-align: center;
        }
main {
  display: grid;
  place-items: center;
}
button {
  --transition-duration: 400ms;
  font-size: 2rem;
  appearance: none;
  background: transparent;
  padding: 1em 2em;
  border-radius: 100px;
  border: 1px solid;
  color: white;
  position: relative;
  overflow: hidden;
  transition: color var(--transition-duration) ease;
  &:hover {
    color: black;
  }
}
.btn-content {
  pointer-events: none;
  position: relative;
  z-index: 3;
}
.btn-cells {
  position: absolute;
  z-index: 2;
  inset: 0;  
  display: grid;
  grid-template-columns: repeat(10, 1fr);
  &::before {
    content: "";
    position: absolute;
    position-anchor: --hovered-cell;
    left: calc(anchor(left) - 20px);
    right: calc(anchor(right) - 20px);
    top: calc(anchor(top) - 20px);
    bottom: calc(anchor(bottom) - 20px);
    margin: 0 auto auto;
  }
  &:has(> :nth-child(n + 11):hover)::before {
    margin: auto auto 0;
  }
  &:hover::before {
    transform: scale(55);
    transition: transform var(--transition-duration) ease, margin 0ms 0ms;
  }
  & span {
    position: relative;
  }
  &:not(:hover) span {
  }
  & span:hover {
    anchor-name: --hovered-cell;
    transition: anchor-name 0ms;
  }
}
body:has(#debug:checked) .btn-cells span {
  outline: 1px solid red;
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
    </style>
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
         <h2 class="section-title centered-title alt">
            Pirate Week 2025 
          </h2>
        <div id="successMessage" class="success-message">Code copied to clipboard!</div>
            <br>
            <main>
            <button onclick="copyCode()">
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
                Click to copy code
              </span>
            </button>
        <br><br><p>Then</p><br><br>
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
    <script>
        //Copy Pasta Pirate Code
        const codeText = "M50-BT3480-7142-0059GM-ON-2-6-1STRD";        
        function copyCode() {
            navigator.clipboard.writeText(codeText).then(function() {
                const successMessage = document.getElementById('successMessage');
                successMessage.classList.add('show');
                setTimeout(function() {
                    successMessage.classList.remove('show');
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
                const successMessage = document.getElementById('successMessage');
                successMessage.classList.add('show');
                setTimeout(function() {
                    successMessage.classList.remove('show');
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
    </div>
</body>
