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

You can run this project locally in **Jupyter Notebook** or **Visual Studio Code (VS Code)**.

### ✅ Requirements

Make sure Python is installed, then install the required packages:

```bash
pip install opencv-python mediapipe pyautogui numpy
pip install screen_brightness_control pycaw comtypes
