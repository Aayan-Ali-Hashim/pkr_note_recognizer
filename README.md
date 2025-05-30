# 💵 PKR Note Recognizer

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
