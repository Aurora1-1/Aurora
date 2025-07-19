<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Photo & Video Enhancer</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: var(--bg-color);
            color: var(--text-color);
            text-align: center;
            position: relative;
            transition: background 0.5s, color 0.5s;
        }
        :root {
            --bg-color: #1d2b64;
            --text-color: white;
        }
        .light-theme {
            --bg-color: #f8f9fa;
            --text-color: #212529;
        }
        .astronaut-theme {
            --bg-color: linear-gradient(135deg, #3a1c71, #d76d77, #ffaf7b);
            --text-color: #ffffff;
        }
        .header {
            padding: 20px;
            background-color: rgba(0,0,0,0.6);
        }
        .announcement {
            background-color: #ff9800;
            color: black;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            font-weight: bold;
        }
        .theme-toggle {
            position: absolute;
            top: 20px;
            right: 20px;
            padding: 10px;
            cursor: pointer;
            background: #fff;
            border: none;
            border-radius: 5px;
            font-weight: bold;
        }
        .features, .section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
        }
        .feature-card, .section-card {
            background: rgba(255,255,255,0.1);
            border-radius: 10px;
            padding: 20px;
            width: 250px;
            box-shadow: 0 0 10px rgba(0,0,0,0.5);
        }
        .logo {
            position: fixed;
            bottom: 10px;
            left: 10px;
            background-color: rgba(0,0,0,0.5);
            padding: 5px 10px;
            border-radius: 5px;
            font-weight: bold;
            font-size: 1.2rem;
            font-family: 'Brush Script MT', cursive;
        }
        footer {
            margin-top: 40px;
            font-size: 0.8rem;
            opacity: 0.6;
        }
    </style>
</head>
<body><button class="theme-toggle" onclick="toggleTheme()">Toggle Theme</button>

<div class="header">
    <h1 style="font-family: 'Brush Script MT', cursive; font-size: 3rem;">Welcome to Aurora</h1>
    <p>Where Creativity Meets Intelligence. 🚀</p>
</div>

<div class="announcement">
    🎉 Official Launch on <strong>1 February 2026</strong>! Stay tuned! 🎉
</div>

<h2>Explore Our Extensive Features ✨</h2>
<div class="features" id="features"></div>

<h2>About Us</h2>
<div class="section" id="about"></div>

<h2>Contact</h2>
<div class="section" id="contact"></div>

<h2>Team</h2>
<div class="section" id="team"></div>

<h2>Blog / Updates</h2>
<div class="section" id="blog"></div>

<div class="logo">A</div>

<footer>
    &copy; 2026 Aurora - All rights reserved.
</footer>

<script>
    let currentTheme = 0;
    const themes = ['', 'light-theme', 'astronaut-theme'];

    function toggleTheme() {
        document.body.classList.remove(themes[currentTheme]);
        currentTheme = (currentTheme + 1) % themes.length;
        if (themes[currentTheme]) {
            document.body.classList.add(themes[currentTheme]);
        }
    }

    const content = {
        features: [
            "🎨 AI Style Transfer - Turn photos into artworks.",
            "🌟 AI Colorizer - Colorize black and white photos automatically.",
            "🎬 Basic Editing Tools - Trim, split, merge videos easily.",
            "🎶 Music Library - Access a wide collection of free music & sound effects.",
            "🎤 Voiceover Recording - Record your own voice within the app.",
            "📜 Text & Titles - Add animated text with various fonts and styles.",
            "🔄 Video Transitions - Smooth transitions between video clips.",
            "💬 Auto Captions - Generate subtitles automatically from speech.",
            "🎨 Stickers & Emojis - Add fun stickers, gifs, and emojis.",
            "🗡️ Chroma Key (Green Screen) - Remove backgrounds using green screen tools.",
            "🔍 3D Zoom Pro - Create cinematic 3D zoom effects effortlessly."
        ],
        about: "Aurora is built to redefine creativity with cutting-edge AI tools for enhancing photos and videos effortlessly.",
        contact: "Email us at: support@aurora.io",
        team: "Meet the passionate team of developers, designers, and AI experts behind Aurora.",
        blog: "Stay tuned for exciting updates, tutorials, and tips on maximizing your creativity with Aurora!"
    };

    function renderContent() {
        document.getElementById('features').innerHTML = content.features.map(f => `<div class='feature-card'>${f}</div>`).join('');
        document.getElementById('about').innerHTML = `<div class='section-card'>${content.about}</div>`;
        document.getElementById('contact').innerHTML = `<div class='section-card'>${content.contact}</div>`;
        document.getElementById('team').innerHTML = `<div class='section-card'>${content.team}</div>`;
        document.getElementById('blog').innerHTML = `<div class='section-card'>${content.blog}</div>`;
    }

    renderContent();
</script>

</body>
</html>
