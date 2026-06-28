# AeroCut AI by MCR

AeroCut AI by MCR is a production-grade, automated, AI-orchestrated video production studio with an interactive Web UI. It automates the entire pipeline of video creation: research, scriptwriting, voiceover generation, visual asset creation, caption formatting, video compilation, and final rendering.

## 🌍 Language Guides / ভাষা নির্দেশিকা / Guías de Idiomas / भाषा निर्देशिका

*   [English Installation Guide](#-english-installation-guide)
*   [বাংলা ইন্সটলেশন নির্দেশিকা (Bengali Guide)](#-বাংলা-ইন্সটলেশন-নির্দেশিকা-bengali-guide)
*   [Guía de Instalación en Español (Spanish Guide)](#-guía-de-instalación-en-español-spanish-guide)
*   [हिंदी इंस्टॉलेशन निर्देशिका (Hindi Guide)](#-हिंदी-इंस्टॉलेशन-निर्देशिका-hindi-guide)

---

## 🇺🇸 English Installation Guide

### 🚀 Key Features
*   **Interactive Web-UI:** Manage projects, templates, API keys, and monitor pipeline progress in real-time.
*   **Multi-Language Interface:** Built-in support for English, Bengali, Spanish, and Hindi.
*   **Active AI Capabilities:** Monitor configured AI engines (OpenAI, Gemini, ElevenLabs, etc.).
*   **Dynamic ZIP Export:** Export all scripts, voiceovers, visual assets, and videos in a single ZIP file at any stage.

### 💻 System Requirements
*   **OS:** macOS 12+, Linux (Ubuntu/Debian), or Windows 10+ (via WSL2).
*   **CPU:** Quad-core or higher recommended (Apple Silicon M-series preferred).
*   **RAM:** 8 GB minimum (16 GB recommended).
*   **Disk Space:** 5 GB+ free space.
*   **Dependencies:** Python 3.10+, Node.js 18+, and **FFmpeg**.

### ⚙️ Step-by-Step Installation
1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/0xmcr/AeroCut-AI.git
    cd AeroCut-AI
    ```
2.  **Set Up Virtual Environment & Python Packages:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # Windows: venv\Scripts\activate
    pip install -r requirements.txt
    ```
3.  **Install Frontend Packages:**
    ```bash
    cd web-ui
    npm install
    cd ..
    ```
4.  **Configure Environment Variables:**
    ```bash
    cp .env.example .env
    ```
    *(Open `.env` and enter your API keys, or configure them later using the Keys tab in the Web UI).*
5.  **Run the Server:**
    ```bash
    python3 server/main.py
    ```
    Open `http://localhost:8000` in your web browser.

---

## 🇧🇩 বাংলা ইন্সটলেশন নির্দেশিকা (Bengali Guide)

### 🚀 মূল সুবিধাসমূহ
*   **ইন্টারেক্টিভ ওয়েব ইউআই:** প্রজেক্ট এবং এপিআই কী রিয়েল-টাইমে ম্যানেজ করুন।
*   **বহুভাষিক সাপোর্ট:** ইংরেজি, বাংলা, স্প্যানিশ এবং হিন্দি ভাষার সাপোর্ট।
*   **সহজ এক্সপোর্ট:** এক ক্লিকে পুরো প্রজেক্টের সমস্ত এসেট ও ভিডিও জিপ (ZIP) আকারে ডাউনলোড করুন।

### 💻 হার্ডওয়্যার প্রয়োজনীয়তা
*   **অপারেটিং সিস্টেম:** macOS 12+, Linux (Ubuntu/Debian), অথবা Windows 10+ (WSL2)।
*   **র্যাম (RAM):** ন্যূনতম ৮ জিবি (১৬ জিবি রেকমেন্ডেড)।
*   **প্রয়োজনীয় ইউটিলিটি:** Python 3.10+, Node.js 18+, এবং **FFmpeg**।

### ⚙️ ইন্সটলেশন নির্দেশাবলী
১.  **রিপজিটরি ক্লোন করুন:**
    ```bash
    git clone https://github.com/0xmcr/AeroCut-AI.git
    cd AeroCut-AI
    ```
২.  **ভার্চুয়াল এনভায়রনমেন্ট ও ডিপেন্ডেন্সি সেটআপ:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # উইন্ডোজের জন্য: venv\Scripts\activate
    pip install -r requirements.txt
    ```
৩.  **ফ্রন্টএন্ড প্যাকেজ ইন্সটল করুন:**
    ```bash
    cd web-ui
    npm install
    cd ..
    ```
৪.  **এনভায়রনমেন্ট ফাইল কনফিগার করুন:**
    ```bash
    cp .env.example .env
    ```
    *(ফাইলটি ওপেন করে আপনার এআই এপিআই কী-গুলো বসিয়ে দিন অথবা সরাসরি ওয়েব ড্যাশবোর্ডের Keys ট্যাব থেকেও কনফিগার করতে পারেন)।*
৫.  **সার্ভার চালু করুন:**
    ```bash
    python3 server/main.py
    ```
    আপনার ব্রাউজারে `http://localhost:8000` লিঙ্কটি ওপেন করুন।

---

## 🇪🇸 Guía de Instalación en Español (Spanish Guide)

### 🚀 Características Clave
*   **Interfaz de Usuario Web:** Gestione proyectos y claves API en tiempo real.
*   **Soporte Multilingüe:** Soporte nativo para inglés, bengalí, español e hindi.
*   **Exportación ZIP Dinámica:** Descargue todos los archivos del proyecto (scripts, voces, imágenes y video final) en un solo archivo ZIP.

### 💻 Requisitos del Sistema
*   **SO:** macOS 12+, Linux (Ubuntu/Debian), o Windows 10+ (vía WSL2).
*   **RAM:** Mínimo 8 GB (16 GB recomendado).
*   **Dependencias:** Python 3.10+, Node.js 18+, y **FFmpeg**.

### ⚙️ Instalación Paso a Paso
1.  **Clonar el Repositorio:**
    ```bash
    git clone https://github.com/0xmcr/AeroCut-AI.git
    cd AeroCut-AI
    ```
2.  **Configurar Entorno Virtual y Dependencias de Python:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # En Windows: venv\Scripts\activate
    pip install -r requirements.txt
    ```
3.  **Instalar Paquetes del Frontend:**
    ```bash
    cd web-ui
    npm install
    cd ..
    ```
4.  **Configurar Variables de Entorno:**
    ```bash
    cp .env.example .env
    ```
    *(Abra `.env` e introduzca sus claves API, o configúrelas en la pestaña Keys del panel de control web).*
5.  **Iniciar el Servidor:**
    ```bash
    python3 server/main.py
    ```
    Abra `http://localhost:8000` en su navegador web.

---

## 🇮🇳 हिंदी इंस्टॉलेशन निर्देशिका (Hindi Guide)

### 🚀 मुख्य विशेषताएं
*   **वेब यूजर इंटरफेस (Web UI):** रियल-टाइम में प्रोजेक्ट्स और एपीआई (API) कीज को प्रबंधित करें।
*   **बहुभाषी सपोर्ट:** अंग्रेजी, बंगाली, स्पेनिश और हिंदी के लिए इन-बिल्ट सपोर्ट।
*   **आसान एक्सपोर्ट:** सभी जनरेटेड एसेट्स और वीडियो को एक क्लिक में ज़िप (ZIP) फाइल में डाउनलोड करें।

### 💻 सिस्टम आवश्यकताएँ
*   **ऑपरेटिंग सिस्टम:** macOS 12+, Linux (Ubuntu/Debian), या Windows 10+ (WSL2 के माध्यम से)।
*   **रैम (RAM):** न्यूनतम 8 जीबी (16 जीबी अनुशंसित)।
*   **सॉफ्टवेयर आवश्यकताएँ:** Python 3.10+, Node.js 18+, और **FFmpeg**।

### ⚙️ चरण-दर-चरण इंस्टॉलेशन
1.  **रिपॉजिटरी क्लोन करें:**
    ```bash
    git clone https://github.com/0xmcr/AeroCut-AI.git
    cd AeroCut-AI
    ```
2.  **वर्चुअल एनवायरनमेंट और पायथन पैकेज सेटअप:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # विंडोज के लिए: venv\Scripts\activate
    pip install -r requirements.txt
    ```
3.  **फ्रंटएंड पैकेज इंस्टॉल करें:**
    ```bash
    cd web-ui
    npm install
    cd ..
    ```
4.  **एनवायरनमेंट वेरिएबल कॉन्फ़िगर करें:**
    ```bash
    cp .env.example .env
    ```
    *(फाइल खोलकर अपनी एपीआई कीज दर्ज करें, या बाद में वेब डैशबोर्ड पर Keys टैब से कॉन्फ़िगर करें)।*
5.  **सर्वर शुरू करें:**
    ```bash
    python3 server/main.py
    ```
    अपने वेब ब्राउज़र में `http://localhost:8000` खोलें।
