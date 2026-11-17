<div align="center">

# ✦ ANOMALIX AI ✦

### AI-POWERED LOG ANOMALY INVESTIGATION AGENT

**Detect. Investigate. Explain. Secure.**

![Python](https://img.shields.io/badge/Python-3.11+-gold?style=for-the-badge&logo=python&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-AI%20Agent-silver?style=for-the-badge)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Anomaly%20Detection-gold?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-silver?style=for-the-badge&logo=streamlit&logoColor=black)

**An intelligent cybersecurity investigation system that transforms raw server logs into meaningful security insights.**

</div>

---

## 🏆 1. Project Overview

**AnomaliX AI** is an AI-powered Log Anomaly Investigation Agent designed to analyze server logs, identify unusual activities, investigate suspicious patterns, correlate related events, and generate explainable investigation reports.

Traditional log monitoring systems often generate large volumes of alerts, making it difficult for security analysts to identify meaningful incidents.

AnomaliX AI addresses this challenge by combining **Machine Learning, intelligent agent-based investigation, log analytics, and explainable reporting** into a unified platform.

Instead of simply identifying unusual log entries, AnomaliX AI aims to investigate the surrounding evidence and help analysts understand:

- What happened?
- When did it happen?
- Which events are related?
- Why is the activity considered unusual?
- What evidence supports the finding?
- What should a human analyst investigate next?

---

## 🎯 2. Problem Statement

Modern applications and servers continuously generate large volumes of log data.

Security teams face several challenges:

- Huge volumes of server logs.
- Difficulty identifying abnormal activities.
- Repeated and noisy security alerts.
- Limited visibility into relationships between events.
- Time-consuming manual investigations.
- Difficulty understanding why an alert was generated.

**Our Solution:** AnomaliX AI combines anomaly detection with an AI investigation agent to turn raw log data into structured, explainable security investigations.

---

## 💡 3. Key Innovation

### From Log Detection to Intelligent Investigation

Most basic log monitoring systems focus on detecting unusual entries.

AnomaliX AI takes the process further.

| Traditional Log Monitoring | AnomaliX AI |
|---|---|
| Identifies unusual log entries | Detects and investigates unusual patterns |
| Generates individual alerts | Correlates related events |
| Requires manual analysis | Uses an AI agent to assist investigation |
| Provides limited context | Collects supporting evidence |
| Basic alert reporting | Explainable investigation reports |

**Core Differentiator:** Event correlation combined with an AI-powered investigation workflow.

---

## 🚀 4. Key Features

### 🔍 Intelligent Log Analysis
- Upload server log files.
- Parse and normalize log records.
- Extract timestamps, IP addresses, HTTP methods, endpoints, and status codes.
- Identify malformed or unsupported records.

### 🤖 AI Investigation Agent
- LangChain-powered investigation workflow.
- Uses specialized tools to analyze log evidence.
- Answers questions about analyzed logs.
- Generates context-aware investigation summaries.
- Explains findings using available evidence.

### 🧠 Machine Learning Anomaly Detection
- Isolation Forest-based anomaly detection.
- Feature engineering from log records.
- Identification of unusual traffic patterns.
- Detection results presented with supporting information.

### 🔗 Event Correlation
- Groups related suspicious events.
- Examines source IP addresses and time proximity.
- Identifies repeated error patterns.
- Connects related log activities into investigation cases.

### ⚖️ Risk Assessment
- Calculates investigation risk scores.
- Categorizes findings into risk levels.
- Combines machine-learning signals and rule-based indicators.
- Helps analysts prioritize investigations.

### 📁 Evidence Collection
- Collects relevant log records.
- Organizes supporting evidence.
- Connects findings with their original log entries.
- Provides context for investigation results.

### 📊 Interactive Security Dashboard
- Security overview.
- Anomaly statistics.
- Event timelines.
- Risk distribution.
- Investigation case summaries.
- Visual analytics.

### 📄 Automated Investigation Reports
- Investigation summaries.
- Anomaly details.
- Supporting evidence.
- Risk assessments.
- Recommended defensive next steps.

---

## 🏗️ 5. System Architecture

```text
                 ANOMALIX AI
                       |
                       ▼
              SERVER LOG UPLOAD
                       |
                       ▼
                LOG PROCESSING
                       |
                       ▼
              FEATURE ENGINEERING
                       |
                       ▼
           ┌───────────────────────┐
           │   ANALYSIS ENGINE     │
           │                       │
           │  Isolation Forest     │
           │  Rule-Based Detection │
           └───────────────────────┘
                       |
                       ▼
                RISK ASSESSMENT
                       |
                       ▼
                EVENT CORRELATION
                       |
                       ▼
           ┌───────────────────────┐
           │  ANOMALIX AI AGENT    │
           │                       │
           │  Log Analysis Tool    │
           │  Anomaly Detection    │
           │  Event Correlation    │
           │  Risk Calculation     │
           │  Evidence Collection  │
           │  Report Generation    │
           └───────────────────────┘
                       |
                       ▼
             INVESTIGATION RESULTS
                       |
             ┌─────────┴─────────┐
             ▼                   ▼
       AI ANALYST CHAT      REPORT GENERATION
             |                   |
             └─────────┬─────────┘
                       |
                       ▼
              STREAMLIT DASHBOARD
                       |
                       ▼
                HUMAN ANALYST
```

---

## 🤖 6. AI Agent Architecture

AnomaliX AI uses a central investigation agent supported by specialized tools.

### Main Agent: AnomaliX Investigation Agent

The agent coordinates the investigation process and uses tools to retrieve and analyze evidence.

| Agent Tool | Responsibility |
|---|---|
| `analyze_logs` | Analyzes parsed server logs |
| `detect_anomalies` | Identifies unusual patterns |
| `correlate_events` | Connects related events |
| `calculate_risk` | Calculates investigation risk |
| `collect_evidence` | Retrieves supporting log records |
| `generate_report` | Creates investigation reports |

### Agent Workflow

1. Receives an investigation request.
2. Determines which analysis tools are required.
3. Calls the appropriate tools.
4. Reviews the structured analysis results.
5. Produces an evidence-based explanation.
6. Generates an investigation summary.

**Important:** Machine learning and deterministic analysis perform the actual detection. The LLM helps interpret the structured results and communicate findings. The agent should not invent evidence or independently declare an attack without sufficient support.

---

## ⚙️ 7. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| LangChain | AI agent orchestration |
| LLM Provider | Investigation reasoning and explanations |
| Pandas | Log processing and analysis |
| NumPy | Numerical operations |
| Scikit-learn | Machine learning |
| Isolation Forest | Anomaly detection |
| Streamlit | Interactive web application |
| Plotly | Data visualization |
| SQLite | Optional investigation history |

---

## 🔄 8. Project Workflow

```text
STEP 1: Upload server logs
           |
STEP 2: Parse and normalize records
           |
STEP 3: Extract relevant features
           |
STEP 4: Run anomaly detection
           |
STEP 5: Apply security rules
           |
STEP 6: Calculate risk scores
           |
STEP 7: Correlate related events
           |
STEP 8: AI agent investigates findings
           |
STEP 9: Generate explanations and reports
           |
STEP 10: Human analyst reviews results
```

---

## 📂 9. Project Structure

```text
ANOMALIX_AI/
│
├── .vscode/
│
├── knowledge/
│
├── src/
│   └── anomalix_ai/
│
├── .gitignore
├── AGENTS.md
├── CLAUDE.md
├── CURSOR.md
├── GEMINI.md
├── README.md
├── pyproject.toml
└── uv.lock
```

---



## 💻 10. Installation and Setup

### Prerequisites

- Python 3.11 or compatible version.
- Visual Studio Code.
- Git.
- An LLM API key for the AI investigation features.

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/AnomaliX-AI.git
```

### Step 2: Navigate to the Project

```bash
cd AnomaliX-AI
```

### Step 3: Create a Virtual Environment

```bash
python -m venv .venv
```

### Step 4: Activate the Environment

**Windows PowerShell:**

```powershell
.venv\Scripts\Activate.ps1
```

### Step 5: Install Dependencies

```bash
python -m pip install --upgrade pip
```

```bash
python -m pip install -r requirements.txt
```

### Step 6: Configure Environment Variables

Create a `.env` file using `.env.example` as a reference.

Add your LLM provider's API key and required configuration.

**Never upload your actual `.env` file or API keys to GitHub.**

### Step 7: Run the Application

```bash
python -m streamlit run app/dashboard.py
```

The application should open in your browser.

---

## 📊 11. Expected Application Modules

| Module | Expected Output |
|---|---|
| Log Processing | Structured log records |
| Anomaly Detection | Anomaly classifications |
| Rule Engine | Security indicators |
| Risk Engine | Risk scores and categories |
| Event Correlation | Grouped investigation cases |
| AI Agent | Evidence-based investigation explanations |
| Dashboard | Interactive analytics |
| Report Generator | Downloadable investigation reports |

---

## 🛡️ 12. Security and Reliability

AnomaliX AI is designed with the following principles:

- Evidence-based investigation.
- Explainable anomaly detection.
- Secure API key management.
- Input validation.
- Error handling for malformed log files.
- Human-in-the-loop investigation.
- No automatic destructive actions.
- Clear separation between observed facts and possible explanations.

The system supports investigation and decision-making. Final security decisions remain with a human analyst.

---

## 🧪 13. Testing and Validation

The project should be validated using controlled sample log datasets.

Important test areas:

- Valid log parsing.
- Invalid log handling.
- Feature extraction.
- Anomaly detection.
- Risk score calculation.
- Event correlation.
- Evidence retrieval.
- Report generation.
- AI agent tool execution.
- Missing API key handling.

Synthetic log data should be clearly identified as synthetic.

---

## 🔮 14. Future Enhancements

Potential future improvements include:

- Real-time log monitoring.
- Integration with SIEM platforms.
- Multi-source log analysis.
- Advanced temporal anomaly detection.
- Historical anomaly comparison.
- Threat intelligence enrichment.
- Investigation case prioritization.
- Multi-format log ingestion.
- Advanced explainability.
- Role-based analyst access.

---

## 🎯 15. Project Goals

AnomaliX AI aims to:

1. Reduce manual log investigation effort.
2. Improve visibility into unusual server activities.
3. Connect related events into meaningful cases.
4. Provide explainable investigation results.
5. Assist analysts in prioritizing security findings.
6. Demonstrate practical integration of AI agents and machine learning in cybersecurity.

---

## 👨‍💻 16. Developer

**Project:** AnomaliX AI  
**Category:** Artificial Intelligence | Machine Learning | Cybersecurity  
**Project Type:** AI-Powered Investigation Agent  
**Primary Language:** Python

**Developer:** YOUR NAME

---

## ⭐ 17. Support the Project

If you find AnomaliX AI interesting:

- Give the repository a ⭐ Star.
- Fork the repository.
- Explore the source code.
- Share feedback and suggestions.

---

<div align="center">

### ✦ ANOMALIX AI ✦

**DETECT. INVESTIGATE. EXPLAIN. SECURE.**

*Turning raw logs into intelligent security investigations.*

</div>
