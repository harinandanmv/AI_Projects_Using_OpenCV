# 🧠 Real-Time AI Vision Tools

A powerful collection of real-time computer vision applications built using **Python**, **OpenCV**, **MediaPipe**, and more. Each module demonstrates a unique AI-powered visual utility — from detecting emotions to triggering alerts based on gestures or poses.

---

## 🚀 Features

* 🎭 Emotion detection with speech feedback
* 👀 Facial mesh visualization
* 🧤 Hand distance alert system
* 🧍 Human pose detection and intruder alarm with email
* 🧥 Invisibility cloak illusion (color masking)
* 🔴 Red object detection with HSV masking
* 🔧 Modular and extensible — ideal for demos or further development

---

## 🛠 Tech Stack

* Python 3.x
* OpenCV
* MediaPipe
* DeepFace
* pyttsx3
* NumPy
* smtplib (for alerts via email)

---

## 🔗 Modules Overview

* [`face_emotion_detection.py`](#face_emotion_detectionpy--facial-emotion-classifier)
* [`face_mesh_visualization.py`](#face_mesh_visualizationpy--face-mesh-viewer)
* [`hand_distance_alert.py`](#hand_distance_alertpy--hand-proximity-beeper)
* [`imposter_alarm.py`](#imposter_alarmpy--intruder-detection-with-email-alert)
* [`invisible_cloak.py`](#invisible_cloakpy--invisibility-cloak-effect)
* [`obj_detection.py`](#obj_detectionpy--red-color-object-detector)
* [`pose_detect.py`](#pose_detectpy--pose-estimation-viewer)

---

## 📁 Project Modules & Explanations

### `face_emotion_detection.py` – **Facial Emotion Classifier**

Detects real-time facial emotions using DeepFace and announces them via text-to-speech.
*Use Case:* Mood-aware systems, emotional feedback loops.

---

### `face_mesh_visualization.py` – **Face Mesh Viewer**

Applies facial landmark mesh in real-time using MediaPipe FaceMesh.
*Use Case:* Augmented reality, facial alignment, eye tracking.

---

### `hand_distance_alert.py` – **Hand Proximity Beeper**

Estimates the hand’s distance from the camera. If it’s too close, a beep is triggered.
*Use Case:* Gesture control alerts, interaction safety zones.

---

### `imposter_alarm.py` – **Intruder Detection with Email Alert**

Detects human pose and sends a frame capture via email alert. Audio alarm plays until the human is gone.
*Use Case:* Entry detection system, AI-powered lab alert.

---

### `invisible_cloak.py` – **Invisibility Cloak Illusion**

Masks red-colored fabric in webcam feed and replaces it with the static background.
*Use Case:* Visual effects, chroma-key experiments.

---

### `obj_detection.py` – **Red Color Object Detector**

Uses HSV color masking to detect red objects in the camera feed.
*Use Case:* Basic color-based tracking and interaction.

---

### `pose_detect.py` – **Pose Estimation Viewer**

Tracks human body pose using MediaPipe Pose and visualizes it.
*Use Case:* Fitness tracking, movement detection, pose classification.

---

## 📂 Project Structure

```
ai-vision-tools/
├── face_emotion_detection.py
├── face_mesh_visualization.py
├── hand_distance_alert.py
├── imposter_alarm.py
├── invisible_cloak.py
├── obj_detection.py
├── pose_detect.py
├── config.env             # Email credentials (keep secret)
├── .gitignore
├── README.md
└── requirements.txt
```

---

## ⚙️ Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/ai-vision-tools.git
cd ai-vision-tools
```

2. **(Optional) Create and activate a virtual environment**

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Configure email for intruder alert (optional)**
   Create a `config.env` file:

```
SENDER_EMAIL=your_email@gmail.com
EMAIL_PASSWORD=your_email_password_or_app_password
RECEIVER_EMAIL=receiver_email@gmail.com
```

5. **Run a module**

```bash
python face_emotion_detection.py
```

---

## 📄 .gitignore Example

```
.env
config.env
__pycache__/
*.pyc
*.jpg
*.log
venv/
```

---

## 📦 Sample `requirements.txt`

```
opencv-python
mediapipe
deepface
pyttsx3
numpy
```

To generate the full list:

```bash
pip freeze > requirements.txt
```

---

## ❓ FAQ

**Q: I get a "camera not available" or "device busy" error.**
A: Only one script can use the webcam at a time. Make sure no other module or app is using it.

**Q: My email alert isn’t working.**
A: Make sure you’re using an [App Password](https://support.google.com/accounts/answer/185833) for Gmail, and that less secure app access is enabled if required.

**Q: DeepFace throws a model loading error.**
A: Ensure you have internet access when first running it, as it downloads the models. You may also need to install `tensorflow`.

**Q: Nothing is spoken in the emotion detector.**
A: Check your system audio permissions and ensure `pyttsx3` is installed properly. It may need `espeak` or `sapi5` on your OS.

---

## 🙋‍♂️ Author

**M V Harinandan**
📧 [harinandanmv11@gmail.com](mailto:harinandanmv11@gmail.com)
🔗 GitHub: [github.com/yourusername](https://github.com/harinandanmv)
