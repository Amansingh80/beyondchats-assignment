# NodeJS LLM Script

## Setup Instructions

```bash
npm install
cp .env.example .env
# Add your API keys to .env
node index.js
```

## Features
- Fetches articles from Laravel API
- Google Search integration
- Web scraping of top-ranking articles
- LLM-based content optimization
- Automatic article publishing

## Environment Variables
```
LARAVEL_API_URL=http://localhost:8000/api
OPENAI_API_KEY=your_key_here
GOOGLE_API_KEY=your_key_here
```