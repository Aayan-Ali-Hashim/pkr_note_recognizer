# 💵 PKR Note Recognizer

## 🌐 Live Demo

👉 [Click here to try the PKR Note Recognizer](https://pkr-note-recognizer-frontend.vercel.app/)

An AI-powered web application to recognize Pakistani currency notes using a deep learning model (MobileNetV2), a Flask backend, and a responsive web interface.

---

## 🔗 Related Repositories

- 🔧 **Backend (Flask + MobileNetV2 Model)**  
  [pkr_note_recognizer_backend](https://github.com/yourusername/pkr_note_recognizer_backend)

- 🎨 **Frontend (Web Interface)**  
  [pkr_note_recognizer_frontend](https://github.com/yourusername/pkr_note_recognizer_frontend)

---

## 🎯 Real-World Problem It Solves

Accurately identifying currency notes is critical in many everyday situations:

- Visually impaired individuals struggle to recognize note denominations.
- Businesses face human error in handling and verifying cash.
- Financial institutions require fast, automated note recognition for machines like ATMs, deposit kiosks, or cash counters.

This system provides an AI-based solution to recognize **Pakistani Rupee (PKR)** notes in real-time from images. It can be integrated into:

- Mobile apps for accessibility
- Retail checkout systems
- Currency validation hardware
- Educational or financial tech tools

---

## 🧠 Overview

The PKR Note Recognizer is a full-stack machine learning project that allows users to upload images of PKR notes and get the denomination prediction instantly. The backend uses a fine-tuned MobileNetV2 model, and the frontend provides a simple, intuitive interface.

---

## 📸 Demo

![Demo Screenshot](/ss.png)


---

## ⚙️ Tech Stack

| Layer      | Technology                     |
|------------|--------------------------------|
| Frontend   |  React
| Backend    | Flask (Python)                 |
| Model      | MobileNetV2 (TensorFlow/Keras) |
| Deployment | Render,Vercel                  |

---

## 🧩 Architecture

```text
[ User ]
   ↓
[ Frontend ]
   ↓ HTTP (Image Upload)
[ Flask API ]
   ↓
[ Trained MobileNetV2 Model ]
   ↓
[ Predicted Note Denomination ]

```
## Setup Instructions
✅ Prerequisites
- Python 3.8+
- Node.js and npm (if using React frontend)
- Git

**Clone the Main Project (with Submodules)**
```
git clone --recurse-submodules https://github.com/yourusername/pkr_note_recognizer.git
cd pkr_note_recognizer
```

If you forgot --recurse-submodules, run:
```
git submodule update --init --recursive
```

**Backend Setup (Flask + Model)**
```
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt

# Run the server
python app.py
```
- Backend runs at: http://localhost:5000
- API endpoint: POST /predict (accepts image file)

**Frontend Setup (React)**

```
cd ../frontend
npm install
npm start
```
- Frontend runs at: http://localhost:3000
- It connects to the Flask backend to fetch predictions.

**Dataset & Model**
- Dataset: Custom-collected images of PKR notes (10, 20, 50, 100, 500, 1000, 5000)
- Model: MobileNetV2 pretrained on ImageNet, fine-tuned on this dataset
- Accuracy: ~[90+]% on test data

**Features**
-  Upload image of PKR note and get prediction instantly
-  Lightweight model for fast inference
-  Simple and responsive web UI
-  Clean API interface for future integrations

**Future Improvements**
- Deploy as mobile app using React Native / Flutter
- Add audio output for accessibility
- Support multiple currencies
-Improve model with larger dataset and augmentations
- Add history/log of predictions

**🧑‍💻 Author**
Aayan Ali Hashim
[GitHub](https://github.com/Aayan-Ali-Hashim)
[LinkedIn](https://www.linkedin.com/in/aayan-ali-922a14p1b/)

