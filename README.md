
<h1 align="center">♟️ Chess Video Analyzer</h1>
<p align="center">
  <em>Watch. Decode. Comment. Entertain.</em><br>
  <strong>AI-powered Chess Video Summarizer with YOLO and LLMs</strong>
</p>
              <div style="display: flex; justify-content: center; align-items: center; height: 100vh;">
  <img width="512" height="512" 
       alt="ChatGPT Image Aug 21, 2025 at 10_54_23 AM" 
       src="https://github.com/user-attachments/assets/1c90c24c-1fa3-46c2-a38e-6d2f4f31460a" />
</div>


---

## 🧠 What It Does

🎥 Takes a chess gameplay video and turns it into a narrated, move-by-move commentary show:

- 🕵️ Detects chess pieces and tracks movements using **YOLOv8**
- ♟️ Reconstructs the game by understanding board positions
- 🧠 Uses **OpenAI GPT** to generate fun or strategic commentary
- 🔊 Optional voice-over using **gTTS**
- 💻 Web interface with **Streamlit** (optional)

---

## 📁 Notebooks Overview

| Notebook         | Description                                                  |
|------------------|--------------------------------------------------------------|
| `YOLO.ipynb`| YOLO setup and chess piece detection pipeline                |
| `MAIN_APP.ipynb`| Full video-to-commentary system using LLM and optional TTS   |

---

## 🛠️ Tech Stack

- `YOLOv8` - Computer vision for object detection
- `OpenCV` - Video handling and frame processing
- `python-chess` - Board logic and legal move tracking
- `OpenAI` - LLM-generated strategic or fun commentary
- `gTTS` - Text-to-speech (optional)
- `Streamlit` - Simple web UI (optional)

---

## 🚀 Getting Started

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Add your **OpenAI API key** to environment variables or notebook.

3. Run the notebooks in order:
   - `YOLO.ipynb` – Piece detection using YOLO
   - `MAIN_APP.ipynb` – Move generation + commentary pipeline

---

## 🎬 Sample Output

> “White sacrifices the bishop… for *what* exactly? Let’s find out.”  
> <sub>– AI Chess Commentator</sub>

---

## ⚠️ Notes

- Best with **top-down chess videos**
- Fixed-angle camera improves accuracy
- Prompts can be customized to change tone of commentary

---
