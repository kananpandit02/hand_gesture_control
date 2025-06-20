# 🖐️ Hand Gesture Control Suite using MediaPipe & OpenCV

[![Colab](https://img.shields.io/badge/Google%20Colab-%23000000.svg?logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/1Y4Mc3SkkGYlL9fyfsZeUveqfEqUZ8j_3?usp=drive_open)
![License: None](https://img.shields.io/badge/License-None-lightgrey)

---

## 📚 Table of Contents

- [📖 Overview](#-overview)  
- [🎯 Objectives](#-objectives)  
- [🧠 Motivation](#-motivation)  
- [🖐️ Hand Gesture Modules](#-hand-gesture-modules)  
  - [🖱️ Virtual Mouse Control](#️-part-1-virtual-mouse-control)  
  - [🔊 Brightness & Volume Control](#-part-2--brightness-and-volume-control-system)  
  - [📽️ Presentation Slides Control](#️-part-3--presentation-slides-control-system)  
- [🔮 Future Work](#-future-work)  
- [📢 Citation](#-citation)  
- [🌐 Connect With Us](#-connect-with-us)  

---

## 📖 Overview

This project is an all-in-one **Hand Gesture Control Suite** that leverages **MediaPipe**, **OpenCV**, and **PyAutoGUI** to perform system-level interactions using hand gestures captured through a webcam. The suite includes three main modules:  
- Virtual Mouse Control  
- System Brightness & Volume Adjustment  
- Presentation Slide Navigation  

It enables a **touchless interface** ideal for accessibility, smart environments, and hands-free computing.

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

## 🖐️ Hand Gesture Modules

---

### ✅ Part 1: Virtual Mouse Control

Control your mouse using hand gestures!  
Real-time hand tracking enables pointer movement, clicks, and scrolling:

| Gesture                       | Fingers Used                                | Description                       | Action               |
|------------------------------|---------------------------------------------|-----------------------------------|----------------------|
| 🤘 Spiderman Gesture         | Thumb + Index + Pinky up                    | Toggle mouse control              | 🖱️ Enable/Disable    |
| ☝️ Index Finger Up           | Only Index up                               | Cursor movement                   | 🖱️ Move cursor       |
| 🤏 Thumb + Index Touch       | Thumb and Index touching                    | Left Click                        | 🖱️ Click             |
| 🤏 Thumb + Middle Touch      | Thumb and Middle touching                   | Right Click                       | 🖱️ Right-click       |
| 🤏 Thumb + Index + Middle    | All three touching                          | Double Click                      | 🖱️ Double-click      |
| ✌️ Index + Middle Up         | Index and Middle up                         | Scroll Up                         | ⬆️ Scroll up         |
| 🖖 Index + Middle + Ring Up  | Index, Middle, Ring up                      | Scroll Down                       | ⬇️ Scroll down       |

ℹ️ Notes:
- Use **Spiderman gesture** to toggle control with a 1s cooldown.
- Ensure fingers are clearly visible and close together for clicks.
- Press **ESC** to exit the module.

---

### ✅ Part 2: Brightness and Volume Control System

Use wrist tilt + hand gestures to control system volume and brightness:

| Gesture                         | Hand   | Description                              | Action                            |
|----------------------------------|--------|------------------------------------------|-----------------------------------|
| 🤘 Spiderman Gesture             | Left/Right | Toggle control (Volume / Brightness)   | Enable control                    |
| ✋ Hand Tilt Up/Down             | Right  | Adjust brightness via tilt               | Brightness +/−                    |
| ✋ Hand Tilt Up/Down             | Left   | Adjust volume via tilt                   | Volume +/−                        |

🔎 Visual Feedback:
- Yellow bar = Brightness (bottom left)
- Blue bar = Volume (top right)
- ✅ Green = Active | ❌ Red = Inactive

---

### ✅ Part 3: Presentation Slides Control System

Control slides in presentations using clear gestures:

| Gesture Name        | Description                            | Action             | When It Works                      |
|---------------------|----------------------------------------|--------------------|------------------------------------|
| ✊ Fist              | Toggle START/STOP gesture system       | System ON/OFF      | Single hand + 5s cooldown          |
| 👉 Index Up         | Move to next slide                     | ➡️ Next Slide      | When system is STARTED             |
| ✌️ Index + Middle   | Move to previous slide                 | ⬅️ Previous Slide  | When system is STARTED             |

⌛ Cooldowns:
- Fist Toggle: 5s  
- Slide Control: 1s

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
