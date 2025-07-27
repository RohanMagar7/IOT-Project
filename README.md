
# 🎙️ Offline AI Voice-Controlled Assistant

An offline, privacy-first, AI-powered voice assistant built using Python. It runs entirely on local hardware (e.g., Raspberry Pi 5), with no internet required. Designed for voice-controlled tasks like opening apps, setting reminders, telling the time, and more.

---

## 🔧 Features

- 🧠 **Fully Offline AI Core** — No internet, no cloud, all processing on-device
- 🎤 **Voice Activation** — Trigger using a hotword or manual start
- 🗣️ **Speech-to-Text (STT)** — Converts your voice commands to text locally
- 🧾 **Command Understanding** — Rule-based or NLP-based intent recognition
- 🗨️ **Text-to-Speech (TTS)** — Speaks responses using local TTS engines
- ⚙️ **Custom Actions** — Easily programmable to control apps, GPIO, or local services
- 💻 **Platform** — Optimized for Raspberry Pi 5 (but runs on any Linux system)

---

## 🛠️ Tech Stack

| Component        | Technology           |
|------------------|----------------------|
| Programming Lang | Python 3.10+          |
| STT              | Vosk / Whisper.cpp   |
| TTS              | Piper / eSpeak NG    |
| Hotword Detect   | Porcupine / Snowboy  |
| Intent Parsing   | Rasa NLU / Rule-Based |
| OS               | Raspberry Pi OS / Ubuntu |
| UI (optional)    | CLI / Tkinter GUI    |

---

## 🚀 Getting Started

### ✅ Prerequisites

- Python 3.10+
- Git
- Pip
- Microphone and speaker setup
- (For Pi): Raspberry Pi 5 with audio drivers installed

### 📥 Installation

```bash
git clone https://github.com/yourusername/offline-voice-assistant.git
cd offline-voice-assistant
pip install -r requirements.txt
```

### 🔁 Run the Assistant

```bash
python main.py
```

### 📢 Activate with voice or press Enter to start listening.

---

## 📂 Project Structure

```
offline-voice-assistant/
├── main.py                # Entry point
├── stt/                   # Speech-to-text modules
├── tts/                   # Text-to-speech modules
├── intents/               # Command and NLP logic
├── config/                # Configuration files
├── actions/               # Customizable task scripts
└── README.md
```

---

## 🧠 Supported Commands (Examples)

- “What’s the time?”
- “Open browser”
- “Turn off the light” *(if connected to GPIO)*
- “Remind me in 10 minutes”
- “What’s today’s date?”

---

## 🔌 Optional Hardware Integration

Supports Raspberry Pi GPIO for smart home control:

- Light switch
- Fan toggle
- Sensor reading

```python
# Example GPIO action
from gpiozero import LED
led = LED(17)
led.on()
```

---

## 🛡️ Privacy First

Your data never leaves the device. Perfect for sensitive environments or offline usage.

---

## 🧪 TODO / Roadmap

- [ ] Add wake word configuration
- [ ] Improve NLP with offline large language models
- [ ] GUI dashboard for configuration
- [ ] Multi-language support
- [ ] Local music/media control

---

## 🤝 Contributing

Pull requests are welcome! Please open an issue first to discuss what you’d like to change.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📞 Contact

Created by [Your Name](mailto:youremail@example.com)

Project link: [https://github.com/yourusername/offline-voice-assistant](https://github.com/yourusername/offline-voice-assistant)
