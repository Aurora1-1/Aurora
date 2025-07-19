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
            --bg-color: #0b3d91;
            --text-color: #ffffff;
            background-image: url('https://images.unsplash.com/photo-1446776811953-b23d57bd21aa');
            background-size: cover;
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
        .theme-toggle, .astronaut-toggle {
            position: absolute;
            top: 20px;
            right: 20px;
            padding: 10px;
            cursor: pointer;
            background: #fff;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            margin-left: 5px;
        }
        .language-select {
            position: absolute;
            top: 20px;
            left: 20px;
            padding: 10px;
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
<body><button class="theme-toggle" onclick="toggleTheme()">Toggle Light/Dark</button>
<button class="astronaut-toggle" onclick="toggleAstronautTheme()">Astronaut Theme</button>
<select class="language-select" onchange="changeLanguage(this.value)">
    <option value="en">English</option>
    <option value="ur">Urdu</option>
    <option value="fr">French</option>
    <option value="es">Spanish</option>
    <option value="jp">Japanese</option>
    <option value="kr">Korean</option>
    <option value="hi">Hindi</option>
    <option value="pt">Portuguese</option>
    <option value="de">German</option>
</select>

<div class="header">
    <h1 style="font-family: 'Brush Script MT', cursive; font-size: 3rem;">Welcome to Aurora</h1>
    <p>Where Creativity Meets Intelligence. 🚀</p>
</div>

<div class="announcement">
    🎉 Official Launch on <strong>1 February 2025</strong>! Stay tuned! 🎉
</div>

<h2>Explore Our Extensive Features ✨</h2>
<div class="features" id="features"></div>

<div class="logo">A</div>

<footer>
    &copy; 2025 Aurora - All rights reserved.
</footer>

<script>
    const content = {
        en: {
            features: [
                "🎬 Basic Editing Tools - Trim, split, merge videos easily.",
                "🎶 Music Library - Access a wide collection of free music & sound effects.",
                "🎤 Voiceover Recording - Record your own voice within the app.",
                "📜 Text & Titles - Add animated text with various fonts and styles.",
                "🔄 Video Transitions - Smooth transitions between video clips.",
                "💬 Auto Captions - Generate subtitles automatically from speech.",
                "🎨 Stickers & Emojis - Add fun stickers, gifs, and emojis.",
                "🗡️ Chroma Key (Green Screen) - Remove backgrounds using green screen tools.",
                "🔍 3D Zoom Pro - Create cinematic 3D zoom effects effortlessly."
            ]
        }
    };

    function toggleTheme() {
        document.body.classList.toggle('light-theme');
        document.body.classList.remove('astronaut-theme');
    }

    function toggleAstronautTheme() {
        document.body.classList.toggle('astronaut-theme');
        document.body.classList.remove('light-theme');
    }

    function changeLanguage(lang) {
        const data = content[lang] || content['en'];
        document.getElementById('features').innerHTML = data.features.map(f => `<div class='feature-card'>${f}</div>`).join('');
    }

    changeLanguage('en');
</script>

</body>
</html>
