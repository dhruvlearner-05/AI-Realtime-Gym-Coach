# 🏋️ AI Real-Time Gym Coach

An AI-powered fitness coaching application that performs **real-time exercise detection**, **rep counting**, **posture analysis**, and **AI-powered voice coaching** using computer vision and large language models.

The application leverages **MediaPipe Pose**, **OpenCV**, **Groq LLM**, **SQLite**, and **Streamlit** to provide an interactive AI fitness coaching experience.

> **Live Demo:** https://ai-realtime-gym-trainers.streamlit.app/ 
> **GitHub Repository:** https://github.com/dhruvlearner-05/AI-Realtime-Gym-Coach

---

# ✨ Features

- 🎥 Real-time webcam-based exercise tracking
- 🤖 AI-powered coaching using Groq LLM
- 🔊 Real-time voice feedback using Text-to-Speech
- 🔢 Automatic repetition counting
- 📐 Joint angle calculation
- ✅ Posture and form correction
- 🔐 Secure user authentication
- 📊 Workout progress tracking
- 💾 Workout history stored in SQLite
- 🧩 Modular object-oriented architecture

---

# 🏃 Supported Exercises

- Squats
- Push-ups
- Biceps Curls
- Shoulder Press
- Lunges

Each detector performs:
- Repetition counting
- Joint angle computation
- Exercise-specific form analysis
- Live coaching feedback

---

# 🛠️ Tech Stack

### Frontend
- Streamlit
- HTML
- CSS

### Computer Vision
- OpenCV
- MediaPipe

### AI
- Groq LLM

### Voice
- gTTS

### Database
- SQLite

### Authentication
- bcrypt

### Python Libraries
- NumPy
- Pandas

---

# 📂 Project Structure

```text
AI-Realtime-Gym-Coach/
│
├── core/
├── detectors/
│   ├── squat.py
│   ├── pushup.py
│   ├── biceps_curl.py
│   ├── shoulder_press.py
│   └── lunges.py
├── ml_models/
├── services/
│   ├── auth/
│   ├── coaching/
│   ├── config/
│   ├── persistence/
│   ├── state/
│   ├── tracking/
│   ├── ui/
│   └── vision/
├── static/
├── .streamlit/
├── main.py
├── data.db
├── requirements.txt
├── packages.txt
└── README.md
```

---

# ⚙️ Installation

## Clone the Repository

```bash
git clone https://github.com/dhruvlearner-05/AI-Realtime-Gym-Coach.git
cd AI-Realtime-Gym-Coach
```

## Create Virtual Environment

```bash
uv venv
```

Windows

```bash
.venv\Scripts\activate
```

Linux/macOS

```bash
source .venv/bin/activate
```

## Install Dependencies

```bash
uv sync
```

or

```bash
pip install -r requirements.txt
```

## Configure Environment Variables

Create a `.env` file:

```text
GROQ_API_KEY=your_api_key
```

## Run the Application

```bash
streamlit run main.py
```

---

# 🧠 How It Works

1. Captures webcam frames using Streamlit WebRTC.
2. Detects body landmarks with MediaPipe Pose.
3. Calculates exercise-specific joint angles.
4. Counts repetitions using threshold-based state transitions.
5. Performs posture analysis and form validation.
6. Sends workout events to Groq LLM for personalized coaching.
7. Converts AI feedback into voice output.
8. Stores workout history and workout statistics in SQLite.

---

# 📊 Exercise Metrics

| Exercise | Metrics |
|----------|---------|
| Squats | Knee Angle, Back Angle, Depth Status |
| Push-ups | Elbow Angle, Body Alignment, Hip Position |
| Biceps Curls | Elbow Angle, Shoulder Stability, Swing Detection |
| Shoulder Press | Elbow Angle, Arm Extension, Back Arch Detection |
| Lunges | Front Knee Angle, Torso Angle, Balance status |

---



# 👨‍💻 Author

**Dhruv Jain**

---

# 📄 License

This project is licensed under the MIT License.
