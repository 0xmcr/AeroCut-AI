# 🎬 AeroCut AI — Wiki

Welcome to the official **AeroCut AI by MCR** documentation wiki.

## 📚 Table of Contents

- [Overview](#overview)
- [Installation Guide](#installation-guide)
- [API Key Setup](#api-key-setup)
- [Pipeline Templates](#pipeline-templates)
- [Web Dashboard Guide](#web-dashboard-guide)
- [FAQ](#faq)

---

## Overview

AeroCut AI is a fully self-hosted, AI-orchestrated video production studio. It automates the entire video creation pipeline — from research and scripting to voiceover, image generation, captioning, and final video rendering — with **zero manual editing required**.

**Core Technologies:**

| Layer | Technology |
|:---|:---|
| **Backend** | FastAPI (Python 3) |
| **Frontend** | React + TypeScript + Vite |
| **Video Rendering** | Remotion (headless Chromium) |
| **Text / Script AI** | OpenAI GPT-4o, Google Gemini, xAI |
| **Voice / TTS** | ElevenLabs, Piper-TTS, Doubao Speech |
| **Image / Video AI** | fal.ai (Kling v3, Flux), Google Imagen, Runway Gen-3 |

---

## Installation Guide

### 🇺🇸 English

#### Prerequisites

| Tool | Version | Install |
|:---|:---|:---|
| Python | 3.10+ | [python.org](https://python.org) |
| Node.js | 18+ | [nodejs.org](https://nodejs.org) |
| FFmpeg | Latest | `brew install ffmpeg` / `apt install ffmpeg` |

#### Setup

```bash
git clone https://github.com/0xmcr/AeroCut-AI.git
cd AeroCut-AI

# Create virtual environment
python3 -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
cd web-ui && npm install && cd ..

# Configure environment
cp .env.example .env

# Start the server
python3 server/main.py
```

Open **http://localhost:8000** in your browser.

---

### 🇧🇩 বাংলা — ইন্সটলেশন গাইড

#### প্রয়োজনীয় সফটওয়্যার

| টুল | ভার্সন | ইন্সটল |
|:---|:---|:---|
| Python | 3.10+ | [python.org](https://python.org) |
| Node.js | 18+ | [nodejs.org](https://nodejs.org) |
| FFmpeg | Latest | `brew install ffmpeg` / `apt install ffmpeg` |

#### সেটআপ

```bash
git clone https://github.com/0xmcr/AeroCut-AI.git
cd AeroCut-AI

# ভার্চুয়াল এনভায়রনমেন্ট তৈরি করুন
python3 -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate

# ডিপেন্ডেন্সি ইন্সটল করুন
pip install -r requirements.txt
cd web-ui && npm install && cd ..

# এনভায়রনমেন্ট কনফিগার করুন
cp .env.example .env

# সার্ভার চালু করুন
python3 server/main.py
```

ব্রাউজারে যান: **http://localhost:8000**

> Keys ট্যাবে গিয়ে আপনার AI API কী গুলো সেট করুন। প্রতিটি কীয়ের পাশে "কী নিন ↗" লিঙ্ক থেকে সরাসরি প্রোভাইডারের সাইটে যেতে পারবেন।

---

### 🇪🇸 Español — Guía de Instalación

#### Requisitos previos

| Herramienta | Versión | Instalar |
|:---|:---|:---|
| Python | 3.10+ | [python.org](https://python.org) |
| Node.js | 18+ | [nodejs.org](https://nodejs.org) |
| FFmpeg | Latest | `brew install ffmpeg` / `apt install ffmpeg` |

#### Configuración

```bash
git clone https://github.com/0xmcr/AeroCut-AI.git
cd AeroCut-AI

# Crear entorno virtual
python3 -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate

# Instalar dependencias
pip install -r requirements.txt
cd web-ui && npm install && cd ..

# Configurar variables de entorno
cp .env.example .env

# Iniciar el servidor
python3 server/main.py
```

Abre tu navegador en **http://localhost:8000**

---

### 🇮🇳 हिंदी — इंस्टॉलेशन गाइड

#### आवश्यकताएं

| टूल | संस्करण | इंस्टॉल |
|:---|:---|:---|
| Python | 3.10+ | [python.org](https://python.org) |
| Node.js | 18+ | [nodejs.org](https://nodejs.org) |
| FFmpeg | Latest | `brew install ffmpeg` / `apt install ffmpeg` |

#### सेटअप

```bash
git clone https://github.com/0xmcr/AeroCut-AI.git
cd AeroCut-AI

# वर्चुअल एनवायरनमेंट बनाएं
python3 -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate

# डिपेंडेंसीज़ इंस्टॉल करें
pip install -r requirements.txt
cd web-ui && npm install && cd ..

# एनवायरनमेंट कॉन्फ़िगर करें
cp .env.example .env

# सर्वर शुरू करें
python3 server/main.py
```

ब्राउज़र में खोलें: **http://localhost:8000**

---

## API Key Setup

Go to the **Keys tab** in the Web Dashboard to configure your AI provider keys. Each key has a direct **"Get Key ↗"** link to the provider's official developer console.

| Environment Variable | Provider | Purpose | Get Key |
|:---|:---|:---|:---|
| `OPENAI_API_KEY` | OpenAI | Script writing, image generation | [platform.openai.com](https://platform.openai.com/api-keys) |
| `FAL_KEY` | fal.ai | Video generation (Kling v3, Flux) | [fal.ai/dashboard](https://fal.ai/dashboard) |
| `ELEVENLABS_API_KEY` | ElevenLabs | Realistic voice/TTS | [elevenlabs.io](https://elevenlabs.io) |
| `GOOGLE_API_KEY` | Google AI Studio | Gemini + Imagen + TTS | [aistudio.google.com](https://aistudio.google.com) |
| `RUNWAY_API_KEY` | Runway | Video generation Gen-3 | [runwayml.com](https://runwayml.com) |
| `SUNO_API_KEY` | Suno | AI music generation | [suno.ai](https://suno.ai) |
| `PEXELS_API_KEY` | Pexels | Free stock footage | [pexels.com/api](https://www.pexels.com/api/) |
| `PIXABAY_API_KEY` | Pixabay | Free images & music | [pixabay.com/api](https://pixabay.com/api/docs/) |
| `HEYGEN_API_KEY` | HeyGen | Avatar spokesperson videos | [heygen.com](https://heygen.com) |
| `XAI_API_KEY` | xAI (Grok) | Script writing, image generation | [x.ai](https://x.ai) |

> **Tip:** You can start with just `OPENAI_API_KEY` — the system will automatically use only available tools.

---

## Pipeline Templates

AeroCut AI includes **13 production-grade video pipeline templates**, all at `production` stability:

| Template | Category | Best For |
|:---|:---|:---|
| `cinematic` | Cinematic | Movie trailers, dramatic storytelling |
| `animation` | Animation | Animated explainers, full animation |
| `animated-explainer` | Animation | Educational content |
| `screen-demo` | Demo | App/SaaS product demos |
| `avatar-spokesperson` | Avatar | AI spokesperson/presenter |
| `talking-head` | Talking Head | Interview, commentary videos |
| `documentary` | Cinematic | Documentary-style stock footage edits |
| `podcast-repurpose` | Custom | Turn podcasts into video content |
| `clip-factory` | Custom | Extract short clips from long content |
| `localization-dub` | Custom | Translate and dub existing videos |
| `character-animation` | Animation | SVG/Canvas local character animations |
| `hybrid` | Custom | Mix of real footage + generated assets |
| `framework-smoke` | Custom | Minimal test/validation pipeline |

---

## Web Dashboard Guide

### 📁 Projects Tab
- View all your video production projects
- See current pipeline **stage** and **status** at a glance
- Click any project card to open its full workspace
- Click 🗑️ to **permanently delete** a project from your device

### ➕ New Tab
- Enter a **Project Name** (kebab-case, e.g. `my-science-video`)
- Select a **Pipeline Template**
- Write your **Topic / Prompt** in plain language
- Click **Initialize Project** to begin

### 🔑 Keys Tab
- Configure all AI provider API keys from the browser
- Each key shows **Configured ✅** or **Missing ❌** badge
- Click **Get Key ↗** to jump directly to the provider's site
- Click **Update API Keys** to save changes

### 🖥️ Workspace View (when a project is selected)
- **Run Next Stage** — Advances the pipeline step (research → script → assets → render)
- **Export ZIP** — Downloads all project files and assets as a ZIP archive
- **Download Video (MP4)** — Downloads the final rendered video
- **Execution Console** — Real-time AI pipeline log output
- **Active System Capabilities** — Click any numbered badge to see which AI tools are active for each capability

---

## FAQ

**Q: Do I need all API keys to get started?**
> No. You can start with just `OPENAI_API_KEY` or `GOOGLE_API_KEY`. The system selects tools based on what is configured.

**Q: Where are my projects stored?**
> Locally in the `projects/` folder inside the AeroCut AI directory on your device. You can delete them from the dashboard UI.

**Q: Can I run this without internet?**
> Partially — FFmpeg, Piper TTS (local voice), and Remotion work offline. Cloud AI providers (OpenAI, ElevenLabs, etc.) require internet.

**Q: How do I update the app?**
> ```bash
> git pull origin main
> pip install -r requirements.txt
> cd web-ui && npm install && npm run build && cd ..
> python3 server/main.py
> ```

**Q: The server won't start — what do I do?**
> Make sure you have activated your virtual environment (`source venv/bin/activate`) and that FFmpeg is installed (`ffmpeg -version`).

**Q: Can I use this on Windows?**
> Yes, via WSL2 (Windows Subsystem for Linux). Native Windows support is in progress.

---

*AeroCut AI by MCR — Built for creators who want real video, not slideshow tricks.*
