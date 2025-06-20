# 🖐️ Hand Gesture Control Suite using MediaPipe & OpenCV

[![Colab](https://img.shields.io/badge/Google%20Colab-%23000000.svg?logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/1Y4Mc3SkkGYlL9fyfsZeUveqfEqUZ8j_3?usp=drive_open)  
![License: None](https://img.shields.io/badge/License-None-lightgrey)

---

## 📚 Table of Contents

- [📖 Overview](#-overview)  
- [🎯 Objectives](#-objectives)  
- [🧠 Motivation](#-motivation)  
- [🚀 How to Run](#-how-to-run)  
- [🖐️ Hand Gesture Modules](#-hand-gesture-modules)  
  - [🖱️ Virtual Mouse Control](#️-part-1-virtual-mouse-control)  
  - [🔊 Brightness & Volume Control](#-part-2-brightness-and-volume-control-system)  
  - [📽️ Presentation Slides Control](#️-part-3-presentation-slides-control-system)  
- [🔮 Future Work](#-future-work)  
- [📢 Citation](#-citation)  
- [📄 License](#-license)  
- [🌐 Connect With Us](#-connect-with-us)

---

## 📖 Overview

**Hand Gesture Control Suite** is an integrated project developed by:

- **Kanan Pandit** (B2430051)  
- **Partha Mete** (B2430052)  
- **Ramakrishna Mission Vivekananda Educational and Research Institute**, Belur Math, Howrah, West Bengal

This project brings together multiple real-time hand gesture-based system control modules into one cohesive toolkit using **MediaPipe**, **OpenCV**, and **PyAutoGUI**. It enables intuitive, touchless interaction with a computer using simple hand gestures captured via webcam.

Modules included:
- 🖱️ Virtual Mouse  
- 🔊 Brightness & Volume Adjustment  
- 📽️ Presentation Slide Navigation  

Ideal for use in accessibility tools, smart classrooms, and human-computer interaction (HCI) research.

---

## 🎯 Objectives

- Develop accurate real-time hand gesture recognition using MediaPipe.
- Implement intuitive gesture-based controls for common computer tasks.
- Combine multiple gesture modules in a unified and easy-to-use system.
- Enable seamless user experience across platforms via webcam input.

---

## 🧠 Motivation

In a world moving toward **touchless interaction**, especially after the pandemic, gesture control offers a powerful alternative to traditional input devices. This project is designed to:
- Improve accessibility for differently-abled users.
- Explore human-computer interaction (HCI) using computer vision.
- Serve as a foundation for future smart home or classroom systems.

---

## 🚀 How to Run

You can run this project locally in **Jupyter Notebook** or **Visual Studio Code (VS Code)**
Make sure Python is installed, then install the required packages:
```bash
pip install opencv-python mediapipe pyautogui numpy
pip install screen_brightness_control pycaw comtypes
```
### 🧪 Steps to Run

1. **Clone the repository:**

```bash
git clone https://github.com/kananpandit02/hand_gesture_control.git
cd hand_gesture_control
```
2. **Launch Jupyter Notebook using::**
```bash
jupyter notebook
```
3. **Run each cell step-by-step:**
   Ensure your webcam is connected and accessible.

Only run one gesture module at a time to avoid conflicts.
3. **💡 Usage Tips:**
  Run the program in a well-lit environment.
  Use a plain background to avoid gesture misdetection.
  Keep gestures clear and deliberate.
  Press the ESC key to exit any module safely.


💡 Usage Tips
Run the program in a well-lit environment.

Use a plain background to avoid gesture misdetection.

Keep gestures clear and deliberate.

Press the ESC key to exit any module safely.











## 🖐️ Hand Gesture Modules

### ✅ Part 1: Virtual Mouse Control

Control your mouse using hand gestures!  
Real-time hand tracking enables pointer movement, clicks, and scrolling:

| Gesture                       | Fingers Used                       | Description           | Action             |
|------------------------------|------------------------------------|------------------------|--------------------|
| 🤘 Spiderman Gesture         | Thumb + Index + Pinky up           | Toggle mouse control   | 🖱️ Enable/Disable   |
| ☝️ Index Finger Up           | Only Index up                      | Cursor movement        | 🖱️ Move cursor      |
| 🤏 Thumb + Index Touch       | Thumb and Index touching           | Left Click             | 🖱️ Click            |
| 🤏 Thumb + Middle Touch      | Thumb and Middle touching          | Right Click            | 🖱️ Right-click      |
| 🤏 Thumb + Index + Middle    | All three touching                 | Double Click           | 🖱️ Double-click     |
| ✌️ Index + Middle Up         | Index and Middle up                | Scroll Up              | ⬆️ Scroll up        |
| 🖖 Index + Middle + Ring Up  | Index, Middle, Ring up             | Scroll Down            | ⬇️ Scroll down      |

#### ℹ️ Notes:
- Use **Spiderman gesture** to toggle control (1s cooldown).
- Ensure fingers are **clearly visible** and close together for clicks.
- Press **ESC** to exit the module.

---

### ✅ Part 2: Brightness and Volume Control System

Use wrist tilt + hand gestures to control system volume and brightness:

| Gesture               | Hand        | Description                        | Action             |
|-----------------------|-------------|------------------------------------|--------------------|
| 🤘 Spiderman Gesture  | Left/Right  | Toggle control (Volume / Brightness) | Enable control     |
| ✋ Hand Tilt Up/Down  | Right       | Adjust brightness via tilt         | Brightness +/−     |
| ✋ Hand Tilt Up/Down  | Left        | Adjust volume via tilt             | Volume +/−         |

#### 🔎 Visual Feedback:
- 🟡 Yellow bar = Brightness (bottom left)  
- 🔵 Blue bar = Volume (top right)  
- ✅ Green = Active | ❌ Red = Inactive

---

### ✅ Part 3: Presentation Slides Control System

Control slides in presentations using clear gestures:

| Gesture Name       | Description                      | Action             | When It Works                |
|--------------------|----------------------------------|--------------------|------------------------------|
| ✊ Fist             | Toggle START/STOP gesture system | System ON/OFF      | Single hand + 5s cooldown    |
| 👉 Index Up        | Move to next slide               | ➡️ Next Slide      | When system is STARTED       |
| ✌️ Index + Middle  | Move to previous slide           | ⬅️ Previous Slide  | When system is STARTED       |

#### ⌛ Cooldowns:
- **Fist Toggle**: 5 seconds  
- **Slide Control**: 1 second

---

## 🔮 Future Work

- Add **gesture-controlled media player** (play/pause/volume).
- Enable **custom gesture recording & training**.
- Integrate with **AR/VR or IoT systems** for smart environments.
- Optimize for **mobile devices or browser-based control**.
- Support for **gesture-based app switching and screen capture**.

---

## 📢 Citation

```bibtex
@misc{fusioneyes2025handgesturecontrol,
  author = {Kanan Pandit and Partha Mete},
  title = {Hand Gesture Control Suite using MediaPipe & OpenCV},
  year = {2025},
  url = {https://github.com/kananpandit02/hand_gesture_control}
}
```
## 📄 License

This project was developed as part of an academic research paper and is **not licensed for public use or redistribution**.

---

## 🌐 Connect With Us

- **Kanan Pandit** (B2430051)  
  🌐 [Portfolio](https://kananpanditportfolio.netlify.app/)  
  ✉️ kananpandot02@gmail.com  

- **Partha Mete** (B2430052)  
  🌐 [Portfolio](https://parthamete.github.io/portfolio/)  
  ✉️ metepartha2001@gmail.com  

- **Ramakrishna Mission Vivekananda Educational and Research Institute**  
  📍 Belur Math, Howrah, West Bengal

