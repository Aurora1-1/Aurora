# Creating a README.md file with the same content as index.html in markdown-friendly format

readme_content = """
# Aurora - Ultimate Editing Studio

Welcome to **Aurora** — Your Ultimate Video & Photo Editor!

## 🌟 Features

- **8K Ultra HD Export Quality**
- **Multi-Layer Timeline Editing**
- **AI Auto-Editing & Smart Tools**
- **Auto Captions in Multiple Languages**
- **Voice Command Editing**
- **AI Mood Filters & Face Tracking**

## 🚀 Quick Start

1. Clone or download this repository.
2. Open the `index.html` file in your browser.
3. Start exploring the Aurora editing experience!

## 🔗 Navigation

- Home
- Features
- Editor
- Gallery
- Login

## 📣 Call to Action

> **Join the Aurora Revolution!**  
> Start Editing Now and create stunning videos & photos effortlessly with AI-powered tools.

## 🧩 About

© 2025 Aurora. All rights reserved.
"""

# Write the README.md file
readme_filename = "/mnt/data/README.md"
with open(readme_filename, "w") as readme_file:
    readme_file.write(readme_content)

readme_filename


