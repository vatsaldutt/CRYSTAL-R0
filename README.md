# CRYSTAL-R0 (Legacy)

Version from Jan 10, 2022
Original Repo: [https://github.com/vatdut8994/Crystal-Old.git](https://github.com/vatdut8994/Crystal-Old.git) \
Superseding version: [https://github.com/vatsaldutt/CRYSTAL-Mark-I.git](https://github.com/vatsaldutt/CRYSTAL-Mark-I.git)

---

## Behold… the Mighty Popsicle Robot

**CRYSTAL-R0** was my first *refined* attempt at building a physical robotic system intended to eventually host an AI assistant capable of perception, interaction, and autonomous action.

This version is now archived and was later superseded by **CRYSTAL-R1**, which was designed explicitly with tighter AI integration in mind. CRYSTAL-R0 primarily relied on **manual control**, augmented by early AI-driven perception and assistant software running off-device.

![Popsicle Robot](https://github.com/user-attachments/assets/b51aae66-d46d-4c80-81dd-a51e4638e4b9)

---

## Background

I was extremely constrained by available resources. The original chassis was built from **ice cream sticks collected over ~8 months**, long before I could afford proper robotics components. Over time, the robot was rebuilt multiple times, gradually incorporating:

* Gear motors
* Stronger structural elements
* Raspberry Pi and Arduino-based control
* Camera and sensor inputs

This project was built at the age of **11**, without formal knowledge of physics, control theory, or robotics. Everything was learned through trial, error, and hands-on experimentation. CRYSTAL-R0 represents that phase of raw, exploratory engineering.

---

## Hardware Overview

* Custom-built robotic arm and chassis
* Arduino-based motor control
* Bluetooth module for manual command input
* Camera for vision experiments
* Gradual migration toward Raspberry Pi integration

---

## Software Overview

CRYSTAL-R0 combined **robot control**, **AI assistant logic**, and a **desktop operating-style interface** into a single experimental system.

### Android Control App (Early Stage)

Initial manual control was implemented via a **custom Android app** built with **MIT App Inventor**.
This app sent Bluetooth signals to the Arduino, which handled low-level motor control.

> Yes, the UI wasn’t pretty. It worked. That was the goal.

<img width="1511" height="853" alt="Android App UI" src="https://github.com/user-attachments/assets/be135548-6190-41f2-bf7f-b51dae3e08d0" />

---

## Desktop Assistant & Control System (Major Upgrade)

Introduced a **desktop-based assistant and control environment** written in Python using **PyQt5**, representing a major leap in capability and ambition.

### Key Capabilities

* **Voice-controlled AI assistant**
* **Multilingual speech input/output** via Google Translate
* **ML-based intent classification** (Keras + NLTK)
* **Web search and scraping** (Google, Wikipedia, fallback crawling)
* **Face recognition–based user identification**
* **Text-to-speech (gTTS & pyttsx3)**
* **Wake-word detection**
* **Built-in desktop web browser**
* **Time, date, and UI state awareness**
* **Custom OS-like GUI shell**

---

## AI & Perception Features

### Intent Classification

* Bag-of-words model trained on custom intents
* Softmax classifier using Keras
* Confidence-thresholded responses

### Computer Vision

* Face recognition using `face_recognition` + OpenCV
* User identification before assistant activation
* Personalized greetings based on detected identity

### Information Retrieval

* Wikipedia summaries
* Google search scraping
* Fallback crawling and heuristic answer extraction
* Cached queries for performance

---

## Architecture (Legacy / Experimental)

CRYSTAL-R0 used a **highly monolithic architecture**, combining:

* UI rendering (PyQt5)
* Speech recognition
* Translation pipeline
* ML inference
* Web scraping
* Vision processing
* Assistant logic
* Robot control interfaces

This design was not scalable or modular—but it enabled rapid experimentation across **AI, UI, robotics, and perception** in a single system. Later CRYSTAL versions significantly refactored this approach.

---

## Author

**Vatsal Dutt**
Creator of CRYSTAL



