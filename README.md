🎬 CineVector – Semantic Movie Recommender

CineVector is an AI-powered semantic movie recommendation system that understands meaning, emotion, and genre — not just keywords.

Using vector embeddings, semantic similarity search, and an elegant Gradio dashboard, CineVector recommends movies based on natural-language user queries such as:

“A movie about deep friendship and survival”
“Something funny with a happy ending”
“A dark mystery detective story”

🚀 Features
🔍 Semantic Search

CineVector uses OpenAI embeddings and ChromaDB to find movies based on the meaning of your query.

🎭 Emotion-Aware Filtering

Recommendations can be sorted by emotional tones:

Happy

Sad

Suspense

Angry

Surprising

🎬 Genre-Based Filtering

Filter by simplified genres:

Fiction

Non-Fiction

🖼️ High-Quality Posters

Each movie displays its poster using TMDB image base URLs.
Missing posters are replaced with a custom “Poster Not Found” image.

⚡ Fast Performance

All embeddings are pre-computed and stored locally, so no OpenAI API calls occur during recommendation — fast & cost-free.

🌐 Easy-to-use Dashboard

Powered by Gradio, offering:

Search box

Dropdowns for genre & tone

A gallery of poster-based recommendations
---
##🏗️ Tech Stack
Component	Technology
Vector Search	ChromaDB
Embeddings	OpenAI Embeddings
UI	Gradio
Data Processing	Pandas, NumPy
Backend	Python
Posters	TMDB image URLs
Environment	.env for API keys
---
##📁 Project Structure
CineVector/
│
├── **chroma_db/**                     # Saved vector embeddings (DO NOT DELETE)
│   ├── index/
│   ├── collections/
│   └── uuid-xxx/
│
├── **data/**
│   ├── movies_with_posters.csv        # Dataset with posters & metadata
│   ├── tagged_overview.txt            # Overview text used for embeddings
│   └── poster_not_found.png           # Fallback poster image
│
├── **dashboard.py**                   # Gradio movie recommendation app
├── **requirements.txt**               # Python dependencies
├── **README.md**                      # Documentation
└── **.env**                           # API keys (ignored in Git)

---

