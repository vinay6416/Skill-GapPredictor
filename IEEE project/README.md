# Skill-Gap Predictor for Students (Career Navigation AI)
### IEEE CS Bangalore Chapter Internship and Mentorship Program – 2026

- **Project ID:** P19
- **Project Duration:** 1st April 2026 to 30th September 2026
- **Students / Developers:** 
  - Vinay Kumar S
  - Yashwanth K
  - Mahesh B K
- **Institution / University:** GITAM University, Bengaluru Campus
- **Faculty Mentor:** Dr. N. Gayathri (M29)

---

## 📌 Project Overview & Evolution (Months 1 – 4)

This project addresses the disconnect between college curricula and current industry recruitment expectations. Students frequently struggle to understand why their resumes are rejected or what precise competencies they lack for specific target roles.

- **Month 1 — Core Skill-Gap Engine:** Predefined company-role benchmark database, input skill matching, readiness scoring, and strength classification.
- **Month 2 — ATS Evaluation & PDF Reporting:** Resume upload (`pdfplumber`, `pypdf`), structure analysis, keyword density calculation, career learning roadmaps, and automated PDF export (`ReportLab`).
- **Month 3 — AI Intelligence & Dynamic Job Ranking:** Polished modern UI dashboard, dynamic tech domain detection, AI Confidence meter, Automatic Web Retrieval (AWR) with `BeautifulSoup`, and multi-role job ranking.
- **Month 4 — Personalization, Interview Prep & Placement Analytics:** Student profile management, SQLite database persistence, resume version history, AI interview drill generator, and interactive placement radar analytics (`Plotly`).

---

## 📂 Project Directory Structure

```text
IEEE project/
├── .vscode/
│   ├── launch.json              # 1-click VS Code Run / Debug configuration
│   └── settings.json            # VS Code Python environment settings
├── .streamlit/
│   └── config.toml              # Streamlit server and theme configurations
├── modules/
│   ├── __init__.py
│   ├── database.py              # SQLite profiles & resume scan history
│   ├── resume_parser.py         # PDF & DOCX text and section extractor
│   ├── skill_extractor.py       # Taxonomy, domain detection & synonym mappings
│   ├── ats_engine.py            # ATS score calculation & AI insights
│   ├── job_scraper.py           # AWR web retrieval & dynamic job ranking
│   ├── roadmap_generator.py     # 4-stage learning roadmaps & milestone projects
│   ├── interview_prep.py        # Technical & STAR behavioral question bank
│   └── pdf_generator.py         # Official IEEE PDF report generation
├── data/
│   └── company_roles.json       # Top tech companies, roles & required skills
├── static/
│   └── styles.css               # Clean, multi-line CSS stylesheet
├── app.py                       # Main Streamlit Dashboard application
├── render.yaml                  # Render.com cloud deployment blueprint
├── requirements.txt             # Python dependencies
├── .gitignore                   # Git exclusion rules
└── README.md                    # Project documentation
```

---

## 🚀 How to Run in VS Code (Localhost)

### Step 1: Open Folder in VS Code
1. Open **VS Code**.
2. Go to **File > Open Folder...** and select:
   ```text
   C:\Users\Mahesh B K\Documents\IEEE project
   ```

### Step 2: Open Integrated Terminal
Press ``Ctrl + ` `` (or go to **Terminal > New Terminal**).

### Step 3: Create and Activate a Python Virtual Environment (Recommended)
In PowerShell:
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```
*(If PowerShell displays a script execution policy restriction, run `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass` once).*

### Step 4: Install Dependencies
```powershell
pip install -r requirements.txt
```

### Step 5: Run the Web App
Execute:
```powershell
streamlit run app.py
```
Or simply press **F5** in VS Code (configured in `.vscode/launch.json`).

The application will automatically open in your web browser at:
👉 **`http://localhost:8501`**

---

## 👥 How to Push to GitHub (For Vinay, Yashwanth, and Mahesh)

### 1. Initialize Git Repository (First Person)
Run these commands inside the `IEEE project` folder:
```bash
git init
git add .
git commit -m "feat: complete IEEE P19 Skill-Gap Predictor Career Navigation AI"
git branch -M main
```

### 2. Connect to GitHub
Create a new empty repository on [GitHub](https://github.com/new) (e.g., `skill-gap-predictor-p19`), then link it:
```bash
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/skill-gap-predictor-p19.git
git push -u origin main
```

### 3. For the Other 2 Teammates to Collaborate:
The other team members can clone and work on the same repository:
```bash
git clone https://github.com/<YOUR_GITHUB_USERNAME>/skill-gap-predictor-p19.git
cd skill-gap-predictor-p19
pip install -r requirements.txt
streamlit run app.py
```
To share changes:
```bash
git pull origin main
git add .
git commit -m "update: improvements"
git push origin main
```

---

## 🌐 Deploy to Cloud via Render (render.com)

You can host this project online so your mentor and recruiters can access it with a live link:

1. Push this project to your GitHub repository.
2. Sign up / Log in to [Render](https://render.com).
3. Click **New + > Web Service**.
4. Select **Build and deploy from a Git repository** and pick your `skill-gap-predictor-p19` repository.
5. Render will automatically detect `render.yaml`, or you can configure:
   - **Environment:** `Python 3`
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `streamlit run app.py --server.port $PORT --server.address 0.0.0.0`
6. Click **Create Web Service**. Within 2-3 minutes, Render will provide you a live public HTTPS URL (e.g. `https://skill-gap-predictor-ai.onrender.com`).

---

## 🏆 Project Achievements
- Fully compliant with IEEE Internship Month 1 to Month 4 milestone deliverables.
- Accurate multi-factor ATS evaluation engine with section & contact integrity checking.
- Automated web scraping of job descriptions (AWR).
- Personalized 8-week learning pathways with milestone project ideas.
- Exportable IEEE-compliant PDF assessment reports.
