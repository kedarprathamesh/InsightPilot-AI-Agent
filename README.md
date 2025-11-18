# 📊 InsightPilot — AI Agent 

A lightweight, single-file Flask application that uses the **Gemini API** to simulate a **Senior Data Analyst**.
Provide any natural-language description of a dataset or analytical goal, and the system instantly generates a **comprehensive analysis report** including:

* Data Usability Scoring
* Key Metrics & Time-Series Insights (e.g., YOY comparisons)
* Simulated Exploratory Data Analysis (EDA)
* Strategic, Analyst-Level Recommendations

The interface is clean, responsive, and fully contained within one Python file.

---

## ✨ Key Features

### 🧠 **Senior Analyst Persona**

The model responds like an experienced data analyst—producing strategic, actionable, and clearly-structured insights.

### 📈 **Metrics & Analysis Generation**

Automatically identifies and produces:

* Suggested key performance metrics
* Time-series comparisons (YOY, MOM)
* Conversion metrics
* Behavioral trends
* Churn / retention signals

### 🎨 **Modern UI**

* Built with **Flask** (backend)
* **Tailwind CSS** for a clean and professional front-end
* **Showdown.js** to render Markdown results beautifully in the browser
  All served directly from a single file.

### 🗂️ **Single-File Deployment**

The entire application—including HTML, CSS, and JavaScript—is embedded inside **`InsightPilot-AI-Agent.ipynb`**, making deployment trivial.

---

## 🚀 Installation & Setup

### **Prerequisites**

* Python 3.x
* A **Gemini API Key** (from Google AI Studio)

---

### 1. **Download or Clone the Project**

```bash
git clone https://github.com/kedarprathamesh/InsightPilot-AI-Agent
```

Or download **`data_analysis_app.py`** directly.

---

### 2. **Install Required Packages**

```bash
pip install Flask requests
```

---

### 3. **Set Your Gemini API Key**

The app uses an environment variable: `GEMINI_API_KEY`

#### macOS / Linux:

```bash
export GEMINI_API_KEY="YOUR_API_KEY_HERE"
```

#### Windows (CMD):

```cmd
set GEMINI_API_KEY=YOUR_API_KEY_HERE
```

#### Windows (PowerShell):

```powershell
$env:GEMINI_API_KEY="YOUR_API_KEY_HERE"
```

> 💡 You *can* hardcode the key in the file, but environment variables are strongly recommended.

---

### 4. **Run the Application**

```bash
jupyter nbconvert --to notebook --execute InsightPilot-AI-Agent.ipynb
```

Visit in your browser:

```
http://127.0.0.1:5000
```

---

## 💡 How to Use

1. Open the app in your browser.

2. In the input box, describe your dataset or analytical goal:

   **Example Prompt:**
   *"I have customer activity data with columns: customer_id, subscription_date, monthly_spend, region. Provide YOY metrics and evaluate churn risk."*

3. Click **Generate Senior Analysis**.

4. The app returns a full professional report including:

   * Usability Score
   * Detailed Analysis
   * Key Metrics
   * Simulated EDA
   * Strategic Recommendations

---

## 📁 Project Structure

This project is intentionally simple:

```
InsightPilot-AI-Agent.ipynb   # Full Flask app + UI + Gemini logic in one file
```

No templates. No static directories. Fully self-contained.

---
