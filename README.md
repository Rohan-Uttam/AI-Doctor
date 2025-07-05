# 🚀 Project Setup Guide

This guide provides step-by-step instructions to set up your project environment, including installation of FFmpeg and PortAudio across macOS, Linux, and Windows, as well as setting up a Python virtual environment using Pipenv, pip, or conda.

---

## 📚 Table of Contents

1. [🛠 Installing FFmpeg and PortAudio](#installing-ffmpeg-and-portaudio)
   - [🍎 macOS](#macos)
   - [🐧 Linux](#linux)
   - [🪟 Windows](#windows)
2. [🐍 Setting Up a Python Virtual Environment](#setting-up-a-python-virtual-environment)
   - [📦 Using Pipenv](#using-pipenv)
   - [🔧 Using pip and venv](#using-pip-and-venv)
   - [🌱 Using Conda](#using-conda)
3. [🏃 Running the Application](#project-phases-and-python-commands)

---

## 🛠 Installing FFmpeg and PortAudio

### 🍎 macOS

1. **Install Homebrew (if not already installed):**

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install FFmpeg and PortAudio:**

   ```bash
   brew install ffmpeg portaudio
   ```

---

### 🐧 Linux (Debian/Ubuntu)

1. **Update Package List:**

   ```bash
   sudo apt update
   ```

2. **Install FFmpeg and PortAudio:**

   ```bash
   sudo apt install ffmpeg portaudio19-dev
   ```

---

### 🪟 Windows

#### 📥 Download FFmpeg:

1. Visit: https://ffmpeg.org/download.html  
2. Go to the Windows builds section and download the latest **static build**

#### 🗂 Extract & Set Up FFmpeg:

1. Extract the ZIP to a folder (e.g., `C:\ffmpeg`)
2. Add `C:\ffmpeg\bin` to your **System PATH**:
   - Open Start → search "Environment Variables"
   - Click "Edit the system environment variables"
   - In System Properties → "Environment Variables"
   - Under System variables → Edit the **Path**
   - Click **New** → add: `C:\ffmpeg\bin`
   - Click **OK**

#### 🎙 Install PortAudio:

1. Download binaries: http://www.portaudio.com/download.html  
2. Follow Windows installation instructions from the site

---

## 🐍 Setting Up a Python Virtual Environment

### 📦 Using Pipenv

1. **Install Pipenv:**

   ```bash
   pip install pipenv
   ```

2. **Install Dependencies:**

   ```bash
   pipenv install
   ```

3. **Activate Environment:**

   ```bash
   pipenv shell
   ```

---

### 🔧 Using `pip` and `venv`

1. **Create Virtual Environment:**

   ```bash
   python -m venv venv
   ```

2. **Activate Environment:**

   - macOS/Linux:

     ```bash
     source venv/bin/activate
     ```

   - Windows:

     ```bash
     venv\Scripts\activate
     ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

---

### 🌱 Using Conda

1. **Create Conda Environment:**

   ```bash
   conda create --name myenv python=3.11
   ```

2. **Activate Conda Environment:**

   ```bash
   conda activate myenv
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

---

## 🏃 Project Phases and Python Commands

### Phase 1: 🧠 Brain of the Doctor

```bash
python brain_of_the_doctor.py
```

---

### Phase 2: 🗣️ Voice of the Patient

```bash
python voice_of_the_patient.py
```

---

### Phase 3: 👨‍⚕️ Voice of the Doctor

```bash
python voice_of_the_doctor.py
```

---

### Phase 4: 💻 Launch Gradio UI

```bash
python gradio_app.py
```

---
