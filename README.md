# ScholarAgent

**ScholarAgent** — Automated Research Concierge (Kaggle Capstone scaffold)

## Overview

ScholarAgent is an AI-powered research orchestrator designed to automate the process of searching, synthesizing, and summarizing academic and technical content. This scaffold provides a foundation for building a production-ready research assistant using FastAPI, LLM integrations, and advanced memory management.

## Features

- **Orchestrator Agent**: Core research coordination engine
- **Stubbed Search Tool**: Ready for integration with real search APIs
- **Memory Adapter**: Persistent knowledge management
- **Summarizer Agent**: Content synthesis and summarization
- **Kaggle-Friendly Demo**: Runnable notebook without external API keys

## Quick Start

### Local Setup

```bash
# Clone the repository
git clone https://github.com/AnuvardhanKanuri/ScholarAgent.git
cd ScholarAgent

# Install dependencies
pip install -r backend/requirements.txt

# Run the FastAPI server
cd backend
uvicorn app.main:app --reload
```

### Run the Demo Notebook

```bash
jupyter notebook notebooks/demo.ipynb
```

## Architecture

```
ScholarAgent/
├── backend/
│   ├── app/
│   │   ├── main.py             # FastAPI entry point
│   │   ├── agents/
│   │   │   ├── orchestrator.py # Main research agent
│   │   │   ├── summarizer.py   # Content summarizer
│   │   │   └── search_tool.py  # Search integration (stubbed)
│   │   └── memory/
│   │       └── adapter.py      # Memory management
│   ├── requirements.txt
│   └── Dockerfile
├── notebooks/
│   └── demo.ipynb             # Kaggle-friendly demo
├── docs/
│   └── ARCHITECTURE.md
└── README.md
```

## Next Steps

- [ ] Integrate a real LLM provider (Gemini, OpenAI, Claude)
- [ ] Replace `SearchToolStub` with real web search/PDF pipeline
- [ ] Add secure sandboxed code runner microservice
- [ ] Implement authentication and rate limiting
- [ ] Deploy to cloud infrastructure

## Stubs & Placeholders

All external API calls are currently stubbed for a judges-friendly demo. See `backend/app/agents/README_STUBS.md` for detailed instructions to replace stubs with real providers.

## License

MIT

## Author

Anuvardhan Kanuri
