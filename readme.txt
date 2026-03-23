# 🏥 AI Hospital Booking Assistant

## 📌 Overview

The **AI Hospital Booking Assistant** is an intelligent voice-enabled system that allows patients to interact with a virtual receptionist to book medical appointments seamlessly.

Powered by **FastAPI, Generative AI, and Speech Technologies**, the assistant can understand user queries, manage doctor schedules, and confirm appointments in real-time.

---

## 🚀 Key Features

### 🎙️ Voice-Based Interaction

* Real-time voice communication with AI receptionist
* Speech-to-text (user input) and text-to-speech (AI response)

### 🤖 AI Receptionist (Sarah)

* Acts as a hospital front desk assistant
* Understands natural language queries
* Supports **multiple languages**:

  * English
  * Hindi
  * Telugu

### 📅 Appointment Management

* View available doctors
* Check appointment slots
* Book appointments instantly
* Prevents double booking using database constraints 

### 🧠 Smart AI Integration

* Uses **Gemini AI** for conversational intelligence
* Handles tool-based function calling:

  * List doctors
  * Check availability
  * Book appointments

### 🔊 Audio Response System

* Generates natural voice responses using **gTTS**
* Returns audio in real-time to frontend

---

## ⚙️ How It Works

1. **Start Voice Call**

   * User enters name and email
   * Selects preferred language

2. **Conversation with AI**

   * AI receptionist greets the user
   * Understands intent (booking, inquiry, etc.)

3. **Backend Processing**

   * AI triggers backend tools:

     * Fetch doctors
     * Check availability
     * Book appointment

4. **Response Delivery**

   * AI responds via:

     * Text
     * Voice audio

---

## 🖥️ Tech Stack

* **Backend:** FastAPI
* **Frontend:** HTML, TailwindCSS, JavaScript 
* **Database:** SQLite
* **AI Model:** Google Gemini
* **Speech:**

  * SpeechRecognition (browser)
  * gTTS (text-to-speech)

---

## ⚙️ Installation & Run

### 1. Clone the Repository

```bash
git clone https://github.com/Pawan82003/AI-Hospital-Assistant.git
cd AI-Hospital-Assistant
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Setup Environment Variables

Create a `.env` file and add:

```env
GEMINI_API_KEY=your_api_key_here
```

### 4. Run the Application

```bash
uvicorn app:app --reload
```

### 5. Open in Browser

```
http://127.0.0.1:8000
```

---

## 📊 Database Design

### Doctors Table

* Doctor Name
* Specialty

### Appointments Table

* Patient Name
* Doctor Name
* Appointment Time
* Email
* Status

---

## 🌐 API Endpoints

* `GET /` → Load frontend UI
* `POST /agent/new_session` → Create AI session
* `POST /agent/message` → Send message to AI

---

## 🎯 Use Cases

* Hospital appointment booking
* Virtual receptionist systems
* Healthcare automation
* Voice-based AI assistants

---

## ⚠️ Disclaimer

This system is a prototype for demonstration purposes.
It is not intended to replace real hospital systems or medical professionals.

---

## 👤 Author

**Pawan**

---
