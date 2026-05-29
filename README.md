# 💼 AI Job Assistant & ATS Optimization Engine (n8n Workflow)

An enterprise-grade, fully automated career intelligence pipeline built on **n8n**. This system acts as an elite AI career strategist that screens candidate resumes against specific job descriptions, scores ATS compatibility, generates bespoke recruitment-ready documents, and automates the delivery process.

---

## 🔄 Core Workflow Architecture
[Webhook Input] ➔ [Extract PDF Resume] ➔ [OpenAI Agent (GPT-4o-mini)] ➔ [HTML Dashboard Render] ➔ [HTML to PDF Generation] ➔ [Gmail Delivery] ➔ [Google Sheets Logging]

1. **Trigger:** Receives application details (Name, Email, Job Title, Company, Job Description) and a PDF resume via an **n8n Webhook**.
2. **Resume Parsing:** Extracts plain text from the uploaded PDF resume file.
3. **AI Intelligence Core:** Powered by **OpenAI GPT-4o-mini**, the system acts as a senior technical recruiter to perform a deep comparative gap analysis. It securely outputs:
   * A tailored, high-impact **Cover Letter** (300–450 words).
   * An **ATS-Optimized Resume Summary** prose.
   * A calculated **ATS Match Score (1-100%)** alongside missing keywords and actionable improvement metrics.
4. **Visual Rendering:** Formats the complex JSON analysis into a beautifully designed responsive modern glassmorphism **HTML Report**.
5. **PDF Compiler:** Converts the raw HTML dashboard into a downloadable high-quality PDF report.
6. **Automated Dispatch:** Instantly sends a personalized email to the applicant via **Gmail** with their application metrics and the PDF download link.
7. **Database Logging:** Records the user info, job metadata, timestamps, and document links into a **Google Sheet** for tracking.

---

## 🛠️ Tech Stack & Integrations

* **Workflow Automation:** n8n (Advanced AI & LangChain Nodes)
* **LLM Engine:** OpenAI Chat Model (`gpt-4o-mini`)
* **Document Processing:** Built-in PDF Text Extractor & HTML-CSS-to-PDF API
* **Email System:** Gmail OAuth2 Integration
* **Data Logging:** Google Sheets API

---

## 🌟 Key Features

* **Rigorous Extraction Intelligence:** Systematically evaluates must-have vs. nice-to-have qualifications without hallucinating fake candidate data.
* **Dynamic Glassmorphic UI:** Outputs a beautiful dashboard with native progress rings tracking candidate strength metrics.
* **Production-Ready & Fully Automated:** Runs silently in the background from ingestion to email delivery without needing manual intervention.

---

## 💻 Setup & Installation

### Prerequisites
* An active **n8n** instance (v1+ with Advanced AI components).
* API Keys/Credentials for:
  * OpenAI Developer Platform
  * HTML to PDF Service (htmlcsstopdf)
  * Gmail (OAuth2 authorized)
  * Google Sheets (OAuth2 authorized)

### Installation Steps
1. Clone this repository or download the `AI Job Assistant .json` file.
2. In your n8n workspace, click the top-right options menu (three dots) and select **Import from File**.
3. Upload the JSON file.
4. Set up your node credentials for **OpenAI**, **Gmail**, **Google Sheets**, and **HTML to PDF**.
5. Ensure your Google Sheet template contains the following columns: `email`, `job title`, `generated_at`, and `pdf_link`.
6. Set the workflow to **Active**.

---

## 📌 Repository Tags (Topics)
`n8n` `automation-workflows` `openai-gpt4` `ats-optimizer` `resume-parser` `ai-agents` `job-application-automation` `html-to-pdf` `langchain`
