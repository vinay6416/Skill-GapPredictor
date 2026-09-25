# Skill Gap Predictor

## 📌 Project Overview

The **Skill Gap Predictor** is a web-based career analysis platform designed to help students and job seekers identify the gap between their existing skills and the skills required for their target job roles.

The system analyzes a user's resume, extracts relevant skills, compares them with the required skills for selected career roles, identifies missing skills, and provides a personalized roadmap for improving those skills.

The platform combines a PHP-based web interface with Python-based modules for resume parsing, skill extraction, ATS analysis, career-role matching, interview preparation, roadmap generation, and PDF report generation.

---

## 🎯 Problem Statement

Students and fresh graduates often find it difficult to understand whether their current technical skills are sufficient for a particular job role.

Traditional resume evaluation mainly focuses on resume formatting and keyword matching. It may not clearly explain:

* Which skills the candidate already possesses.
* Which skills are required for a particular job.
* Which skills are missing.
* Which skills should be learned first.
* How the candidate can prepare for the target role.

The **Skill Gap Predictor** addresses this problem by comparing candidate skills with job-role requirements and generating an understandable skill-gap analysis.

---

## 💡 Proposed Solution

The system provides a centralized platform where users can:

1. Upload their resume.
2. Extract existing skills automatically.
3. Select or identify a target job role.
4. Compare existing skills with required job skills.
5. Identify missing skills.
6. Analyze ATS compatibility.
7. Generate interview preparation material.
8. Generate a personalized learning roadmap.
9. Generate a PDF career analysis report.

---

## 🎯 Objectives

The main objectives of the Skill Gap Predictor are:

* To automatically extract skills from resumes.
* To identify technical and professional skills.
* To compare candidate skills with job-role requirements.
* To identify missing or insufficient skills.
* To provide skill-gap analysis.
* To suggest learning areas for career development.
* To support interview preparation.
* To generate personalized career roadmaps.
* To generate detailed PDF reports.
* To provide a simple and user-friendly career analysis platform.

---

## 🚀 Key Features

### 📄 Resume Analysis

The system allows users to upload their resumes and analyze their content.

Features include:

* Resume text extraction.
* Resume parsing.
* Skill identification.
* Education and experience information extraction.
* Resume content analysis.

---

### 🧠 Skill Extraction

The system identifies skills from the uploaded resume.

Examples include:

```text
Python
Java
SQL
HTML
CSS
JavaScript
React
PHP
MySQL
Git
Docker
Cloud Computing
Machine Learning
```

The extracted skills are used for further skill-gap analysis.

---

### 📊 Skill Gap Prediction

The main feature of the system is skill-gap analysis.

The system compares:

```text
Candidate Skills
       +
Target Job Requirements
       ↓
Skill Comparison
       ↓
Missing Skills
       ↓
Skill Gap Analysis
```

For example:

```text
Target Role: Python Developer

Required Skills:
✓ Python
✓ SQL
✓ Git
✓ REST API
✓ Flask
✓ Docker

Candidate Skills:
✓ Python
✓ SQL
✓ Git

Missing Skills:
✗ REST API
✗ Flask
✗ Docker
```

This helps users understand what they need to learn for their target role.

---

## 💼 Job Role Matching

The system contains job-role information and required skills.

Example:

```text
Software Developer
Python Developer
Web Developer
Data Analyst
Data Scientist
Cloud Administrator
Backend Developer
Frontend Developer
```

The system compares the user's skills with the requirements of the selected role.

---

## 📈 ATS Analysis

The system also provides Applicant Tracking System (ATS) analysis.

The ATS module can analyze:

* Relevant keywords.
* Required skills.
* Resume content.
* Job-role matching.
* Missing keywords.
* Resume improvement areas.

The purpose is to help users understand how closely their resume matches a target role.

---

## 🎤 Interview Preparation

The system provides interview preparation based on the selected career role.

It can generate:

* Technical questions.
* Programming questions.
* Role-based questions.
* HR interview preparation.
* Important topics to study.

Example:

```text
Target Role: Python Developer

Interview Topics:
- Python fundamentals
- OOP
- Data structures
- SQL
- REST APIs
- Flask
- Git
```

---

## 🛣️ Personalized Learning Roadmap

After identifying the skill gap, the system can generate a learning roadmap.

Example:

```text
Current Skills
      ↓
Missing Skills
      ↓
Priority Skills
      ↓
Learning Topics
      ↓
Projects
      ↓
Interview Preparation
      ↓
Target Job Role
```

This provides users with a structured direction for improving their employability skills.

---

## 📄 PDF Report Generation

The system can generate career analysis reports in PDF format.

The report can contain:

* Candidate information.
* Extracted skills.
* Target job role.
* Required skills.
* Existing skills.
* Missing skills.
* ATS analysis.
* Career recommendations.
* Learning roadmap.
* Interview preparation.

---

# 🏗️ System Architecture

```text
                         ┌──────────────────┐
                         │       USER       │
                         └────────┬─────────┘
                                  │
                                  ▼
                     ┌────────────────────────┐
                     │     Web Interface      │
                     │      PHP / HTML        │
                     │      CSS / JavaScript  │
                     └───────────┬────────────┘
                                 │
                                 ▼
                     ┌────────────────────────┐
                     │       PHP API          │
                     │        api.php          │
                     └───────────┬────────────┘
                                 │
                ┌────────────────┴────────────────┐
                │                                 │
                ▼                                 ▼
       ┌──────────────────┐             ┌──────────────────┐
       │     Database     │             │ Python Bridge    │
       │      MySQL       │             │    bridge.py     │
       └──────────────────┘             └────────┬─────────┘
                                                  │
                                                  ▼
                              ┌─────────────────────────────┐
                              │       Python Modules        │
                              ├─────────────────────────────┤
                              │ Resume Parser               │
                              │ Skill Extractor             │
                              │ ATS Engine                   │
                              │ Job Role Matcher             │
                              │ Interview Preparation        │
                              │ Roadmap Generator            │
                              │ PDF Generator                │
                              └──────────────┬──────────────┘
                                             │
                                             ▼
                              ┌─────────────────────────────┐
                              │      Skill Gap Analysis     │
                              └──────────────┬──────────────┘
                                             │
                                             ▼
                              ┌─────────────────────────────┐
                              │      Career Report / PDF    │
                              └─────────────────────────────┘
```

---

# 🔄 System Workflow

```text
User
 │
 ▼
Upload Resume
 │
 ▼
Resume Parser
 │
 ▼
Extract Resume Information
 │
 ▼
Skill Extractor
 │
 ▼
Identify Candidate Skills
 │
 ▼
Select Target Job Role
 │
 ▼
Retrieve Required Skills
 │
 ▼
Compare Skills
 │
 ├───────────────┐
 ▼               ▼
Matched       Missing
Skills        Skills
 │               │
 └───────┬───────┘
         ▼
   Skill Gap Analysis
         │
         ▼
 Learning Roadmap
         │
         ▼
 Interview Preparation
         │
         ▼
    PDF Report
```

---

# 🛠️ Technologies Used

## Frontend

* HTML5
* CSS3
* JavaScript

## Backend

* PHP
* Python
* Flask/API

## Database

* MySQL

## Python

* Python 3
* Resume parsing
* Skill extraction
* Data processing
* ATS analysis
* PDF generation

## Libraries

The required Python libraries are listed in:

```text
requirements.txt
```

Major libraries may include:

```text
Flask
Pandas
NumPy
PyPDF
ReportLab
Requests
```

---

# 📂 Project Structure

```text
IEEE project/
│
├── index.php
├── api.php
├── db.php
├── bridge.py
│
├── create_student_report.py
├── generate_final_report.py
│
├── Dockerfile
├── docker-compose.yml
├── render.yaml
├── requirements.txt
├── README.md
│
├── data/
│   └── company_roles.json
│
├── modules/
│   ├── __init__.py
│   ├── ats_engine.py
│   ├── database.py
│   ├── interview_prep.py
│   ├── job_scraper.py
│   ├── pdf_generator.py
│   ├── resume_parser.py
│   ├── roadmap_generator.py
│   └── skill_extractor.py
│
├── static/
│   ├── app.js
│   └── styles.css
│
└── workflow_diagram.png
```

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone https://github.com/vinay6416/IEEE-Project-.git
```

Move into the project directory:

```bash
cd IEEE-Project-
```

---

## 2. Install Python

Make sure Python 3 is installed.

Check the version:

```bash
python --version
```

---

## 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```powershell
venv\Scripts\activate
```

---

## 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🗄️ Database Configuration

The project uses MySQL for storing application data.

Database configuration is handled through:

```text
db.php
```

For local development, configure the required:

```text
Database Host
Database Name
Username
Password
Port
```

For production deployment, database credentials should be stored using environment variables rather than directly inside the source code.

---

# ▶️ Running the Project Locally

Start the required Python service:

```bash
python bridge.py
```

Then start the PHP application using your local PHP environment.

For example:

```bash
php -S localhost:8000
```

Open:

```text
http://localhost:8000/
```

---

# 🐳 Docker Deployment

The project contains:

```text
Dockerfile
docker-compose.yml
```

Build the Docker image:

```bash
docker build -t skill-gap-predictor .
```

Run the container:

```bash
docker run -p 8000:8000 skill-gap-predictor
```

Then open:

```text
http://localhost:8000/
```

---

# ☁️ Cloud Deployment

The project contains:

```text
render.yaml
Dockerfile
```

These files support cloud deployment.

The application can be deployed to a cloud hosting platform and accessed using a public HTTPS URL.

Example:

```text
https://skill-gap-predictor.onrender.com
```

The actual URL depends on the deployment configuration.

---

# 🔐 Security Considerations

For production deployment:

* Do not commit API keys to GitHub.
* Do not store database passwords directly in source code.
* Use environment variables for sensitive information.
* Validate uploaded resume files.
* Restrict allowed file extensions.
* Limit uploaded file sizes.
* Protect database credentials.
* Use HTTPS.
* Validate user input.
* Protect API endpoints.

---

# 📊 Example Skill Gap Analysis

### Target Role

```text
Backend Developer
```

### Required Skills

```text
Python
SQL
REST API
Git
Docker
Flask
Linux
```

### Candidate Skills

```text
Python
SQL
Git
```

### Identified Skill Gap

```text
REST API
Docker
Flask
Linux
```

### Suggested Learning Order

```text
1. REST API
2. Flask
3. Linux
4. Docker
```

### Recommended Preparation

```text
Backend Development
        ↓
REST APIs
        ↓
Flask
        ↓
Database Integration
        ↓
Docker
        ↓
Project Development
        ↓
Interview Preparation
```

---

# 📌 Advantages

* Simple resume analysis.
* Automated skill extraction.
* Job-role based skill comparison.
* Identifies missing skills.
* Provides career guidance.
* Supports ATS analysis.
* Generates learning roadmaps.
* Supports interview preparation.
* Generates PDF reports.
* Combines PHP and Python technologies.
* Can be deployed as a web application.

---

# 🔮 Future Enhancements

Future versions can include:

* AI-powered skill extraction.
* More job-role datasets.
* Real-time job-market data.
* Advanced skill prediction models.
* Personalized course recommendations.
* Voice-based interview practice.
* Resume improvement suggestions.
* Multi-language resume processing.
* User accounts and dashboards.
* Advanced analytics.
* Mobile application.
* Integration with online learning platforms.

---

# 🎓 Academic Project

The **Skill Gap Predictor** is developed as an academic/IEEE project to demonstrate the practical application of:

* Web Development
* Python Programming
* Resume Processing
* Skill Extraction
* Applicant Tracking System Analysis
* Database Management
* API Integration
* Career Analysis
* Recommendation Systems
* PDF Report Generation
* Cloud Deployment

---
# 👨‍💻 Developer
**Vinay Kumar S**
**Yashwanth K**
**Mahesh B K**
Engineering Students

GitHub:
https://github.com/vinay6416
---
# 📜 License
This project is developed for **educational and academic purposes**.
---
## ⭐ Project Goal
> **"Identify the skills you have, discover the skills you need, and build a roadmap to reach your target career."**
---
## 🔗 Repository
GitHub Repository:
https://github.com/vinay6416/IEEE-Project-
