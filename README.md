# Senior Home Healthcare: AI System for Blood Pressure and Glucose Analysis

**Team Members**  
[@KyleHung7](https://github.com/KyleHung7) | [@samko5sam](https://github.com/samko5sam) | [@BlankTsai](https://github.com/BlankTsai) | [@peculab](https://github.com/peculab)

---
## 🎥 Initial Project Videos  
#### **(1) Proposal Video:** [Watch on YouTube](https://youtu.be/FfFTi43dxN8)  
#### **(2) Progress Report Video:** [Watch on YouTube](https://youtu.be/rVCsg0ngz98)
---
## 🎬 Contest Project Videos  
#### **(1)  Final Product Video:** [Watch on YouTube](https://youtu.be/pasdptc12KI) 
#### **(2)  Final Proposal Video:** [Watch on YouTube](https://youtu.be/20EEMxKKD0s)
---

## 🧠 Project Overview

**HealthLLM: AI-Powered Blood Pressure & Glucose Analysis for Elders**

This project addresses the rising health risks of **hypertension and diabetes** among the elderly in Taiwan—two of the top ten causes of death.  
It offers a **digital solution for families and caregivers** to monitor and manage elderly health data in real time using AI analysis.

---

## 🚨 Real-World Problem

- In Taiwan, **11,625 people died from diabetes** and **8,930 from hypertension** in 2023.
- **20–60% of diabetics** also suffer from hypertension, increasing risks of chronic complications like kidney failure or blindness.
- A case of an elderly patient fainting due to **hypoglycemia** after improper diet and medication adjustment highlighted the need for better daily monitoring.
- **Manual record-keeping is scattered**, often split between paper logs and chat apps like LINE, making data hard to manage.

---

## 🎯 Project Goals

- Enable families to **track elder health daily and accurately**
- Reduce health risks due to **lack of medical knowledge**
- Simplify health **recording and reporting** for caregivers
- Enhance **trust and peace of mind** through intelligent alerts

---

## 👥 Target Users

- **Elderly Patients (50+)** with hypertension or diabetes  
- **Family Caregivers (30–50 yrs)** actively involved in daily monitoring  
- **Care Institutions & Home Caregivers** managing multiple elders' data  

---

## 💡 Solution: HealthLLM System

We built a web-based platform tailored for senior healthcare that integrates:

- 📸 **Elder uploads photos** of health data → caregiver notified instantly  
- 📝 **Caregiver view**: table-based health logs, trend charts, and auto-generated reports  
- 🤖 **AI Assistant** for real-time Q&A and care guidance  
- 📤 **PDF reports** ready for doctor visits or family sharing  

---

## ⚙️ Technical Architecture

- **Frontend**: Python (Flask) for intuitive web interface 
- **Backend**: Python (Flask) for data handling & AI processing  
- **AI Tools**:
  - Trend detection (blood pressure & glucose)
  - Retrieval-Augmented Generation (RAG) for customized care advice  
- **Google OAuth**: Secure login for elders and caregivers

---
## Workflow

```mermaid
graph TD
    A[User fills in health information] --> B{Choose input method}
    B --> C1[Manually enter values]
    B --> C2[Photo recognition of health data gemini-2.5-flash-preview-04-17]
    
    C1 --> D{Health data validation}
    C2 --> E[Convert image to values] --> D

    D -->|Correct format| F[Save data to system]
    D -->|Incorrect format| G[Show error message and re-enter]

    F --> H{Perform analysis}
    H --> I[Blood pressure trend analysis gemini-2.0-flash]
    H --> J[Blood glucose trend analysis gemini-2.0-flash]
    H --> K[Health summary generation gemini-2.0-flash]
    H --> L[Care advice & QA via RAG: llama3.2, then gemini-2.0-flash]

    I --> M[Draw blood pressure chart]
    J --> N[Draw blood glucose chart]
    K --> O[Generate summary text]
    L --> P[Voice input via ffmpeg, voice output via whisper]

    M & N & O & P --> Q[Return and display results to user]
```

---
## 📅 Development Timeline

- **Weeks 9–15**: System design, implementation, and iteration  
- **Week 16**: Final presentation and testing with real users  

---

## 📈 Impact & Benefits

### 👴 For Elders  
- Daily data tracking = better disease management  
- Early warnings prevent serious complications  

### 👨‍👩‍👧 For Families  
- Less stress, better communication  
- Greater involvement and confidence in care  

### 🩺 For Doctors  
- Reliable data improves diagnosis and medication adjustment  
- Fewer emergency visits and hospitalizations  

### 🌍 For Society  
- Raises public awareness of chronic disease management  
- Supports aging population with scalable, sustainable tech  

---

## 🔮 Future Vision: From Home Care to Happy Workplaces

### For Enterprises  
- Integrate into corporate wellness programs  
- Support employees managing eldercare responsibilities remotely  

### Strategic Value  
- Lower employee stress and absenteeism  
- Strengthen organizational care culture  
- Enhance employer branding and talent retention  
- Align with **CSR**, **ESG**, and **age-friendly policies**

> _“A single platform to protect family health and build a sustainable care culture.”_


