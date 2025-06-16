# BlogLLaMA-
# 📝 AI Blog Generator with LLaMA 2

This is a **Streamlit-based web app** that generates blog posts using the **LLaMA 2 model**. Users can input a topic, choose a blog style, and set the word count — and the app will generate a professional, casual, humorous, or technical blog post using the LLaMA 2 language model.

---

## 🚀 Features

- Generate blog posts on any topic
- Choose word count (50–2000)
- Select tone/style: Professional, Casual, Humorous, Technical
- Runs locally using the `llama-2-7b-chat.ggmlv3.q8_0.bin` model
- Clean and interactive Streamlit UI

---

## 🧠 How It Works

1. The user enters:
   - A topic
   - Number of words
   - Blog style
2. The app uses a LLaMA 2 model (via `ctransformers`) to generate a coherent blog post
3. The response is displayed in the Streamlit interface with the option to download the result

---

## 📦 File Structure
Blog/
├── Blog.py
├── model/
│   ├── llama_model.py
│   └── llama-2-7b-chat.ggmlv3.q8_0.bin


---

## 🛠️ Prerequisites

- Python 3.8+
- [Anaconda](https://www.anaconda.com/products/distribution) or virtualenv
- Internet (for initial model download/setup)

---

## 🔧 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/blog-generator-llama2.git
cd blog-generator-llama2

# Create virtual environment
conda create -n bloggen python=3.9
conda activate bloggen

# Install dependencies
pip install -r requirements.txt

