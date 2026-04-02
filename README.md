# Grantfinder
GrantFinder: AI-Powered Travel Grant Discovery &amp; Proposal Generator  GrantFinder is an AI-driven, multi-agent system built to automate the process of discovering, evaluating, and applying for travel grants
📌 Overview

GrantFinder is a multi-agent AI system that automates the process of:

🔍 Finding relevant travel grants
📄 Extracting eligibility criteria
🧠 Summarizing & ranking opportunities
✍️ Generating a complete grant proposal



⚡ Problem

Finding academic travel funding is difficult because:

Grants are scattered across multiple websites
Eligibility is unclear and unstructured
Manual reading takes hours
Proposal writing is time-consuming
💡 Solution

GrantFinder solves this using a multi-agent pipeline:

Search → Extract → Summarize → Score → Draft Proposal
🧠 System Architecture
🔎 1. SearchAgent
Generates intelligent queries
Scrapes web results (Bing / DuckDuckGo)
Returns relevant grant URLs
📄 2. ExtractorAgent
Fetches web pages
Extracts eligibility sections
Uses fallback for noisy pages
🧠 3. SummarizerAgent
Uses Gemini API to summarize grants
Scores relevance using:
Keywords
Location
Travel/conference relevance
Ranks best opportunities
✍️ 4. DraftAgent
Generates a full grant proposal
Tailored to:
Conference
Research topic
Funding needs
Includes fallback when API quota is exceeded
🔄 Example Output
📌 Top Grant Found
Cornell Global Hubs Research Seed Grant
Score: 23.4
✍️ Generated Proposal (Snippet)
Proposal for Global Hubs Research Seed Grant: Advancing AI-Accelerated Materials Discovery for Carbon Capture and Utilization

Funding Request: USD 2,000

Objective:
To present research at an international conference and contribute to global decarbonization efforts.

Full proposal available here:
📄

🧪 Tech Stack
Python
Google Gemini API
BeautifulSoup (Web scraping)
Requests
tqdm (progress tracking)
Kaggle Notebook
🔑 Features

✅ Multi-agent architecture
✅ Real-time grant discovery
✅ Eligibility extraction from raw HTML
✅ Intelligent scoring system
✅ Automated proposal writing
✅ API quota-safe fallback logic
✅ Clean, production-ready outputs

🧠 AI Concepts Used
Multi-agent systems
Sequential workflows
LLM-powered reasoning
Custom tools (scraping + scoring)
Context engineering
Observability (logs + scoring)
Fallback handling (long-running systems)
🌍 Use Case

This system is designed for:

🎓 Students
🧑‍🔬 Researchers
🌱 Early-career innovators
🌍 Individuals from developing regions

Who need funding for:

Conferences
Research travel
Academic presentations
📂 Project Structure
GrantFinder/
│
├── grantfinder.ipynb       # Main notebook
├── proposal_draft.txt      # Generated proposal
├── grant_summary.json      # Ranked grants
├── memory_bank.json        # Agent memory/logs
├── README.md
⚙️ Setup
1. Install dependencies
pip install requests beautifulsoup4 tqdm google-generativeai
2. Set API Key

GOOGLE_API_KEY=your_api_key_here
▶️ Run
search_agent.run(profile)
extractor_agent.run(urls)
summarizer_agent.run(data)
draft_agent.run(top_grant)
📈 Impact

⏱️ Saves 3–5 hours → under 1 minute
📄 Generates ready-to-submit proposals
🌍 Improves access to global opportunities

🏆 Track

🟩 Agents for Good
Helping researchers access funding and global exposure

🔮 Future Improvements
Google Search API integration
PDF proposal export
Email automation
Grant alerts system
UI dashboard
👨‍💻 Author

Saksham Walia
University of Wollongong India

⭐ Final Note

GrantFinder demonstrates how AI agents can solve real academic problems by automating discovery, analysis, and content generation—making global opportunities more accessible.
