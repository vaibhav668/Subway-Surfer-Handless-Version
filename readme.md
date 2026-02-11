🎮 AI-Powered Gesture-Based Subway Surfers Controller

Play Subway Surfers without touching the keyboard.

This project uses real-time pose detection to control the game using body movements. It converts shoulder movement into directional keyboard inputs, enabling hands-free gameplay.

🚀 Project Overview

This system uses computer vision to detect body pose through a webcam and maps movement to in-game controls:

⬅️ Lean Left → Move Left

➡️ Lean Right → Move Right

⬆️ Move Up → Jump

⬇️ Move Down → Slide

The screen is divided into intelligent directional zones, and based on shoulder midpoint tracking, the system triggers corresponding key presses in real time.

This project explores:

Human-Computer Interaction

Gesture Recognition

Accessibility-focused Gaming

Real-time AI Applications

🛠 Tech Stack

Python

OpenCV

MediaPipe (Pose Estimation)

pynput (Keyboard Input Simulation)

🧠 How It Works

Webcam captures real-time video.

MediaPipe detects body landmarks.

Shoulder landmarks (11 & 12) are used to calculate midpoint.

Midpoint is compared against screen center.

If movement crosses threshold zones:

A keyboard arrow key is triggered.

Direction change logic prevents repeated key spamming.
