<div align="center">

# 🧠⚡ **AI Doctor System — Environment Setup Guide**  
A complete cross-platform setup for running the **4-phase AI medical assistant system**, including audio processing, speech interfaces, and Gradio UI.

---

### 🛠 Technologies Included
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-Audio/Video-green?style=for-the-badge&logo=ffmpeg)
![PortAudio](https://img.shields.io/badge/PortAudio-Sound-blue?style=for-the-badge)
![pipenv](https://img.shields.io/badge/pipenv-Environment-yellow?style=for-the-badge)
![Conda](https://img.shields.io/badge/conda-Environment-blue?style=for-the-badge)
![Gradio](https://img.shields.io/badge/Gradio-Web_UI-orange?style=for-the-badge)

---

</div>

# 📚 **Table of Contents**
1. 🛠 [Installing FFmpeg & PortAudio](#installing-ffmpeg-and-portaudio)  
2. 🐍 [Setting Up Python Environment](#setting-up-a-python-virtual-environment)  
3. 🧪 [Running Each Project Phase](#running-the-application)  
4. 🚀 [Launch Gradio App](#launch-gradio-ui)

---

# 🛠 **Installing FFmpeg and PortAudio**

## 🍎 **macOS**

### 1️⃣ Install Homebrew  
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 2️⃣ Install FFmpeg + PortAudio  
```bash
brew install ffmpeg portaudio
```

---

## 🐧 **Linux (Ubuntu / Debian)**

### 1️⃣ Update  
```bash
sudo apt update
```

### 2️⃣ Install FFmpeg + PortAudio  
```bash
sudo apt install ffmpeg portaudio19-dev
```

---

## 🪟 **Windows**

### ▶ Install FFmpeg  
Download from:  
https://ffmpeg.org/download.html

1. Choose **Windows static build**  
2. Extract to: `C:\ffmpeg`  
3. Add to PATH:  
   ```
   C:\ffmpeg\bin
   ```
   Steps:  
   - Search **Environment Variables**  
   - Edit **PATH** → Add new → paste the path  
   - Save

### ▶ Install PortAudio  
Download from:  
http://www.portaudio.com/download.html

Install using provided Windows instructions.

---

# 🐍 **Setting Up a Python Virtual Environment**

## 📦 **Using Pipenv (recommended)**

### 1️⃣ Install Pipenv  
```bash
pip install pipenv
```

### 2️⃣ Install Dependencies  
```bash
pipenv install
```

### 3️⃣ Activate  
```bash
pipenv shell
```

---

## 🔧 **Using pip + venv**

### 1️⃣ Create Environment  
```bash
python -m venv venv
```

### 2️⃣ Activate  

macOS/Linux:
```bash
source venv/bin/activate
```

Windows:
```bash
venv\Scripts\activate
```

### 3️⃣ Install Requirements  
```bash
pip install -r requirements.txt
```

---

## 🌱 **Using Conda**

### 1️⃣ Create Conda Environment  
```bash
conda create --name myenv python=3.11
```

### 2️⃣ Activate  
```bash
conda activate myenv
```

### 3️⃣ Install Requirements  
```bash
pip install -r requirements.txt
```

---

# 🏃 **Project Phases and Python Commands**

Below are the **four phases** of the AI Doctor workflow.

---

## 🧠 **Phase 1 — Brain of the Doctor**

Runs the core reasoning logic.

```bash
python brain_of_the_doctor.py
```

---

## 🗣️ **Phase 2 — Voice of the Patient**

Captures and processes patient-side audio.

```bash
python voice_of_the_patient.py
```

---

## 👨‍⚕️ **Phase 3 — Voice of the Doctor**

Generates doctor-side voice outputs.

```bash
python voice_of_the_doctor.py
```

---

## 💻 **Phase 4 — Launch Gradio UI**

Starts the web interface.

```bash
python gradio_app.py
```

---

<div align="center">

# 🎉 **Setup Complete!**  
You're now ready to run the full AI Doctor System across all platforms.

</div>
