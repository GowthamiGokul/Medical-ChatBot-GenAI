
---

### 🖥️ Bash Script to Generate the `README.md`

Save the following as `generate_readme.sh`:

```bash
#!/bin/bash

cat << 'EOF' > README.md
# CAREPAL: AI-Driven Health & Activity Partner

## 🧠 Problem Statement
Many individuals struggle to navigate overwhelming and often conflicting online health information. CAREPAL addresses this by delivering **personalized, evidence-based wellness guidance** through a chatbot that simplifies medical content into actionable lifestyle recommendations.

## 🚀 Project Overview
CAREPAL is a generative AI-powered chatbot that provides health and wellness recommendations based on reliable guidelines from the **WHO**, **CDC**, and **US Department of Health Services**. It uses the **Llama 2 language model** and semantic search to deliver context-aware, non-diagnostic advice.

## ⚙️ Steps to Run the Project

### 1. Create a Conda Environment
\`\`\`bash
conda create -n mchatbot python=3.8 -y
\`\`\`

### 2. Activate the Conda Environment
\`\`\`bash
conda activate mchatbot
\`\`\`

### 3. Install the requirements
\`\`\`bash
pip install -r requirements.txt
\`\`\`

### 4. Add Pinecone credentials to \`.env\` file
\`\`\`ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
\`\`\`

### 5. Download the Llama 2 Model
Download and place the following model file in the \`model\` directory:
- \`llama-2-7b-chat.ggmlv3.q4_0.bin\`  
From: [HuggingFace - TheBloke](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main)

## 📦 Description
This project demonstrates the creation of an end-to-end medical chatbot using Llama 2. It retrieves and answers medical queries based on contextually relevant data.

## 🧰 Prerequisites
- Python 3.8
- Conda
- API Keys for Pinecone & OpenAI
- Internet access to download model files

## ▶️ How to Use
1. Follow the setup instructions above.
2. Run the main script (e.g., \`app.py\`) from the project root directory.

---

## 🛠️ Tech Stack

| Layer           | Technologies Used              |
|----------------|----------------------------------|
| Frontend       | React.js                         |
| Backend        | Flask (Python)                   |
| LLM            | Meta's Llama 2                   |
| Embeddings     | OpenAI Embedding Models          |
| Vector DB      | Pinecone                         |
| NLP Libraries  | SpaCy, NLTK                      |
| Deployment     | Localhost / Streamlit (optional) |

---

## 📚 Dataset Sources

- [WHO Guidelines on Physical Activity](https://apps.who.int/iris/bitstream/handle/10665/336656/9789240015128-eng.pdf)
- [CDC Physical Activity Guidelines](https://health.gov/sites/default/files/2019-09/Physical_Activity_Guidelines_2nd_edition.pdf)
- Dietary Guidelines for Americans 2020–2025
- Curated health and wellness datasets

---

## 🧩 Approach Used

1. **Text Preprocessing**: Chunk documents (~200 tokens) while preserving context.
2. **Embedding Generation**: Convert chunks using OpenAI’s embedding models.
3. **Semantic Indexing**: Store embeddings in Pinecone for similarity-based retrieval.
4. **Query Resolution**: Retrieve relevant chunks, pass to Llama 2 for response generation.
5. **Integration**: Built end-to-end pipeline with Flask backend + React frontend.

---

## 🧠 Model Information

- **Llama 2-7B Chat** (quantized version)
- Context window: 4096 tokens
- Conversational, RAG-based response generation
- Non-diagnostic, privacy-respecting recommendations

---

## 📊 Application Results

- Response time: ~2 seconds
- Highly personalized guidance based on user input
- Adheres to public health recommendations

---

## 🧱 Application Architecture

> 📌 *Paste architecture diagram image here*

---

## 📈 Future Enhancements

- Support for multiple languages
- Integration with wearables (e.g., Fitbit, Apple Health)
- Expansion to cover more health topics
- Real-time mood and sentiment tracking

---

## 👨‍💻 Author

- Dhyey Joshi  
> Sponsored by **Crisis Technologies Innovation Lab** – Fall 2024

## 📝 License

This project is licensed under the [MIT License](LICENSE).
