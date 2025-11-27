<div align="center">
  <!-- Replace this link with your actual logo file -->
  <img width="290" height="1024" alt="Gemini_Generated_Image_3pw40i3pw40i3pw4" src="https://github.com/user-attachments/assets/9a01e030-80de-410a-b79a-4494d6f3c807" />
  <h1>GradeGuard AI</h1>
  <h3>Multi-Agent Academic Health Assessment & Exam Readiness System</h3>
</div>
GradeGuard AI is a machine-learning powered multi-agent framework built to analyze student performance, assess academic risk, evaluate exam eligibility, and generate personalized study recommendations.  
Developed as part of the **Kaggle 5-Day Intensive AI Agent Challenge**, this project demonstrates how predictive modeling and coordinated AI agents can meaningfully support academic decision-making.

---

## Overview  

Educational institutions and students often lack a unified, data-driven system to understand academic standing, detect risk factors, or prepare effectively for exams. GradeGuard AI addresses this challenge by combining:

- Machine learning predictions  
- Structured multi-agent collaboration  
- Memory and reasoning capabilities  
- Academic health evaluation  
- Visual performance analytics  

The result is a system that acts as a **virtual academic advisor**, capable of analyzing real student behavior and providing actionable insights.

---

## Core Features  

### Performance Insights  
Extracts academic patterns from ML predictions, including performance distribution, absence trends, and failure risk.

### Personalized Study Recommendations  
Generates a 7-day adaptive study plan, computes academic risk, and provides curated study resources.

### Academic Health Evaluation  
Assesses attendance, internal scores, and failure count to determine mid-semester and final exam eligibility.

### Advisor Interaction  
A basic conversational agent that generates study plans, displays progress, and supports simple academic queries.

### Study Progress Memory  
Stores day-wise study hours to track learning habits and consistency over time.

### Visual Dashboards  
Includes performance visualizations, eligibility summaries, and heatmaps to improve interpretability.

---

## Multi-Agent Architecture  

The system is composed of five coordinated agents:

- **Insights Agent** – Statistical and performance analysis  
- **Recommendation Agent** – Study planning and risk scoring  
- **Academic Health Agent** – Eligibility evaluation and attendance analysis  
- **Advisor Agent** – Query-based interaction  
- **Memory Agent** – Study progress tracking  

A central **System Controller** manages communication across all agents.

---

## Machine Learning Integration  

A separate ML notebook was used to train a model on:

- Study time  
- Absences  
- Failures  
- Internal scores (G1, G2)  

The model outputs a predicted performance class for each student.  
This result is stored as: `student_predictions.json` and used as the primary data source for the agents.

---

## Repository Structure  
```bash
GradeGuard-AI/
│
├── GradeGuard_AI.ipynb # Main notebook with full multi-agent system
├── student-performance-prediction.ipynb
├── student_predictions.json # ML output used by agents
├── README.md # Project documentation
```

---

## How to Run  

### Option 1 — Kaggle  
Upload the notebook, attach the dataset containing `student_predictions.json`, and run all cells.

### Option 2 — Local  
```bash
git clone https://github.com/<your-username>/GradeGuard-AI.git
cd GradeGuard-AI
jupyter notebook GradeGuard_AI.ipynb
```
## Future Work

- GradeGuard AI is designed as an expandable academic intelligence system. Planned enhancements include:
- LLM-based Advisor Agent for natural, conversational guidance
- Teacher Analytics Dashboard for class-level insights
- Predictive Exam Score Modeling for early risk notifications
- Topic-wise learning recommendations to identify weak areas
- Mobile/Web deployment for real-world student use
- Integration with LMS systems (Google Classroom, Moodle, Canvas)

These extensions aim to evolve GradeGuard AI into a comprehensive academic decision-support platform.

## Conclusion

GradeGuard AI demonstrates how multi-agent systems combined with machine learning can enhance educational decision-making.
It provides students with meaningful academic insights, structured study support, eligibility evaluation, and clear performance analytics.

The system is a foundation for future AI-driven educational tools aimed at improving student outcomes at scale.
