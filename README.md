
# ♟️ Chess Vision Narrator

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Computer%20Vision-green.svg)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow.svg)
![License](https://img.shields.io/badge/License-MIT-red.svg)

---

**Created by: John Doe**  
**Date: March 26, 2025**

Welcome to **Chess Vision Narrator**, a magical fusion of chess, computer vision, and a sprinkle of humor! Picture this: a machine that gazes upon a chessboard, tracks every pawn’s bold step and knight’s daring leap, and weaves a witty tale of the battle. That’s the adventure I, John Doe, set out to craft—a tool that not only detects moves from video but narrates them with a grin.

---

## 🎬 The Story Begins

In a flickering room, I watched two chess masters duel, their pieces dancing across the board. A wild thought struck me: *What if a machine could see this game and tell its story?* Thus began my quest—to build a system that spots the 12 chess warriors (pawns, rooks, knights, bishops, queens, kings, in black and white), follows their moves, and spins them into tales like “That pawn to e4 is braver than a knight in shining armor!” From shadowy corners to shaky hands, this journey battles every challenge to bring chess to life.

---

## 🛠️ The Magic Behind the Curtain

Here’s how this enchanted contraption works:

- **The Eagle Eye**: Powered by [YOLOv8](https://github.com/ultralytics/ultralytics) (small variant, `yolov8s.pt`), it spots chess pieces with near-perfect precision (mAP50: 0.991).
- **The Move Weaver**: A custom `ChessMoveDetector` tracks piece movements across video frames, maps them to the 8x8 board, and validates them with `python-chess`.
- **The Bard**: [OpenAI’s GPT-4](https://openai.com) crafts humorous commentary, brought to life as audio by `gTTS`.
- **The Stage**: A [Streamlit](https://streamlit.io) app lets you upload videos, watch the annotated moves, and hear the tale.

Built in Google Colab with a Tesla T4 GPU, this is a blend of tech and whimsy!

---

## 📚 The Treasure Chest: Dataset

The heart of this quest lies in the `Chess-Piece-Detection-2` dataset from [Roboflow](https://roboflow.com). A trove of images—hundreds, maybe thousands—shows chessboards in all their glory: wooden, plastic, bright, dim, top-down, or angled. Each piece is marked with YOLO-friendly bounding boxes, ready to train our eagle-eyed model.

---

## 🏆 The Spoils of Victory

After 11 epochs of training, the results dazzled:
- **Training Triumph**: YOLOv8 hit an mAP50 of 0.991, with weights saved to `/content/drive/My Drive/Chess_Model/`.
- **Move Magic**: Tested on `How To Play The Queen’s Gambit.mp4`, it traced moves like "e4", "e5", "Nf3" and crafted an annotated video.
- **Narration Glory**: The Streamlit app delivered moves, visuals, and a downloadable audio tale.

A few gremlins (file path mix-ups, mAP errors) were banished, but the saga continues with more videos to conquer!

---

## 🚀 Dreams of Tomorrow

The horizon beckons with grand adventures:
- 🌟 **Live Action**: Optimize for real-time webcam narration with YOLOv8 nano.
- 📖 **Rich Tales**: Expand the dataset with synthetic boards or crowd-sourced games.
- 🧠 **Wise Counsel**: Add [Stockfish](https://stockfishchess.org) to judge moves—blunders or brilliance.
- 👥 **Player Dance**: Track hands or use multi-cameras to spot turns.
- 📱 **Far and Wide**: Package it as an app or web service, mobile-ready.

This could become the ultimate chess companion!

---

## 🧩 How to Join the Quest

### Prerequisites
- Python 3.8+
- Google Colab (or a GPU-enabled setup)
- Libraries: `ultralytics`, `openai`, `gtts`, `streamlit`, `python-chess`

### Setup
1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/chess-vision-narrator.git
   cd chess-vision-narrator
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Train the model (see `train.ipynb`).
4. Run the app:
   ```bash
   streamlit run app.py
   ```

### Files
- `train.ipynb`: Trains YOLOv8 on the dataset.
- `app.py`: The Streamlit app for move detection and narration.
- `ChessMoveDetector.py`: Core move detection logic.

---

## 🤝 Contribute to the Saga

Spotted a bug? Got a wild idea? Pull requests and issues are welcome! Let’s make this tale legendary.


*“A pawn’s journey begins with a single step, but with vision and voice, it becomes an epic.”*  
Happy coding, and may your moves be brilliant!
```

