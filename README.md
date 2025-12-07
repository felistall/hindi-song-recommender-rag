# ***🎶 Hindi Songs Recommendation System (RAG + Hugging Face + BGE)***

**A Retrieval-Augmented Generation (RAG) based Hindi Songs Recommender that combines semantic search, cosine similarity, BGE-M3 embeddings, and Hugging Face LLMs to suggest Bollywood songs based on the user’s mood, genre, tempo, and vibe.**

**📌 Features**

🎧 100+ curated Bollywood songs dataset (genre, mood, decade, tempo)
🔍 BGE-M3 semantic embeddings for high-quality retrieval
📐 Cosine similarity search for top-K matches
🧠 RAG pipeline with Hugging Face LLM (Mistral / Falcon / Flan T5)
🚀 Fully Colab-ready — no paid APIs required
🎤 Mood-based, genre-based, decade-based recommendations
🧱 Modular architecture (load → embed → retrieve → RAG generation)

**🛠 Tech Stack**

Component	Technology
Embeddings	BGE-M3 (FlagEmbedding)
LLM	Hugging Face Transformers (Mistral / Falcon / Flan-T5)
Retrieval	Cosine Similarity (sklearn)
Dataset	Custom curated Bollywood songs CSV
Runtime	Google Colab GPU

**▶️ How to Run**
1. Run the Colab Notebook
Open main.ipynb
Upload the dataset
Run all cells

**🤖 How The System Works**
Step 1 — Dataset Loading
Loads metadata for 100+ Hindi songs
(title, artist, genre, mood, decade, tempo, tags)

Step 2 — Embedding Generation
Uses BGE-M3 to create a dense vector for each song.

Step 3 — Retrieval
Cosine similarity finds top-K semantically similar songs.

Step 4 — RAG Prompting
A Hugging Face LLM reasons over retrieved results and generates recommendations.

Step 5 — User Output
A clean, natural-language list of recommendations.

**🧪 Example Queries**
Try:
"romantic slow heartbreak from 2010s"
"energetic dance song for party"
"emotional patriotic Bollywood song"
"classic old Hindi romantic songs"

**📊 Dataset Overview**
100 Bollywood songs
Features:
title
artist
movie
year, decade
genre, mood, tempo
tags (combined features)
Clean, training-ready format

**📝 Roadmap**

 Add UI using Streamlit / Gradio
 Add audio feature extraction (MFCC, BPM)
 Add real lyrics scraping (Genius / Musixmatch API)
 Add Spotify-based audio features
 Deploy to Hugging Face Spaces

**🤝 Contributing**

Pull requests, issues, and suggestions are welcome!

**⭐ Show Support**
If you like this project, consider giving it a ⭐ on GitHub.
Your support motivates more open-source Bollywood + AI projects!
