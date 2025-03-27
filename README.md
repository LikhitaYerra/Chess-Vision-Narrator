
<h1 align="center">♟️ Chess Video Analyzer</h1>
<p align="center">
  <em>Watch. Decode. Comment. Entertain.</em><br>
  <strong>AI-powered Chess Video Summarizer with YOLO and LLMs</strong>
</p>

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
| `Untitled7.ipynb`| YOLO setup and chess piece detection pipeline                |
| `Untitled9.ipynb`| Full video-to-commentary system using LLM and optional TTS   |

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
   - `Untitled7.ipynb` – Piece detection using YOLO
   - `Untitled9.ipynb` – Move generation + commentary pipeline

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

## 📄 License

MIT License — feel free to use, fork, and improve this project!

---
