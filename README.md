# 🛡️ Safe Surf AI

**Safe Surf AI** is a browser-based web safety tool designed to detect and prevent access to malicious, phishing, and suspicious URLs using AI models and multi-layered threat analysis techniques.

---

## 🔍 Features

- 🔗 Real-time URL scanning and threat evaluation
- 🤖 AI-powered classification (phishing, suspicious, safe)
- 🔍 Detection of shortened URLs and homographs
- 🧠 Integration with VirusTotal for multi-engine checks
- 🌐 Chrome Extension for seamless browsing protection
- 🎨 Modern animated UI with login and registration options

---

## 🧱 Tech Stack

| Layer        | Technology                        |
|--------------|------------------------------------|
| Frontend     | HTML, CSS, JavaScript (Popup UI)   |
| Extension    | Chrome Manifest V3, JS APIs        |
| Backend      | Django, FastAPI (for some modules) |
| AI Modules   | Python (sklearn, transformers, etc.)|
| Automation   | Selenium for live page capture     |
| External APIs| VirusTotal                         |

---

## 🚀 Getting Started

### 📦 Prerequisites

- Python 3.8+
- Node.js (optional, for advanced frontend dev)
- Chrome browser
- Git

### 🔧 Installation

```bash
git clone https://github.com/prathamesh-chavan-22/Safe_surf_ai.git
cd Safe_surf_ai

### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate     # or venv\Scripts\activate on Windows
pip install -r requirements.txt
python manage.py runserver

### 🧩 Chrome Extension Setup

1. Open `chrome://extensions` in Chrome  
2. Enable **Developer mode**  
3. Click **Load Unpacked**  
4. Select the `extension/` folder from this repo  

---

### 🌐 How It Works

1. User clicks the Chrome Extension icon  
2. The current tab’s URL is extracted and checked:
   - 🔗 Is it shortened?  
   - 🧿 Is it a homograph?  
   - 🧪 Does it appear malicious via VirusTotal?  
   - 🤖 What does the custom AI model say?  
3. ✅ Results are shown in an animated popup with safety status
