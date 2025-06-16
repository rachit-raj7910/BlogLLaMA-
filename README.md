# BlogLLaMA
# 📝 AI Blog Generator with LLaMA 2

This is a **Streamlit-based web app** that generates blog posts using the **LLaMA 2 model**. Users can input a topic, choose a blog style, and set the word count — and the app will generate a professional, casual, humorous, or technical blog post using the LLaMA 2 language model.

## Features

- Generate blog posts on any topic
- Choose word count (50–2000)
- Select tone/style: Professional, Casual, Humorous, Technical
- Runs locally using the `llama-2-7b-chat.ggmlv3.q8_0.bin` model
- Clean and interactive Streamlit UI

##  How It Works
1. The user enters:
   - A topic
   - Number of words
   - Blog style
2. The app uses a LLaMA 2 model (via `ctransformers`) to generate a coherent blog post
3. The response is displayed in the Streamlit interface with the option to download the result

##  File Structure
```
Blog-generation-app/
│
├── model/
│   ├── llama_model.py                     # Model logic (loads and queries LLaMA 2)
│   └── llama-2-7b-chat.ggmlv3.q8_0.bin    # The quantized LLaMA 2 model file
│
├── Blog.py                                 # Main Streamlit application script
│
├── requirements.txt                       # Required Python packages
│
└── README.md                              # Project documentation (this file)




## Prerequisites
- Python 3.8 or higher (3.10.0 used by me)
- Streamlit
- langchain
- ctransformers

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

## Contributing
We welcome contributions to improve this project! Whether it's fixing a bug, improving performance, or adding a new feature — your help is appreciated.

