🌐 Browser Use Web UI







🚀 Overview

Browser Use Web UI is an AI-powered browser interaction tool built on Gradio. It extends the functionality of browser-use, allowing users to control browsers with AI agents.

🔹 Features

Supports AI Agents for automated browser tasks.

Integration with LLMs (Google, OpenAI, Azure, Anthropic, etc.).

Persistent Browser Sessions for enhanced user experience.

VNC Support for real-time browser monitoring.

Custom Browser Support to use existing browser logins.

Streamlit-based UI for seamless interaction.

📥 Installation Guide

🔧 Prerequisites

Python 3.11+

Git

Docker (optional for containerized deployment)

🏠 Local Installation

1️⃣ Clone the Repository

git clone https://github.com/browser-use/web-ui.git
cd web-ui

2️⃣ Set Up Python Environment

python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate    # Windows

3️⃣ Install Dependencies

pip install -r requirements.txt

4️⃣ Start the Web UI

python webui.py --ip 127.0.0.1 --port 7788

🐳 Docker Installation

1️⃣ Clone Repository & Setup Environment

git clone https://github.com/browser-use/web-ui.git
cd web-ui
cp .env.example .env

Edit .env with API keys and required settings.

2️⃣ Build & Run Container

docker compose up --build

For persistent browser sessions:

CHROME_PERSISTENT_SESSION=true docker compose up --build

3️⃣ Access the Web UI

Web Interface: http://localhost:7788

VNC Viewer: http://localhost:6080/vnc.html (Password: "vncpassword")

🔧 Configuration

Modify environment variables in .env file:

CHROME_PERSISTENT_SESSION=true  # Keep browser open
RESOLUTION=1920x1080x24         # Browser resolution
VNC_PASSWORD=your_password      # VNC authentication

📜 License

This project is licensed under the MIT License.

