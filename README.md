# 🦖 Hand Gesture Controlled Dino Game using Computer Vision

This project lets you **control the Chrome Dino game** using your **hand gestures** via OpenCV and MediaPipe.  
It tracks your hand landmarks and detects how many fingers are open or closed to control the dinosaur’s actions.

---

## 📂 Repository Contents

- **`main.py`** — Main script that captures webcam feed, detects hand gestures, and triggers Dino game actions.
- **`directkeys.py`** — Script to simulate keyboard key presses for controlling the Dino.
- **`handland_marks.png`** — Image reference for hand landmark positions (from MediaPipe).
- **`README.md`** — Project documentation.
- **`LICENSE`** — MIT license for open-source usage.

---

## 🎮 How It Works

1. **Hand Tracking** — Uses MediaPipe to detect 21 landmarks on your hand in real-time.
2. **Finger Count Detection** — Determines how many fingers are open based on landmark positions.
3. **Game Control Logic**:
   - **1 to 4 fingers open** → Dino keeps running (no jump).
   - **All 5 fingers closed (fist)** → Dino jumps.

The detection is continuous, so you can play the game without touching the keyboard.

---

## 🚀 Features

- Play without touching the keyboard
- Real-time hand tracking using a webcam
- Simple and intuitive control gestures
- Uses MediaPipe for accurate and fast landmark detection

---

🎥 Gameplay Demo
![Gameplay Demo](gameplay.gif)

---

## 📦 Installation

Make sure you have **Python 3.7+** installed.

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Hand_Gesture_Dino_Game_using_CV.git
   cd Hand_Gesture_Dino_Game_using_CV

2. Install dependencies:

   ```bash
   pip install opencv-python mediapipe
   ```

---

## 🖥 Usage

1. Open the **Chrome Dino Game**:

   * Disconnect from the internet and press space in Chrome **OR**
   * Visit: [chrome://dino](chrome://dino)

2. Run the script:

   ```bash
   python main.py
   ```

3. Make sure your webcam is active and your hand is visible in the frame.

4. Control the Dino:

   * Show **1–4 open fingers** → Dino runs as usual.
   * Make a **closed fist** (0 fingers open) → Dino jumps.

---

## 📄 Hand Landmark Reference

The file `handland_marks.png` shows how MediaPipe indexes the 21 landmarks on the hand.
This project uses those points to calculate finger positions and determine if they are open or closed.

---

## ⚖ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

* [OpenCV](https://opencv.org/) — Computer vision library
* [MediaPipe](https://mediapipe.dev/) — Hand tracking solution by Google
* Chrome Dino Game — Built into Google Chrome
