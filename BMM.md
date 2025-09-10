<head>  <meta name="darkreader-lock" /></head>
<div id="question" class="question-text">Is the BMM in development?</div>
<div id="answer" class="answer-text">NO</div>
<div id="emoji" class="emoji-text">😡</div>
<br>
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
    </div>
<style>
body {
    margin: 0;
    padding: 0;
    background-color: #0e1117;
    color: #fff;
    font-family: 'Arial', sans-serif;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    overflow: hidden;
}

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
// Ensure the animation works properly when the page loads
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
});
    
</script>
