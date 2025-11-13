🎬 CineVector – Semantic Movie Recommender

CineVector is an AI-powered semantic movie recommendation system that understands meaning, emotion, and genre — not just keywords.

Using vector embeddings, semantic similarity search, and an elegant Gradio dashboard, CineVector recommends movies based on natural-language user queries such as:

“A movie about deep friendship and survival”
“Something funny with a happy ending”
“A dark mystery detective story”


---

## 🚀 Features

- 🔎 **Semantic search** — Natural-language queries (not keyword matching)  
- 🎭 **Emotion-aware sorting** — Filter/sort by `joy`, `sadness`, `fear`, `anger`, `surprise`  
- 🗂️ **Genre filtering** — Simple genre buckets (e.g., Fiction / Non-Fiction)  
- 🖼️ **Poster gallery** — TMDB posters or a fallback **Poster Not Found** image  
- ⚡ **Fast & cost-efficient** — Embeddings persisted locally so runtime queries do **not** use OpenAI credits

---

## 🗂️ Project structure
- CineVector/
- │
- ├── **chroma_db/**                     # Saved vector embeddings (DO NOT DELETE)
- │   ├── index/
- │   ├── collections/
- │   └── uuid-xxx/
- │
- ├── **data/**
- │   ├── movies_with_posters.csv        # Dataset with posters & metadata
- │   ├── tagged_overview.txt            # Overview text used for embeddings
- │   └── poster_not_found.png           # Fallback poster image
- │
- ├── **dashboard.py**                   # Gradio movie recommendation app
- ├── **requirements.txt**               # Python dependencies
- ├── **README.md**                      # Documentation
- └── **.env**                           # API keys (ignored in Git)

---

