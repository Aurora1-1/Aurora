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

<h2>Explore Our Features ✨</h2>
<div class="features">
    <div class="feature-card">🎬 Basic Editing Tools - Trim, split, merge videos easily.</div>
    <div class="feature-card">🎶 Music Library - Access a wide collection of free music & sound effects.</div>
</div>

<div class="logo">A</div>

<footer>
    &copy; 2026 Aurora - All rights reserved.
</footer>

<script>
    function toggleTheme() {
        document.body.classList.toggle('light-theme');
    }
</script>

</body>
</html>
