# 🎸 Air Guitar with MediaPipe and Python

This is a virtual **Air Guitar** built using **MediaPipe**, **OpenCV**, and **Pygame** in Python. It lets you play guitar chords by simply using hand gestures in front of your webcam!

- 🖐️ Left hand: Chooses the chord based on the number of fingers up (like fretting).
- 🤚 Right hand: Detects strumming motion (like a real strum).
- 🔊 Plays sound based on the selected chord and strumming action.


## 🧠 How It Works

- Uses **MediaPipe Hands** to track both hands in real time.
- **Left hand** is used to count the number of raised fingers → selects one of 6 chords (0–5).
- **Right hand** is monitored for a quick vertical movement → simulates a strum.
- When a strum is detected, the currently selected chord is played using **Pygame** audio.


## 📁 Project Structure

air_guitar/
├── air_guitar.py # Main Python script
└── sounds/
├── 1.mp3
├── 2.mp3
├── EM.mp3
├── GM.mp3
├── 3.mp3
└── 4.mp3


> 🎵 **Note:** You need to provide your own chord or strumming `.mp3` files inside the `sounds/` folder.  
> These will correspond to finger counts 0 through 5.


## 🚀 Getting Started

### 1. Clone this repository

```
git clone https://github.com/agneya-1402/AirGuitar.git
cd AirGuitar
```
### 2. Install requirements
```
pip install opencv-python mediapipe pygame
```
### 3. Add your own chord audio files
Create a sounds/ folder in the same directory as the script, and add 6 .mp3 sound files:

1.mp3 → 0 fingers

2.mp3 → 1 finger

EM.mp3 → 2 fingers

GM.mp3 → 3 fingers

3.mp3 → 4 fingers

4.mp3 → 5 fingers

Feel free to rename and swap these with real chord sounds (e.g., from a guitar sample pack).

### 4. Run the script
```
python app.py
```
Then wave your hands in front of your webcam!


## 🛠️ Tech Stack
MediaPipe – Real-time hand tracking
OpenCV – Webcam and UI rendering
Pygame – Sound playback

## 🤘 Future Improvements
Add more realistic strumming logic (velocity-based volume or multi-string simulation)
Visual fretboard and chord labels
Add a GUI using Tkinter or PyQt
Create a browser version using MediaPipe Hands in JavaScript

## 🙌 Credits
Made with 💻 and 🎸 by Agneya Pathare

## 📄 License
MIT License – do whatever you want, just give credit!
