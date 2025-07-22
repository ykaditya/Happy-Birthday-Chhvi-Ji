<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday My Love! 💕</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;600;700&family=Poppins:wght@300;400;600&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(135deg, #ffffff 0%, #ffebee 25%, #ffcdd2 50%, #ef9a9a 75%, #e57373 100%);
            background-size: 400% 400%;
            animation: gradientShift 12s ease infinite;
            height: 100vh;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
            font-family: 'Poppins', sans-serif;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .star {
            position: absolute;
            color: #f8bbd0;
            font-size: 12px;
            animation: twinkle 2s infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 1; }
        }

        .container {
            text-align: center;
            z-index: 10;
            padding: 3rem;
            max-width: 900px;
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.9), rgba(255, 255, 255, 0.7));
            border-radius: 30px;
            backdrop-filter: blur(10px);
            box-shadow: 0 20px 50px rgba(244, 143, 177, 0.15), 0 0 100px rgba(255, 255, 255, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.8);
            transition: all 0.5s ease;
            position: relative;
            overflow: hidden;
        }

        .container::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: conic-gradient(transparent, rgba(244, 143, 177, 0.1), transparent);
            animation: rotate 4s linear infinite;
            z-index: -1;
        }

        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        .container:hover {
            transform: translateY(-10px);
            box-shadow: 0 30px 60px rgba(244, 143, 177, 0.25), 0 0 150px rgba(255, 255, 255, 0.3);
        }

        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 4.5rem;
            font-weight: 700;
            background: linear-gradient(45deg, #e91e63, #f48fb1, #f8bbd0, #fce4ec, #e91e63);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientText 3s ease infinite, float 3s ease-in-out infinite;
            margin-bottom: 1.5rem;
            text-shadow: 0 0 30px rgba(233, 30, 99, 0.3);
            opacity: 1;
            animation-delay: 0.5s;
            animation-fill-mode: both;
        }

        @keyframes gradientText {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        .subtitle {
            font-size: 1.8rem;
            color: #ad1457;
            margin-bottom: 2.5rem;
            text-shadow: 0 2px 10px rgba(233, 30, 99, 0.1);
            opacity: 0;
            animation: slideInUp 1s ease forwards 1.5s;
            font-weight: 300;
            letter-spacing: 1px;
        }

        .love-message {
            font-size: 1.3rem;
            color: #c2185b;
            margin-bottom: 2.5rem;
            font-style: italic;
            opacity: 0;
            animation: slideInUp 1s ease forwards 2s;
            line-height: 1.6;
        }

        .next-button {
            padding: 1.2rem 4rem;
            font-family: 'Poppins', sans-serif;
            font-size: 1.4rem;
            background: linear-gradient(45deg, #e91e63, #f48fb1, #f8bbd0, #e91e63);
            background-size: 300% 300%;
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 10px 30px rgba(233, 30, 99, 0.3);
            transition: all 0.3s ease;
            opacity: 0;
            animation: bounceIn 1s ease forwards 3s, buttonGlow 2s ease-in-out infinite 4s;
            font-weight: 500;
            letter-spacing: 1px;
            position: relative;
            overflow: hidden;
        }

        .next-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
            transition: left 0.5s;
        }

        .next-button:hover::before {
            left: 100%;
        }

        .next-button:hover {
            transform: scale(1.05) translateY(-5px);
            box-shadow: 0 15px 40px rgba(233, 30, 99, 0.5);
            background: linear-gradient(45deg, #f8bbd0, #f48fb1, #e91e63, #c2185b);
        }

        @keyframes buttonGlow {
            0%, 100% { box-shadow: 0 10px 30px rgba(233, 30, 99, 0.3); }
            50% { box-shadow: 0 10px 30px rgba(233, 30, 99, 0.6), 0 0 50px rgba(233, 30, 99, 0.3); }
        }

        .audio-controls {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.6));
            backdrop-filter: blur(10px);
            padding: 15px 20px;
            border-radius: 50px;
            display: flex;
            align-items: center;
            z-index: 100;
            box-shadow: 0 10px 30px rgba(233, 30, 99, 0.15);
            border: 1px solid rgba(255, 255, 255, 0.8);
            transition: all 0.3s ease;
        }

        .audio-controls:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(233, 30, 99, 0.2);
        }

        .audio-controls button {
            background: none;
            border: none;
            font-size: 1.8rem;
            cursor: pointer;
            color: #e91e63;
            margin-right: 15px;
            transition: all 0.3s ease;
            padding: 5px;
            border-radius: 50%;
        }

        .audio-controls button:hover {
            transform: scale(1.3);
            background: rgba(233, 30, 99, 0.1);
        }

        .audio-controls input {
            width: 120px;
            height: 5px;
            background: rgba(233, 30, 99, 0.2);
            border-radius: 5px;
            outline: none;
            -webkit-appearance: none;
        }

        .audio-controls input::-webkit-slider-thumb {
            appearance: none;
            width: 15px;
            height: 15px;
            background: #e91e63;
            border-radius: 50%;
            cursor: pointer;
            box-shadow: 0 2px 10px rgba(233, 30, 99, 0.3);
        }

        .floating-hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 2;
        }

        .heart {
            position: absolute;
            color: #e91e63;
            font-size: 20px;
            animation: floatUp 8s linear infinite;
            opacity: 0.8;
        }

        @keyframes floatUp {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.8;
            }
            90% {
                opacity: 0.8;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }

        .sparkle {
            position: absolute;
            width: 6px;
            height: 6px;
            background: #f8bbd0;
            border-radius: 50%;
            animation: sparkleAnim 2s ease-in-out infinite;
            pointer-events: none;
        }

        @keyframes sparkleAnim {
            0%, 100% {
                opacity: 0;
                transform: scale(0);
            }
            50% {
                opacity: 1;
                transform: scale(1);
            }
        }

        @keyframes slideInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes bounceIn {
            0% {
                opacity: 0;
                transform: scale(0.3);
            }
            50% {
                opacity: 1;
                transform: scale(1.05);
            }
            70% {
                transform: scale(0.9);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            h1 {
                font-size: 3rem;
            }
            .subtitle {
                font-size: 1.4rem;
            }
            .love-message {
                font-size: 1.1rem;
            }
            .container {
                width: 95%;
                padding: 2rem;
            }
            .next-button {
                padding: 1rem 2.5rem;
                font-size: 1.3rem;
            }
            .audio-controls {
                bottom: 20px;
                right: 20px;
                padding: 10px 15px;
            }
        }

        /* Special effects */
        .glow {
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from {
                text-shadow: 0 0 20px rgba(233, 30, 99, 0.3);
            }
            to {
                text-shadow: 0 0 30px rgba(233, 30, 99, 0.6), 0 0 40px rgba(244, 143, 177, 0.4);
            }
        }
    </style>
</head>
<body>
    <div class="stars"></div>
    <div class="floating-hearts"></div>
    
    <div class="container">
       <!-- ...existing code... -->
<h1 class="glow">Happy Birthday My Love! 💕✨</h1>
        <div class="subtitle">
            To the most amazing woman in my life
        </div>
        <div class="love-message">
            "Every moment with you is a gift, and today we celebrate the greatest gift of all - YOU! 🌹"
        </div>
        <button class="next-button" onclick="goToNextPage()">
            Begin Your Surprise! 💖
        </button>
    </div>

    


    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.11.4/gsap.min.js"></script>
    <script>
        // Audio controls
        const audio = document.getElementById('birthday-song');
        const playPauseBtn = document.getElementById('play-pause');
        const volumeControl = document.getElementById('volume');
        let isPlaying = false;

        audio.volume = volumeControl.value;

        // Auto-play with user interaction
        document.addEventListener('click', function() {
            if (!isPlaying) {
                audio.play().then(() => {
                    isPlaying = true;
                    playPauseBtn.textContent = '⏸️';
                }).catch(e => console.log('Audio play failed:', e));
            }
        }, { once: true });

        playPauseBtn.addEventListener('click', (e) => {
            e.stopPropagation();
            if (isPlaying) {
                audio.pause();
                playPauseBtn.textContent = '🎵';
            } else {
                audio.play();
                playPauseBtn.textContent = '⏸️';
            }
            isPlaying = !isPlaying;
        });

        volumeControl.addEventListener('input', () => {
            audio.volume = volumeControl.value;
        });

        // Next page function
        function goToNextPage() {
            gsap.to('.next-button', {
                scale: 1.3,
                rotation: 360,
                duration: 0.8,
                ease: "back.out(1.7)",
                onComplete: () => {
                    // Replace with your next page URL
                    
                     window.location.href = "memory.html";
                }
            });
        }

        // Create twinkling stars
        function createStars() {
            const starsContainer = document.querySelector('.stars');
            for (let i = 0; i < 100; i++) {
                const star = document.createElement('div');
                star.className = 'star';
                star.innerHTML = '✨';
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.animationDelay = Math.random() * 2 + 's';
                star.style.animationDuration = (Math.random() * 3 + 2) + 's';
                starsContainer.appendChild(star);
            }
        }

        // Create floating hearts
        function createHearts() {
            const heartsContainer = document.querySelector('.floating-hearts');
            setInterval(() => {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = ['💕', '💖', '💝', '💗', '💓', '💘'][Math.floor(Math.random() * 6)];
                heart.style.left = Math.random() * 100 + '%';
                heart.style.animationDuration = (Math.random() * 5 + 8) + 's';
                heart.style.fontSize = (Math.random() * 10 + 15) + 'px';
                heartsContainer.appendChild(heart);

                setTimeout(() => {
                    heart.remove();
                }, 8000);
            }, 1000);
        }

        // Create sparkles around the container
        function createSparkles() {
            const container = document.querySelector('.container');
            setInterval(() => {
                const sparkle = document.createElement('div');
                sparkle.className = 'sparkle';
                sparkle.style.left = Math.random() * 100 + '%';
                sparkle.style.top = Math.random() * 100 + '%';
                sparkle.style.animationDelay = Math.random() * 2 + 's';
                container.appendChild(sparkle);

                setTimeout(() => {
                    sparkle.remove();
                }, 2000);
            }, 200);
        }

        // Cursor sparkle effect
        document.addEventListener('mousemove', (e) => {
            if (Math.random() > 0.8) {
                const sparkle = document.createElement('div');
                sparkle.className = 'sparkle';
                sparkle.style.left = e.clientX + 'px';
                sparkle.style.top = e.clientY + 'px';
                sparkle.style.position = 'fixed';
                sparkle.style.pointerEvents = 'none';
                sparkle.style.zIndex = '1000';
                document.body.appendChild(sparkle);

                setTimeout(() => {
                    sparkle.remove();
                }, 2000);
            }
        });

        // Initialize all effects
        window.addEventListener('load', () => {
            createStars();
            createHearts();
            createSparkles();
            
            // Add some extra magic with GSAP
            gsap.timeline()
                .from('.container', { duration: 1, scale: 0.8, opacity: 0, ease: "back.out(1.7)" })
                .from('h1', { duration: 1, y: -50, opacity: 0, ease: "bounce.out" }, "-=0.5")
                .from('.subtitle', { duration: 0.8, y: 30, opacity: 0 }, "-=0.3")
                .from('.love-message', { duration: 0.8, y: 30, opacity: 0 }, "-=0.2")
                .from('.next-button', { duration: 0.8, scale: 0, opacity: 0, ease: "back.out(1.7)" }, "-=0.1");
        });

        // Add periodic container glow effect
        setInterval(() => {
            gsap.to('.container', {
                boxShadow: '0 20px 50px rgba(255, 107, 107, 0.3), 0 0 100px rgba(255, 255, 255, 0.3)',
                duration: 2,
                yoyo: true,
                repeat: 1
            });
        }, 5000);
    </script>
<!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Let's Celebrate with Cake!</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: linear-gradient(-45deg, #ff6b9d, #ff8fab, #fff, #ffe0e6);
            background-size: 400% 400%;
            animation: gradientBG 12s ease infinite;
            font-family: 'Arial', sans-serif;
            overflow-x: hidden;
            position: relative;
            padding: 20px;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Background particles */
        .particle {
            position: absolute;
            width: 8px;
            height: 8px;
            border-radius: 50%;
            pointer-events: none;
            opacity: 0.7;
            z-index: 1;
        }

        /* Sparkling stars */
        .star {
            position: absolute;
            width: 4px;
            height: 4px;
            background-color: #ff6b9d;
            border-radius: 50%;
            animation: twinkle 2s infinite alternate;
            z-index: 1;
        }

        @keyframes twinkle {
            0% { opacity: 0.3; transform: scale(0.8); }
            100% { opacity: 1; transform: scale(1.2); }
        }

       .heading {
    font-size: clamp(2rem, 6vw, 4rem);
    font-weight: bold;
    background: linear-gradient(90deg, #ff0080, #7928ca, #ffb347, #ff0080);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-shadow: 0 2px 8px #7928ca, 0 0 30px #fff, 0 0 10px #ff0080;
    margin-bottom: 2rem;
    text-align: center;
    animation: glow 2s ease-in-out infinite alternate;
    z-index: 10;
    position: relative;
}

        @keyframes glow {
            from { text-shadow: 0 0 20px rgba(255, 107, 157, 0.5); }
            to { text-shadow: 0 0 30px rgba(255, 107, 157, 0.8); }
        }

        .cake-container {
            position: relative;
            width: clamp(250px, 80vw, 350px);
            height: clamp(250px, 80vw, 350px);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: transform 0.3s ease;
            z-index: 10;
        }

        .cake-container:hover {
            transform: translateY(-10px) scale(1.02);
        }

        .click-message {
            position: absolute;
            top: -50px;
            font-size: clamp(1rem, 3vw, 1.2rem);
            color: white;
            background: linear-gradient(45deg, #ff6b9d, #e91e63);
            padding: 10px 20px;
            border-radius: 25px;
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.3s ease;
            animation: bounce 2s ease infinite;
            box-shadow: 0 5px 15px rgba(255, 107, 157, 0.4);
        }

        .cake-container:hover .click-message {
            opacity: 1;
            transform: translateY(0);
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }

        .cake {
            position: relative;
            width: 100%;
            height: 80%;
            max-width: 280px;
            max-height: 280px;
            transform-style: preserve-3d;
            transform: perspective(1000px) rotateX(3deg);
            transition: transform 0.3s ease;
            filter: drop-shadow(0 10px 20px rgba(255, 107, 157, 0.3));
        }

        .cake:hover {
            transform: perspective(1000px) rotateX(3deg) scale(1.05);
        }

        .layer {
            position: absolute;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.15);
            display: flex;
            justify-content: center;
            transition: all 0.3s ease;
        }

        .layer-1 {
            height: 25%;
            bottom: 0;
            width: 100%;
            background: linear-gradient(135deg, #ff6b9d, #e91e63);
        }

        .layer-2 {
            height: 22%;
            bottom: 25%;
            width: 85%;
            left: 7.5%;
            background: linear-gradient(135deg, #ff8fab, #ff6b9d);
        }

        .layer-3 {
            height: 20%;
            bottom: 47%;
            width: 70%;
            left: 15%;
            background: linear-gradient(135deg, #ffb3c6, #ff8fab);
        }

        .frosting {
            position: absolute;
            width: clamp(15px, 4vw, 25px);
            height: clamp(20px, 5vw, 35px);
            background: linear-gradient(135deg, #fff, #ffe0e6);
            border-radius: 50%;
            top: -50%;
            filter: drop-shadow(0 2px 5px rgba(0, 0, 0, 0.1));
        }

        .candle {
            position: absolute;
            width: clamp(18px, 4vw, 25px);
            height: clamp(50px, 12vw, 70px);
            background: linear-gradient(135deg, #fff, #ffe0e6);
            top: -80%;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 8px;
            z-index: 15;
            box-shadow: 0 0 10px rgba(255, 255, 255, 0.6);
        }

        .flame {
            position: absolute;
            width: clamp(15px, 4vw, 22px);
            height: clamp(20px, 5vw, 30px);
            background: linear-gradient(to bottom, #ffeb3b, #ff9800, #e91e63);
            border-radius: 50% 50% 30% 30%;
            top: -50%;
            left: 50%;
            transform: translateX(-50%);
            animation: flicker 1.5s infinite;
            filter: drop-shadow(0 0 10px #ff9800);
        }

        @keyframes flicker {
            0%, 100% { transform: translateX(-50%) scale(1); opacity: 1; }
            50% { transform: translateX(-50%) scale(0.95); opacity: 0.9; }
        }

        .balloon {
            position: fixed;
            width: clamp(40px, 10vw, 70px);
            height: clamp(50px, 12vw, 85px);
            top: 120%;
            border-radius: 50%;
            filter: drop-shadow(0 5px 10px rgba(0, 0, 0, 0.2));
            animation: balloonRise 8s ease-in-out forwards;
            z-index: 5;
        }

        .balloon::before {
            content: '';
            position: absolute;
            width: 8px;
            height: 12px;
            background: rgba(255, 255, 255, 0.9);
            bottom: -8px;
            left: 50%;
            transform: translateX(-50%);
            clip-path: polygon(0 0, 100% 0, 50% 100%);
        }

        .balloon::after {
            content: '';
            position: absolute;
            width: 1px;
            height: clamp(60px, 15vw, 100px);
            background: rgba(255, 255, 255, 0.8);
            bottom: -80px;
            left: 50%;
            transform: translateX(-50%);
        }

        @keyframes balloonRise {
            0% { transform: translateY(0) rotate(0deg) translateX(0); }
            25% { transform: translateY(-30vh) rotate(5deg) translateX(50px); }
            50% { transform: translateY(-60vh) rotate(-5deg) translateX(-30px); }
            75% { transform: translateY(-90vh) rotate(3deg) translateX(40px); }
            100% { transform: translateY(-130vh) rotate(0deg) translateX(0); }
        }

        .smoke {
            position: absolute;
            width: 8px;
            height: 8px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 50%;
            filter: blur(3px);
            opacity: 0;
        }

        .next-page-button {
            position: fixed;
            bottom: 40px;
            padding: clamp(12px, 3vw, 18px) clamp(30px, 8vw, 50px);
            font-size: clamp(1rem, 3vw, 1.3rem);
            background: linear-gradient(45deg, #ff6b9d, #e91e63);
            border: none;
            border-radius: 30px;
            color: white;
            cursor: pointer;
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.5s ease;
            box-shadow: 0 0 20px rgba(255, 107, 157, 0.5);
            font-family: 'Arial', sans-serif;
            font-weight: 600;
            z-index: 1000;
            display: flex;
            align-items: center;
            gap: 10px;
            overflow: hidden;
        }

        .next-page-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
            transition: left 0.5s ease;
        }

        .next-page-button::after {
            content: '→';
            font-size: 1.2em;
            transition: transform 0.3s ease;
        }

        .next-page-button:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 0 30px rgba(255, 107, 157, 0.7);
            background: linear-gradient(45deg, #ff8fab, #ff6b9d);
        }

        .next-page-button:hover::after {
            transform: translateX(5px);
        }

        .next-page-button:hover::before {
            left: 100%;
        }

        .next-page-button.show {
            opacity: 1;
            transform: translateY(0);
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
                box-shadow: 0 0 20px rgba(255, 107, 157, 0.5);
            }
            50% {
                transform: scale(1.02);
                box-shadow: 0 0 25px rgba(255, 107, 157, 0.7);
            }
        }

        /* Confetti animation */
        .confetti {
            position: absolute;
            width: 12px;
            height: 12px;
            top: -50px;
            z-index: 8;
        }

        @keyframes confettiFall {
            0% {
                opacity: 1;
                transform: translateY(0) rotateZ(0);
            }
            100% {
                opacity: 0.2;
                transform: translateY(100vh) rotateZ(360deg);
            }
        }

        /* Mobile responsiveness */
        @media (max-width: 768px) {
            body {
                padding: 10px;
            }

            .heading {
                margin-bottom: 1rem;
            }

            .cake-container {
                width: 90vw;
                height: 90vw;
                max-width: 300px;
                max-height: 300px;
            }

            .click-message {
                top: -40px;
                padding: 8px 16px;
            }

            .next-page-button {
                bottom: 20px;
                left: 50%;
                transform: translateX(-50%) translateY(50px);
            }

            .next-page-button.show {
                transform: translateX(-50%) translateY(0);
            }

            .next-page-button:hover {
                transform: translateX(-50%) translateY(-3px) scale(1.05);
            }
        }

        @media (max-width: 480px) {
            .cake-container {
                width: 85vw;
                height: 85vw;
            }

            .frosting {
                width: 12px;
                height: 18px;
            }

            .candle {
                width: 15px;
                height: 45px;
            }

            .flame {
                width: 12px;
                height: 18px;
            }
        }
    </style>
</head>
<body>
    <h1 class="heading">Let's Celebrate! 🎂</h1>
    <div class="cake-container">
        
        <div class="cake">
            <div class="layer layer-1">
                <div class="frosting"></div>
                <div class="frosting" style="left: 25%"></div>
                <div class="frosting" style="right: 25%"></div>
            </div>
            <div class="layer layer-2">
                <div class="frosting"></div>
                <div class="frosting" style="left: 30%"></div>
                <div class="frosting" style="right: 30%"></div>
            </div>
            <div class="layer layer-3">
                <div class="frosting"></div>
                <div class="frosting" style="left: 35%"></div>
                <div class="frosting" style="right: 35%"></div>
                <div class="candle">
                    <div class="flame"></div>
                </div>
            </div>
        </div>
    </div>
    <button class="next-page-button">Continue to Next Page</button>

    <script>
        const cake = document.querySelector('.cake-container');
        const candle = document.querySelector('.candle');
        const flame = document.querySelector('.flame');
        let isClicked = false;

        // Enhanced balloon colors - multiple vibrant colors
        const balloonColors = [
            'linear-gradient(135deg, #ff6b9d, #e91e63)',  // Pink-Red
            'linear-gradient(135deg, #4fc3f7, #29b6f6)',  // Blue
            'linear-gradient(135deg, #81c784, #4caf50)',  // Green
            'linear-gradient(135deg, #ffb74d, #ff9800)',  // Orange
            'linear-gradient(135deg, #ba68c8, #9c27b0)',  // Purple
            'linear-gradient(135deg, #fff176, #fdd835)',  // Yellow
            'linear-gradient(135deg, #ff8a65, #ff5722)',  // Red-Orange
            'linear-gradient(135deg, #4db6ac, #26a69a)',  // Teal
            'linear-gradient(135deg, #f06292, #e91e63)',  // Hot Pink
            'linear-gradient(135deg, #64b5f6, #2196f3)',  // Light Blue
            'linear-gradient(135deg, #aed581, #8bc34a)',  // Light Green
            'linear-gradient(135deg, #ffcc02, #ffc107)',  // Amber
        ];

        // Enhanced confetti colors
        const confettiColors = [
            '#ff6b9d', '#e91e63', '#fff', '#ff8fab', '#ffb3c6', '#ffe0e6',
            '#4fc3f7', '#29b6f6', '#81c784', '#4caf50', '#ffb74d', '#ff9800',
            '#ba68c8', '#9c27b0', '#fff176', '#fdd835', '#ff8a65', '#ff5722'
        ];

        // Create background particles
        function createBackgroundParticles() {
            for (let i = 0; i < 80; i++) {
                setTimeout(() => {
                    const particle = document.createElement('div');
                    particle.classList.add('particle');
                    particle.style.left = `${Math.random() * 100}%`;
                    particle.style.top = `${Math.random() * 100}%`;
                    particle.style.backgroundColor = confettiColors[Math.floor(Math.random() * confettiColors.length)];
                    particle.style.opacity = '0.6';
                    particle.style.transform = 'scale(0)';
                    document.body.appendChild(particle);

                    gsap.to(particle, {
                        scale: Math.random() * 1.5 + 0.5,
                        duration: 1.5,
                        ease: 'elastic.out(1, 0.5)'
                    });

                    gsap.to(particle, {
                        opacity: 0,
                        duration: 4,
                        delay: 2,
                        ease: 'power2.in',
                        onComplete: () => particle.remove()
                    });
                }, i * 80);
            }
        }

        // Create twinkling stars
        function createStars() {
            const starCount = window.innerWidth < 768 ? 30 : 60;
            for (let i = 0; i < starCount; i++) {
                const star = document.createElement('div');
                star.classList.add('star');
                star.style.left = `${Math.random() * 100}%`;
                star.style.top = `${Math.random() * 100}%`;
                star.style.animationDelay = `${Math.random() * 3}s`;
                document.body.appendChild(star);
            }
        }

        // Create initial stars
        createStars();

        function createConfetti() {
            const confetti = document.createElement('div');
            confetti.className = 'confetti';
            confetti.style.left = `${Math.random() * window.innerWidth}px`;
            
            // Enhanced shapes
            const shapes = ['circle', 'square', 'rectangle', 'triangle'];
            const shape = shapes[Math.floor(Math.random() * shapes.length)];
            
            const size = Math.random() * 8 + 6;
            confetti.style.width = `${size}px`;
            confetti.style.height = `${size}px`;
            
            if (shape === 'circle') {
                confetti.style.borderRadius = '50%';
            } else if (shape === 'triangle') {
                confetti.style.width = '0';
                confetti.style.height = '0';
                confetti.style.borderLeft = `${size/2}px solid transparent`;
                confetti.style.borderRight = `${size/2}px solid transparent`;
                confetti.style.borderBottom = `${size}px solid ${confettiColors[Math.floor(Math.random() * confettiColors.length)]}`;
                confetti.style.backgroundColor = 'transparent';
            } else {
                confetti.style.backgroundColor = confettiColors[Math.floor(Math.random() * confettiColors.length)];
                confetti.style.borderRadius = shape === 'square' ? '0' : '2px';
            }
            
            if (shape !== 'triangle') {
                confetti.style.backgroundColor = confettiColors[Math.floor(Math.random() * confettiColors.length)];
            }
            
            document.body.appendChild(confetti);

            // Enhanced animation
            gsap.to(confetti, {
                y: window.innerHeight + 100,
                x: Math.random() * 300 - 150,
                rotation: Math.random() * 720,
                duration: Math.random() * 4 + 3,
                ease: "power2.out",
                onComplete: () => confetti.remove()
            });
        }

        function createBalloon() {
            const balloon = document.createElement('div');
            balloon.className = 'balloon';
            balloon.style.left = `${Math.random() * (window.innerWidth - 70)}px`;
            balloon.style.background = balloonColors[Math.floor(Math.random() * balloonColors.length)];
            document.body.appendChild(balloon);

            // Enhanced wobble animation
            gsap.to(balloon, {
                x: `${Math.random() * 60 - 30}px`,
                duration: 3,
                repeat: -1,
                yoyo: true,
                ease: "sine.inOut"
            });

            balloon.addEventListener('animationend', () => {
                balloon.remove();
            });
        }

        function createSmoke() {
            const smoke = document.createElement('div');
            smoke.className = 'smoke';
            const cakeRect = cake.getBoundingClientRect();
            const candleRect = candle.getBoundingClientRect();
            smoke.style.left = `${candleRect.left + candleRect.width / 2}px`;
            smoke.style.top = `${candleRect.top - 10}px`;
            smoke.style.position = 'fixed';
            document.body.appendChild(smoke);

            gsap.to(smoke, {
                y: -40,
                x: Math.random() * 15 - 7,
                opacity: 0.4,
                scale: 1.5,
                duration: 2.5,
                ease: "power1.out",
                onComplete: () => smoke.remove()
            });
        }

        // Add smoke animation before clicking
        const smokeInterval = setInterval(createSmoke, 800);

        function startCelebration() {
            if (isClicked) return;
            isClicked = true;
            clearInterval(smokeInterval);

            // Create background particles
            createBackgroundParticles();

            // Enhanced cake bounce
            gsap.to(cake, {
                y: -30,
                rotation: 2,
                duration: 0.4,
                repeat: 1,
                yoyo: true,
                ease: "back.out(1.7)"
            });

            // Enhanced flame extinction
            gsap.to(flame, {
                scale: 3,
                opacity: 0,
                rotation: 45,
                duration: 0.6,
                ease: "power2.out"
            });

            gsap.to(candle, {
                opacity: 0,
                y: -40,
                scale: 0.8,
                duration: 1.2,
                delay: 0.3,
                ease: "back.in(1.7)",
                onComplete: () => candle.remove()
            });

            // Enhanced balloon celebration
            const balloonInterval = setInterval(() => {
                for (let i = 0; i < 3; i++) {
                    setTimeout(() => createBalloon(), i * 150);
                }
            }, 300);

            // Enhanced confetti celebration
            const confettiInterval = setInterval(() => {
                for (let i = 0; i < 15; i++) {
                    setTimeout(() => createConfetti(), i * 40);
                }
            }, 200);

            // Show next page button with enhanced animation
            setTimeout(() => {
                const nextButton = document.querySelector('.next-page-button');
                nextButton.classList.add('show');
                
                gsap.fromTo(nextButton, 
                    { y: 50, opacity: 0, scale: 0.8 }, 
                    { y: 0, opacity: 1, scale: 1, duration: 1.2, ease: "elastic.out(1, 0.5)" }
                );
            }, 1500);

            // Stop particle effects after celebration
            setTimeout(() => {
                clearInterval(balloonInterval);
                clearInterval(confettiInterval);
            }, 8000);
        }

        // Add button click handler
        document.querySelector('.next-page-button').addEventListener('click', () => {
            // Enhanced transition effect
            gsap.to(document.body, {
                opacity: 0,
                scale: 0.95,
                duration: 0.5,
                ease: "power2.in",
                onComplete: () => {
                    // You can replace this with your actual next page URL
                    window.location.href = 'celebrate.html';
                }
            });
        });

        // Handle window resize for mobile
        window.addEventListener('resize', () => {
            // Recreate stars on resize
            document.querySelectorAll('.star').forEach(star => star.remove());
            createStars();
        });

        cake.addEventListener('click', startCelebration);
    </script>
</body>
</html>
