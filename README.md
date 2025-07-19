<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aurora - AI Photo & Video Enhancer</title>
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
        .header {
            padding: 20px;
            background-color: rgba(0,0,0,0.6);
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
<body>

    <button class="theme-toggle" onclick="toggleTheme()">Toggle Theme</button>

    <div class="header">
        <h1 style="font-family: 'Brush Script MT', cursive; font-size: 3rem;">Aurora</h1>
        <p>Where Creativity Meets Intelligence. 🚀</p>
    </div>

    <h2>Explore Our Extensive Features ✨</h2>
    <div class="features">
        <div class="feature-card"><h3>🎨 AI Style Transfer</h3><p>Turn photos into artworks like Van Gogh or Ghibli.</p></div>
        <div class="feature-card"><h3>🌌 Ghibli Image Generator</h3><p>Create dreamy Ghibli-inspired images using AI.</p></div>
        <div class="feature-card"><h3>📚 Scholarly Note Scanner</h3><p>Scan handwritten notes & convert them to digital text.</p></div>
        <div class="feature-card"><h3>📊 AI Presentation Maker</h3><p>Create aesthetic slides & presentations instantly with AI.</p></div>
        <div class="feature-card"><h3>🎭 AI Face Morphing</h3><p>Transform faces with AI morphing technology for fun & creativity.</p></div>
        <div class="feature-card"><h3>🌟 AI Colorizer</h3><p>Colorize black and white photos automatically.</p></div>
    </div>

    <h2>About Us</h2>
    <div class="section">
        <div class="section-card"><p>Aurora is built to redefine creativity with cutting-edge AI tools for enhancing photos and videos effortlessly.</p></div>
    </div>

    <h2>Contact</h2>
    <div class="section">
        <div class="section-card"><p>Email us at: support@aurora.io</p></div>
    </div>

    <h2>Team</h2>
    <div class="section">
        <div class="section-card"><p>Meet the passionate team of developers, designers, and AI experts behind Aurora.</p></div>
    </div>

    <h2>Blog / Updates</h2>
    <div class="section">
        <div class="section-card"><p>Stay tuned for exciting updates, tutorials, and tips on maximizing your creativity with Aurora!</p></div>
    </div>

    <div class="logo">Aurora</div>

    <footer>
        &copy; 2025 Aurora - All rights reserved.
    </footer>

    <script>
        function toggleTheme() {
            document.body.classList.toggle('light-theme');
        }
    </script>

</body>
</html>
