```
project-root/
├── app/
│   ├── __init__.py
│   ├── main.py                # FastAPI app instance & server startup
│   ├── api/
│   │   ├── __init__.py
│   │   └── routes.py          # API endpoints (input handling, response generation)
│   ├── core/
│   │   ├── __init__.py
│   │   └── config.py          # Configuration settings (e.g., Hugging Face API token)
│   ├── models/
│   │   ├── __init__.py
│   │   └── schemas.py         # Pydantic models for request/response validation
│   ├── services/
│   │   ├── __init__.py
│   │   ├── article_extractor.py   # Fetches, parses & cleans article content using BeautifulSoup
│   │   ├── agent_summarization.py # Summarization agent using LangChain
│   │   ├── agent_analysis.py      # Analysis agent to extract key arguments and assumptions
│   │   ├── agent_counter.py       # Counter-perspective agent generating the opposite view
│   │   └── llm_integration.py     # Integration of Hugging Face Inference API with LangChain
│   ├── utils/
│   │   ├── __init__.py
│   │   └── helpers.py         # Utility functions (logging, error handling, etc.)
├── tests/
│   ├── __init__.py
│   ├── test_article_extractor.py  # Unit tests for article extraction logic
│   ├── test_agents.py             # Tests for summarization, analysis & counter agents
│   ├── test_routes.py             # Tests for FastAPI routes/endpoints
│   └── test_llm_integration.py    # Tests for the Hugging Face API integration
├── requirements.txt           # Project dependencies (FastAPI, LangChain, BeautifulSoup, etc.)
├── README.md                  # Project documentation & setup instructions
└── .env                       # Environment variables (e.g., Hugging Face API token)


```