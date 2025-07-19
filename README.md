# Creating a zip file with the index.html content

from zipfile import ZipFile
import os

# Create the index.html content
index_html_content = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aurora - Ultimate Editing Studio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header>
        <h1>🌌 Aurora</h1>
        <nav>
            <a href="#">Home</a>
            <a href="#">Features</a>
            <a href="#">Editor</a>
            <a href="#">Gallery</a>
            <a href="#">Login</a>
        </nav>
    </header>

    <section id="hero">
        <h2>Welcome to Aurora</h2>
        <p>Create stunning videos & photos effortlessly with AI-powered tools.</p>
        <button>Start Editing Now</button>
    </section>

    <section id="features">
        <h2>Our Features</h2>
        <ul>
            <li>8K Ultra HD Export Quality</li>
            <li>Multi-Layer Timeline Editing</li>
            <li>AI Auto-Editing & Smart Tools</li>
            <li>Auto Captions in Multiple Languages</li>
            <li>Voice Command Editing</li>
            <li>AI Mood Filters & Face Tracking</li>
        </ul>
    </section>

    <section id="cta">
        <h2>Join the Aurora Revolution</h2>
        <button>Get Started</button>
    </section>

    <footer>
        <p>&copy; 2025 Aurora. All rights reserved.</p>
    </footer>

</body>
</html>
"""

# Write the content to index.html
with open("index.html", "w") as file:
    file.write(index_html_content)

# Create a zip file
zip_filename = "aurora_website.zip"
with ZipFile(zip_filename, 'w') as zipf:
    zipf.write("index.html")

# Clean up the index.html file after zipping
os.remove("index.html")

# Provide the download link
zip_filename

