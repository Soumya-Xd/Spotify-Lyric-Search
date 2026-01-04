# 🎵 Spotify Lyric Search – Semantic ML Model

Spotify Lyric Search is an **AI-powered semantic search system** that identifies songs based on **lyric snippets** using **Sentence-BERT (SBERT)** instead of traditional keyword matching.

The system understands the **meaning of lyrics**, allowing users to find songs even when the lyrics are **incomplete, paraphrased, or slightly incorrect**.

---

## 🚀 Project Highlights

- Semantic lyric-based song search
- Uses **Sentence-BERT (all-MiniLM-L6-v2)**
- Cosine similarity for ranking results
- Handles partial and noisy lyric inputs
- Interactive command-line search
- Saves embeddings for faster reuse
- Fully runnable on **Google Colab**

---

## 🧠 How It Works

1. Lyrics are cleaned and preprocessed
2. Each song lyric is converted into a **vector embedding** using SBERT
3. User-input lyric snippets are encoded using the same model
4. **Cosine similarity** is calculated between query and dataset embeddings
5. Top matching songs are returned with confidence scores

---

## 🛠 Tech Stack

- **Python**
- **Sentence-Transformers (SBERT)**
- **Hugging Face Transformers**
- **PyTorch**
- **scikit-learn**
- **NumPy & Pandas**

---


---

## ▶️ Run on Google Colab (Recommended)

You can directly run this project using the Colab notebook below:

🔗 **Colab Notebook Link**  
👉 https://colab.research.google.com/drive/10xriU-3kSHiFxdoTL0jDJzwG4lknpZx7?usp=sharing

No local setup required.

---

## ⚙️ Installation (Local / Colab)

```bash
pip uninstall -y torch transformers huggingface_hub sentence-transformers accelerate
pip install torch==2.9.0 --no-cache-dir
pip install huggingface_hub==0.21.0 --no-cache-dir
pip install transformers==4.35.2 --no-cache-dir
pip install sentence-transformers==2.2.2 --no-cache-dir

