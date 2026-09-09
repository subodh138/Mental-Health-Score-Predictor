# 🧠 Mental Health Score Predictor

An end-to-end Machine Learning web application that predicts a student's mental health score based on social media habits, screen time, academic workload, and lifestyle metrics.

---

## 🚀 Live Demo

- **Frontend Application:** [https://mental-health-score-predictor-3-9hgc.onrender.com](https://mental-health-score-predictor-3-9hgc.onrender.com)
- **FastAPI Backend (Interactive API Docs):** [https://mental-health-score-predictor-1-hi0o.onrender.com/docs](https://mental-health-score-predictor-1-hi0o.onrender.com/docs)

---

## ✨ Features

* **Interactive SVG Gauge UI:** Real-time visual feedback displaying predicted mental health scores.
* **Robust Input Validation:** Dual-layer client-side and server-side validation using Pydantic schemas.
* **Machine Learning API:** RESTful API powered by FastAPI and Scikit-learn.
* **CORS Integration:** Configured with `CORSMiddleware` for seamless cross-origin requests.
* **CI/CD Deployment:** Automated deployment pipeline hosted on Render and synced with GitHub.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3, JavaScript (ES6+, Fetch API), Dynamic SVG Animations
* **Backend:** Python 3, FastAPI, Uvicorn, Pydantic
* **Machine Learning:** Scikit-learn, Pandas, Joblib
* **Deployment & Infrastructure:** Render (Web Service & Static Site), Git, GitHub

---

## 📋 API Reference

### `POST /predict`

Calculates and returns the predicted mental health score.

#### **Request Body (`JSON`)**
```json
{
  "age": 21,
  "gender": "Male",
  "country": "India",
  "academic_level": "Undergraduate",
  "most_used_platform": "Instagram",
  "purpose_of_use": "Entertainment",
  "avg_daily_usage_hours": 4.5,
  "daily_unlocks": 50,
  "study_hours": 6.0,
  "physical_activity_hours": 1.0,
  "sleep_hours_per_night": 7.0,
  "stress_level": "Medium"
}
