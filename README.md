# GitHub Repo Analyser
GitHub Repo Analyser is a smart tool that scans repositories to deliver concise insights, including code structure, key metrics, and activity trends. It helps developers quickly understand projects, track performance, and make informed decisions efficiently.

Features
 Repository Analysis – Extracts and analyzes repo structure
 Tech Stack Detection – Identifies languages & frameworks used
 Architecture Insights – Understands project organization
 Code Metrics – Generates useful repo statistics
 AI Suggestions – Recommends improvements using LLM reasoning

🛠️ Tech Stack
Backend: FastAPI
Language: Python
AI Integration: LLM-based reasoning module
GitHub Integration: Custom API client

📂 Project Structure
app/
│── main.py                # FastAPI entry point
│
├── github/
│   ├── client.py          # GitHub API interaction
│   └── parser.py          # Repo URL parsing
│
├── analyzers/
│   ├── stack_detector.py  # Detects tech stack
│   ├── structure.py       # Analyzes repo structure
│   └── metrics.py         # Calculates repo metrics
│
├── llm/
│   ├── prompts.py         # Prompt templates
│   └── reasoning.py       # AI-based suggestions
│
└── services/
    └── analyze_repo.py    # Core analysis logic

Installation
# Clone the repository
git clone https://github.com/your-username/github-repo-analyser.git

# Navigate into the project
cd github-repo-analyser

# Create virtual environment
python -m venv venv

# Activate environment
venv\Scripts\activate   # Windows
source venv/bin/activate # Mac/Linux

# Install dependencies
pip install -r requirements.txt

Running the Application
uvicorn app.main:app --reload

