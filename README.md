# 🚨 AI-Powered Incident Diagnosis & Root Cause Analysis Agent

A Python and Generative AI portfolio project that analyzes application logs and service metrics, builds an incident timeline, detects suspicious signals, ranks root-cause hypotheses, and generates structured incident reports.

## ✨ Features

- 📥 Application log and metric analysis
- 🧹 Log severity classification
- 📈 Metric anomaly detection
- 🕒 Incident timeline generation
- 🧠 Evidence-based root-cause hypothesis ranking
- 🤖 Optional LLM-powered incident analysis
- 🔍 Diagnostic recommendations
- 📤 JSON and Markdown report exports
- 🧑‍💻 Human-in-the-loop review

## 🛠️ Tech Stack

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Generative AI
- OpenAI-compatible API
- Python-dotenv

## 📂 Project Structure

```text
ai-incident-diagnosis-rca-agent/
│
├── ai_incident_diagnosis_rca_agent.ipynb
├── README.md
├── requirements.txt
├── .env.example
└── .gitignore
```

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/ai-incident-diagnosis-rca-agent.git
cd ai-incident-diagnosis-rca-agent
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the LLM API (Optional)

Create a `.env` file using `.env.example`:

```env
OPENAI_API_KEY=your_api_key_here
OPENAI_BASE_URL=
OPENAI_MODEL=gpt-4.1-mini
```

Never upload your actual API key or `.env` file to GitHub.

### 5. Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
ai_incident_diagnosis_rca_agent.ipynb
```

Execute the cells from top to bottom.

## 🧠 How It Works

1. Collect application logs and service metrics.
2. Normalize log severity levels.
3. Detect unusual error rates, latency, and database connection usage.
4. Build a chronological incident timeline.
5. Identify and rank potential root causes.
6. Use an optional LLM to explain the incident and suggest diagnostic checks.
7. Generate structured incident reports.

## 📊 Example Scenario

The demonstration simulates a checkout API incident involving:

- Increased HTTP errors.
- Higher P95 response latency.
- Database connection pool pressure.
- Database connection acquisition timeouts.

The system ranks database connection pool exhaustion as a possible root cause and suggests verification steps.

## ⚠️ Limitations

- Uses synthetic demonstration telemetry.
- Does not connect to live production monitoring systems.
- Anomaly thresholds require real-world calibration.
- Root-cause scores do not prove causality.
- LLM recommendations require human verification.
- Does not execute automated remediation.

## 🔮 Future Enhancements

- OpenTelemetry integration.
- Distributed tracing and trace correlation.
- RAG over incident reports and operational runbooks.
- Service dependency graph analysis.
- Historical incident learning.
- Streamlit or React dashboard.
- Integration with Prometheus and Grafana.
- Integration with Jira and Slack.
- Human-approved automated remediation.
- Incident prediction and risk scoring.

## 🔐 Security and Responsible AI

- Use sanitized telemetry for LLM processing.
- Never expose production secrets or credentials.
- Start with read-only monitoring permissions.
- Require human approval before operational changes.
- Maintain audit logs for incident investigations.

## 📄 License

Choose a license such as MIT before publishing the repository.

---

**Built with Python | Generative AI | Observability | Root Cause Analysis | Site Reliability Engineering**
