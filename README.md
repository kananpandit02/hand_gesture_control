# 🖐️ Hand Gesture Control Suite using MediaPipe & OpenCV

This project integrates multiple **hand gesture-based control systems** into a single interactive Jupyter Notebook using **MediaPipe**, **OpenCV**, and **PyAutoGUI**. It allows users to control:

- 🖱️ Virtual Mouse  
- 🔊 System Volume/Brightness  
- 📽️ Presentation Slides

---

## ✅ General Usage Guide for All Modules

Make sure the following conditions are met before using any gesture control module:

### 🎥 Enable Your Webcam
- Ensure your webcam is working and accessible.
- Hand tracking is done in **real-time** using webcam input.

### 💡 Run in a Well-Lit Environment
- Good lighting improves hand landmark detection accuracy.
- Avoid shadows on your hand or excessive glare.

### 🧹 Avoid Cluttered Backgrounds
- Use a clean and plain background to prevent gesture recognition errors.
- Avoid moving objects behind you.

### 🧩 Use One Module at a Time
- Run only **one gesture module at a time** for best performance and accuracy.
- Do not try to mix mouse, volume, and slide controls simultaneously.

### 🖥️ How to Run
- Open the project in **Jupyter Notebook** or **Visual Studio Code**.
- Run **each section individually** to activate the desired control system.
- All gesture modules work using **MediaPipe** + **OpenCV** + **webcam-based real-time hand tracking**.
### 📦 Requirements

Before running the project, make sure to install the required Python packages:
```bash
pip install opencv-python mediapipe pyautogui numpy
pip install screen_brightness_control pycaw comtypes

### ⛔ Exit Instructions
- Press the **ESC** key at any time to exit the program safely.

### ✅ Gesture Guide For All Modules
✅🖱️ Part 1: Virtual Mouse Control
Control your mouse with your hand!

✅ 🖐️ Virtual Mouse Control – Gesture Guide

| Gesture                       | Fingers Used                                | Description                       | Action               |
|------------------------------|---------------------------------------------|-----------------------------------|----------------------|
| 🤘 Spiderman Gesture         | Thumb + Index + Pinky up (Middle, Ring down) | Toggle mouse control (on/off)     | 🖱️ Enable/Disable mouse movement |
| ☝️ Index Finger Up           | Only Index up                                | Move mouse cursor                 | 🖱️ Cursor follows index tip     |
| 🤏 Thumb + Index Touch       | Thumb and Index touching                     | Perform Left Click                | 🖱️ Left-click       |
| 🤏 Thumb + Middle Touch      | Thumb and Middle touching                    | Perform Right Click               | 🖱️ Right-click      |
| 🤏 Thumb + Index + Middle    | All three touching (Index, Middle, Thumb)    | Perform Double Click              | 🖱️ Double-click     |
| ✌️ Index + Middle Up         | Index and Middle up                          | Scroll Up                         | ⬆️ Scroll content up |
| 🖖 Index + Middle + Ring Up  | Index, Middle, and Ring up                   | Scroll Down                       | ⬇️ Scroll content down |
## ℹ️ Notes:
- Make sure your hand is **clearly visible** to the webcam.
- Use the **Spiderman gesture** to **toggle mouse control** (with a 1-second cooldown).
- Click gestures require fingers to be **very close** (almost touching).
- Press **ESC** key to **exit** the program.


✅🔊 Part 2:  Brightness and Volume Control System

✅ ✋ Gesture-Based Brightness & Volume Control -Gesture Guide

| Gesture                         | Hand  | Description                                            | Action                            |
|----------------------------------|--------|--------------------------------------------------------|-----------------------------------|
| 🤘 Spiderman Gesture             | Left / Right | Thumb, Index, and Pinky up (others down)                 | Toggle control (Left = Volume, Right = Brightness) |
| ✋ Hand Tilt Up/Down (Active)     | Right  | Rotate hand upward/downward when active                | Increase / Decrease Brightness    |
| ✋ Hand Tilt Up/Down (Active)     | Left   | Rotate hand upward/downward when active                | Increase / Decrease Volume        |

---

## ℹ️ How It Works

- **Spiderman gesture** toggles control mode:
  - 🫱 **Right hand:** Toggle brightness control
  - 🫲 **Left hand:** Toggle volume control
- Once a hand is active:
  - **Tilt wrist upward** to increase
  - **Tilt wrist downward** to decrease
- **Smooth control** using angle difference and buffer.
- **Glow meters** show brightness and volume levels for visual feedback.
- **ESC key** exits the program.

## 📊 Visual Feedback

- **Yellow horizontal bar**: Brightness (bottom left)
- **Blue vertical bar**: Volume (top right)
- Control is **temporarily displayed** after each adjustment (1.5 seconds)
- Hand status displayed at the top:
  - ✅ Green = Active
  - ❌ Red = Inactive



✅📽️ Part 3:  Presentation slides Control System

✅ 🖐️ Presentation slides Control -Gesture Guide

This guide describes how to control your presentation slides using hand gestures powered by MediaPipe and OpenCV.

---

## ✨ Gesture Summary

| Gesture Name        | Hand Pose Description                                                                 | Action Triggered              | When It Works                         |
|---------------------|----------------------------------------------------------------------------------------|-------------------------------|----------------------------------------|
| ✊ **Fist Toggle**   | All fingers curled (tips below 2nd joints), like a closed fist                        | Toggle START/STOP system      | Only when **one hand is detected** + cooldown (5s) |
| 👉 **Next Slide**    | Only **index finger up** (middle, ring, pinky curled)                                 | Go to **next** slide (`→`)    | Only when system is **STARTED**       |
| ✌️ **Previous Slide**| **Index + middle fingers up** (ring + pinky curled)                                   | Go to **previous** slide (`←`)| Only when system is **STARTED**       |
| 🟩 **Status Bar**    | —                                                                                      | Displays `STARTED` (green) or `STOPPED` (red) | Always visible              |

---

## ⏱️ Cooldown Timings

| Name             | Purpose                                  | Duration     |
|------------------|-------------------------------------------|--------------|
| `TOGGLE_CD`      | Cooldown for **fist gesture toggle**      | 5 seconds    |
| `GESTURE_CD`     | Cooldown for **slide gestures**           | 1 second     |

---

## 💡 Notes

- **System is STOPPED by default.** Use the ✊ *fist gesture* to START or STOP it.
- Only **one hand** is actively analyzed for gesture control.
- All gestures rely on the position of hand landmarks from MediaPipe.
-Press **ESC** key to **exit** the program.



✅✅Regardless of which part you're running:

🧠 Best Practices
🖥️ Run only one module at a time to prevent conflicts.

🎯 Keep your hand centered and within the webcam frame.

💡 Ensure consistent lighting — avoid shadows or glare.

✋ Make deliberate and clear gestures — no fast or abrupt motion.


🔁 General Controls
📷 Webcam is essential — real-time hand tracking is the core.

⏹️ Press ESC anytime to exit any control system safely.

🎬 Each module runs independently — activate them one at a time from Jupyter Notebook or VS Code.



👨‍💻 Developed By
This project is part of the Hand Gesture Control Suite developed using:

🧠 MediaPipe – real-time hand tracking

🧰 OpenCV – image & video processing

🖱️ PyAutoGUI – mouse & keyboard automation

🔉 PyCAW – audio control on Windows

🌞 screen_brightness_control – brightness adjustments





