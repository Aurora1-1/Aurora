<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aurora - Ultimate Editing Studio</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&family=Pacifico&family=Monoton&display=swap');

        body {
            margin: 0;
            font-family: 'Orbitron', sans-serif;
            background: radial-gradient(circle at center, #0f0f0f, #000000);
            color: #FFFFFF;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            background: linear-gradient(90deg, #8A2BE2, #00FFFF);
            box-shadow: 0 4px 10px rgba(0,0,0,0.5);
        }
        .logo {
            font-family: 'Pacifico', cursive;
            font-size: 2em;
            color: #FF1493;
            text-shadow: 0 0 10px #FF1493;
        }
        nav a {
            color: #FFFFFF;
            margin: 0 12px;
            text-decoration: none;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #FF1493;
        }
        .hero {
            text-align: center;
            padding: 120px 20px;
            background: linear-gradient(135deg, #8A2BE2, #00FFFF);
            animation: pulse 5s infinite alternate;
        }
        @keyframes pulse {
            from { opacity: 1; }
            to { opacity: 0.8; }
        }
        .hero h1 {
            font-size: 4em;
            margin-bottom: 15px;
            text-shadow: 0 0 20px #00FFFF;
        }
        .hero p.tagline {
            font-size: 1.8em;
            font-style: italic;
            color: #FFD700;
            margin-bottom: 20px;
        }
        .hero p.release-date {
            font-family: 'Monoton', cursive;
            font-size: 1.6em;
            color: #FF69B4;
            text-shadow: 0 0 10px #FF69B4;
        }
        section {
            padding: 60px 20px;
            border-bottom: 1px solid #333;
        }
        h2 {
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.5em;
            text-shadow: 0 0 10px #8A2BE2;
        }
        ul {
            max-width: 600px;
            margin: 0 auto;
            list-style: none;
            padding: 0;
        }
        ul li {
            margin-bottom: 15px;
            background: #111;
            padding: 10px;
            border-left: 5px solid #8A2BE2;
            border-radius: 5px;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #111111;
            border-top: 1px solid #8A2BE2;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">🚀 Aurora</div>
        <nav>
            <a href="#home">Home</a>
            <a href="#features">Features</a>
            <a href="#editor">Editor</a>
            <a href="#gallery">Gallery</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1>Welcome to Aurora</h1>
        <p class="tagline">Where Creativity Meets Intelligence</p>
        <p>Revolutionizing Editing with AI & Neon Vibes</p>
        <p class="release-date">🚀 Official Release Date: 1 Feb 2026 🚀</p>
    </section>

    <section id="features">
        <h2>✨ Features</h2>
        <ul>
            <li>8K Ultra HD Export</li>
            <li>AI Auto-Editing & Smart Tools</li>
            <li>Voice Command Editing</li>
            <li>Multi-Layer Timeline</li>
            <li>Auto Captions</li>
            <li>Mood Filters & Face Tracking</li>
        </ul>
    </section>

    <section id="gallery">
        <h2>📸 Gallery</h2>
        <p style="text-align:center;">Explore creations by our vibrant community!</p>
    </section>

    <section id="about">
        <h2>👩‍🚀 About Us</h2>
        <p style="max-width:600px; margin:auto; text-align:center;">
            Aurora is redefining creativity with AI-driven video and photo editing tools, wrapped in a stunning futuristic experience.
        </p>
    </section>

    <section id="contact">
        <h2>📬 Contact Us</h2>
        <p style="text-align:center;">Reach out at: <a href="mailto:support@aurora.com" style="color:#00FFFF;">support@aurora.com</a></p>
    </section>

    <footer>
        <p>&copy; 2025 Aurora. All rights reserved.</p>
    </footer>
</body>
</html>
