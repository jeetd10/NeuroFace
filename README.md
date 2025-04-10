
---

# 😊 Face Emotion Recognition


### 🔗 [Live App](https://face-emotion-recognition.netlify.app)

A web app that detects **faces** and recognizes **emotions** in real time using your webcam!

Built using:
- [React](https://reactjs.org)
- [face-api.js](https://github.com/justadudewhohacks/face-api.js/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Framer Motion](https://www.framer.com/motion/)

---

## ✨ Features

### 🎥 Real-Time Emotion Recognition



- Detects faces from a webcam video stream  
- Identifies facial landmarks (like eyes, mouth, etc.)  
- Predicts emotions based on those landmarks

---

## 🎨 Tech & Design Decisions

- ✅ Used **React Context API** instead of Redux (since the app state is small).
- 🎨 Used **Tailwind CSS** for fast and responsive styling.
- 🎞️ **Framer Motion** adds smooth animations and transitions.
- 💻 Face detection and emotion recognition is done **entirely on the frontend** using `face-api.js`.

### Why Not Backend Detection?

Originally considered running face detection on a backend server. But that would:
- Require taking webcam photos frequently
- Send them to a server and wait for responses
- Delay emotion detection due to network speed

👉 Instead, running detection **in the browser** gives instant results—even on slow internet.

**Tradeoff:** This increases processing load on the user's device, which may cause slight lag on mobile devices. But it's worth it for real-time performance.

---

### 📁 Routing & Model Loading

- Used **react-router-dom** for routing with lazy loading.
- The app has two main pages:
  - **Home:** Loads instantly, lightweight
  - **Dashboard:** Loads after user clicks “Run,” and ML models (~6MB) are downloaded.

This gives a smooth user experience without a blank white screen.

---

### 🧰 Other Tools & Libraries

- 📸 [react-webcam](https://github.com/mozmorris/react-webcam): Webcam support  
- 🖼️ [html2canvas](https://github.com/niklasvh/html2canvas): Screenshots of charts  
- 📄 [jsPDF](https://github.com/parallax/jsPDF): Export charts as PDF  

---

### 😬 Things I’d Improve

- Should’ve used **TypeScript** instead of JavaScript.  
  - Early on it was fine, but as the project grew, it became harder to track object types and properties without good autocompletion.

---

## 🚀 Run Locally

```bash
git clone https://github.com/jeetd10/NeuroFace
cd face-emotion-recognition
npm install
npm run start
```

And you’re all set! 🙌

---

## 👥 Participants

| Name               | Roll Number     |
|--------------------|-----------------|
| Jeet Desai         | KU2407U304      |
| Harsh Yadav        | KU2407U286      |
| Prasiddhi Maloniya | KU2407U352      |

---


