# BlogLLaMA
# 📝 AI Blog Generator with LLaMA 2

This is a **Streamlit-based web app** that generates blog posts using the **LLaMA 2 model**. Users can input a topic, choose a blog style, and set the word count — and the app will generate a professional, casual, humorous, or technical blog post using the LLaMA 2 language model.

 **Generates blogs on any topic with a specified word count and audience tone.**
![Screenshot 2025-06-16 141711](https://github.com/user-attachments/assets/0c08753c-469a-41c0-bcdb-504d52ba58f5)
 **Generates blog posts on any topic — from deeply technical to hilariously relatable**
![Screenshot 2025-06-16 142650](https://github.com/user-attachments/assets/07dc13ae-6c77-4c1d-83f9-cd8a6111b6b5)

![Screenshot 2025-06-16 143204](https://github.com/user-attachments/assets/9050d6a2-fca1-4d71-9147-9b6e7140060b)

## Features
- Generate blog posts on any topic
- Choose word count (50–2000)
- Select tone/style: Professional, Casual, Humorous, Technical
- Runs locally using the `llama-2-7b-chat.ggmlv3.q8_0.bin` model
- Clean and interactive Streamlit UI
  
**It can even generate casual blogs with a relaxed, conversational tone**
  ![Screenshot 2025-06-16 142230](https://github.com/user-attachments/assets/3bf9d80b-f4aa-4327-942e-498e19f3c371)

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
```
## Prerequisites
- Python 3.8 or higher (3.10.0 used by me)
- Streamlit
- langchain
- ctransformers
  
## Model Set-up
This project uses the `llama-2-7b-chat.ggmlv3.q8_0.bin` model — a quantized version of Meta's LLaMA 2 with 7 billion parameters — to generate high-quality, contextually relevant blog content. To set it up, simply download the model file from [Hugging Face](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main), place it in the `models/ directory`, and ensure your code points to `models/llama-2-7b-chat.ggmlv3.q8_0.bin`. The `ggmlv3.q8_0` variant is optimized for efficiency, offering reduced memory usage, faster execution on local machines, and strong performance without requiring a GPU — making it ideal for fast, local blog generation tasks.


## Usage
To use the blog generator, simply run `streamlit run Blog.py` from the project directory. The Streamlit interface will open in your browser, where you can enter a blog topic, specify the desired word count, and select the target blog style from a dropdown menu (such as Professional, Casual, Technical and Humorous). Once you click the "Generate" button, the application will process your input using the LLaMA 2 model and display a complete blog post tailored to your preferences — right on the screen.

## Contributing
We welcome contributions to improve this project! Whether it's fixing a bug, improving performance, or adding a new feature — your help is appreciated.

