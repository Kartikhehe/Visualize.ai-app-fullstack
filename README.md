# Chat-to-Visualization App (I'mbesideyou Intern Assignment)

**Name:** Kartik Raj  
**Roll No. :** 230540
**University:** Indian Institute of Technology, Kanpur  
**Department:** Mechanical Engineering  

---

**Chat-to-Visualization App** is deployed at the following link:
https://visualize-ai-app.vercel.app

## 📘 Overview

**Chat-to-Visualization App** is an interactive AI-powered system that explains scientific concepts using both **text** and **visual animations**.  
When a user asks a question (e.g., *“Explain Newton’s First Law of Motion”*), the backend uses a Large Language Model (LLM) to generate:

- A **clear and concise explanation** of the concept  
- A **visualization specification (JSON)** that describes how the concept should be animated  

The frontend then displays:
- The **text explanation** in a chat-style interface (right side)  
- The **auto-generated visualization** on a canvas (left side)

---

## 💡 Use Case

This app is designed to make learning more **visual, engaging, and intuitive**, especially for students studying physics, biology, or other conceptual subjects.  
It bridges the gap between **reading** and **understanding** — helping users see how scientific principles work through interactive visualizations generated on the fly.

Typical use cases include:
- Understanding physics laws (e.g., motion, gravity, optics)  
- Visualizing biological or chemical processes  
- Teaching assistants or educators demonstrating concepts dynamically  

---

## ⚙️ Tech Stack

- **Frontend:** React.js  
- **Backend:** Node.js (Express)  
- **Realtime:** Server-Sent Events (SSE)  
- **LLM:** OpenAI GPT / Ollama / HuggingFace  
- **Database:** PostgreSQL or MongoDB  

---

## 🚀 Features

- 🧠 **AI-Powered Explanations:** Automatically generated responses for any conceptual question  
- 🎨 **Dynamic Visualizations:** Real-time canvas rendering from JSON animation specs  
- 💬 **Chat Interface:** Clean conversational layout for Q&A history  
- 🔁 **Realtime Streaming:** New answers streamed instantly using SSE  
- ⏯️ **Playback Controls:** Play / Pause visualization animations  

---

## 📂 API Endpoints

| Endpoint | Method | Description |
|-----------|---------|-------------|
| `/api/questions` | POST | Submit a user question |
| `/api/questions` | GET | Fetch all questions and their answer IDs |
| `/api/answers/:id` | GET | Fetch text + visualization for an answer |
| `/api/stream` | GET | Listen for realtime events (SSE) |

---

## 🧠 Example Flow

1. User asks:  
"Describe a Solar System"
2. Backend calls LLM → receives:
- Text: “The Solar System consists of the Sun at the center with planets orbiting due to gravity.”
- Visualization JSON: Animated circles showing orbits.  
3. Frontend renders:
- Chat with text explanation  
- Canvas with animated Sun and planets  

---

## 🧩 Future Improvements

- Support for **voice-based queries**  
- Option to **download visualizations** as video or GIF  
- Adding **RAG integration** for more accurate factual responses  
- A **multi-agent system** (Planner + Executor) for complex multi-step visualizations  

---

## 📜 License

This project was developed as part of the **AiPrep Internship Assignment**.  
All rights reserved © 2025 Kartik Raj.
