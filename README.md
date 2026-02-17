# AutoReel
# 🎬 Auto Story Video Generator & Uploader

An end-to-end automated AI content pipeline that generates short-form educational videos.

This system automatically:

- Generates a high-retention script
- Creates structured scene metadata
- Produces AI-generated images
- Synthesizes natural voice narration
- Synchronizes visuals with speech
- Exports a final ready-to-publish video

Built for scalable social media automation.

---

## 🚀 Features

### 🧠 AI Script Generation
- Powered by Groq (LLaMA 3.3 70B)
- Curiosity-driven topics
- Continuous natural narration
- Structured visual metadata

### 🖼️ AI Image Generation
- Stable Diffusion (local GPU)
- Scene-based prompt compilation
- Cinematic consistency
- Automated image pipeline

### 🎙️ Neural Voice Narration
- Microsoft Edge Neural Voices
- Continuous speech flow
- Adjustable speaking rate

### 🎞️ Intelligent Video Assembly
- Word-level timing synchronization
- Smooth crossfade transitions
- Subtle zoom (Ken Burns effect)
- H.264 + AAC export

---

## 🏗️ System Architecture

Groq LLM
↓
Structured JSON (full_script + scenes)
↓
Stable Diffusion → Scene Images
↓
Edge TTS → Full Narration Audio
↓
Word Timing Extraction
↓
MoviePy → Final Video


---

## 📂 Project Structure



AutoStoryGenAndUploader/
│
├── images/ # Generated scene images
├── audio/ # Generated narration files
├── outputs/
│ ├── images/
│ └── audio/
│
├── models/ # Stable Diffusion models
├── main.py # Main pipeline logic
├── requirements.txt
└── README.md


---

## ⚙️ Installation

### 1️⃣ Clone Repository
git clone <repo-url>
cd AutoStoryGenAndUploader

2️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate  # Windows

3️⃣ Install Dependencies
pip install -r requirements.txt


Recommended stable versions:

moviepy==1.0.3
decorator==4.4.2
pillow==9.5.0
edge-tts
diffusers
torch

🔑 Environment Variables

Create a .env file:

GROQ_API_KEY=your_groq_api_key

🧠 Script Generation Output Format
{
  "title": "",
  "full_script": "",
  "scenes": [
    {
      "scene_number": 1,
      "narration": "",
      "main_subject": "",
      "environment": "",
      "mood": "",
      "lighting": "",
      "camera": "",
      "key_elements": []
    }
  ]
}

🖼️ Image Prompt Compilation

Scene metadata is compiled into cinematic prompts:

cinematic stylized illustration of {main_subject} in {environment},
lighting: {lighting},
mood: {mood},
{camera},
featuring {key_elements}

🎙️ Narration Example
edge_tts.Communicate(
    text=full_script,
    voice="en-US-AndrewNeural",
    rate="+3%"
)

🎞️ Video Rendering

Scene duration calculated from narration timing

Smooth transitions using crossfade

Subtle zoom animation

Final MP4 export

📱 Output

16:9 or 9:16 format

Social-media ready

Fully automated pipeline

🎯 Purpose

This project demonstrates:

End-to-end AI automation

Script-to-video pipeline engineering

GPU-based image generation

Neural speech synthesis

Precise multimedia synchronization

It is designed as a scalable AI content engine.

🔮 Future Improvements

Auto subtitle generation

Background music with auto-ducking

Dynamic caption overlays

Multi-language support

Direct social media upload

📜 License

MIT License

👤 Author

Hamza Khan
Computer Science Student
AI • Machine Learning • Automation


---

If you want, I can now:

- Make a **portfolio-optimized version** (stronger for recruiters)
- Add GitHub badges
- Add demo GIF section
- Or make it look more like a serious AI product README

Tell me the direction.
