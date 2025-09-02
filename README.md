# 🎓 SmartScribe – Lecture to Notes & PDFs

SmartScribe transforms **lecture recordings** (MP4) into:

- 📑 A **full transcript** (PDF)  
- 📝 Structured **study notes** (PDF)  
- ⚡ A one-page **cheat sheet** (PDF)  
- 📚 An **appendix** (PDF) with glossary/definitions  

It uses:
- 🎙️ OpenAI Whisper for transcription  
- 🖼️ OCR (EasyOCR + ffmpeg) to capture lecture slides  
- 🤖 GPT-4o for summarising and structuring notes  
- 📄 ReportLab for generating clean, professional PDFs  

---
GOOGLE DRIVE LINK: https://drive.google.com/file/d/1SCy8Fp0U-5c_hJ9ZbfJY6O8PHGOeGEAC/view?usp=sharing

---

## 🚀 Setup Instructions (Step by Step)

### 1. Clone the repository
```bash
git clone https://github.com/BahirQadeer/Melbourne-Hackathon-2025.git
cd smartscribe

###2. Create a Python virtual environment and activate it (Visual Studio Code is Recommended)
python3 -m venv venv

#(on mac)
source venv/bin/activate
#(on windows)
venv\Scripts\activate

### 3. Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install openai reportlab moviepy easyocr imageio-ffmpeg scikit-learn opencv-python faster-whisper python-dotenv
#(on mac)
brew install ffmpeg
#(On Ubuntu/Debian Linux:)
sudo apt update && sudo apt install ffmpeg

### 4. Set the OpenAI API Key
### (on mac)
export OPENAI_API_KEY="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"

### (on windows)
setx OPENAI_API_KEY "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"

### 5. Put your lecture video (e.g. lecture.mp4) in the same folder as main.py.

### 6. Run the program
python main.py lecture.mp4







