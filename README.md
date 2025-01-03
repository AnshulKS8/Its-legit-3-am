# message-for-you- <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To Ridhima</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Georgia', serif;
            background: linear-gradient(to bottom, #ffafbd, #ffc3a0);
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }
        .container {
            text-align: center;
            background: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
            width: 80%;
            max-width: 600px;
            position: relative;
        }
        h1 {
            font-size: 2.5rem;
            color: #ff6f61;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.2rem;
            line-height: 1.8;
            margin-bottom: 20px;
        }
        .footer {
            font-size: 1rem;
            color: #555;
            margin-top: 20px;
        }
        .hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            overflow: hidden;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background: red;
            clip-path: polygon(50% 0%, 61% 16%, 80% 16%, 100% 36%, 100% 60%, 50% 100%, 0% 60%, 0% 36%, 20% 16%, 39% 16%);
            animation: float 5s infinite;
        }
        @keyframes float {
            0% {
                transform: translateY(0) scale(1);
                opacity: 1;
            }
            100% {
                transform: translateY(-100vh) scale(0.5);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>To My Dearest Ridhima,</h1>
        <p>
            From the moment you walked into my life, everything changed. The world feels brighter, and my heart beats with a rhythm it never knew before. You are my sun on cloudy days, my calm amidst the chaos, and the dream I never want to wake up from.
        </p>
        <p>
            Every smile you share lights up my soul, and every laugh of yours is music to my ears. You are my favorite story, one I want to read and write forever. I cherish every moment we’ve spent together, and I look forward to the countless memories we’ll create.
        </p>
        <p>
            I admire your strength, your kindness, and the way you make the simplest things extraordinary. You’ve taught me what it truly means to love and be loved.
        </p>
        <p>
            With you, I’ve found my forever, my home, my everything. I promise to stand by you through every season, to hold your hand in every storm, and to celebrate every joy by your side.
        </p>
        <p>
            You are my greatest blessing, my love, and my life. I’m endlessly grateful for you, and I love you more than words could ever express.
        </p>
        <p class="footer">Forever yours,<br>[Your Name]</p>
        <p style="font-size: 1.5rem; color: #ff6f61; margin-top: 30px;">
            I created this for you at 3 am 💖
        </p>
    </div>
    <div class="hearts"></div>
    <script>
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 3 + 2 + 's';
            document.querySelector('.hearts').appendChild(heart);
            setTimeout(() => heart.remove(), 5000);
        }
        setInterval(createHeart, 300);
    </script>
</body>
</html>
