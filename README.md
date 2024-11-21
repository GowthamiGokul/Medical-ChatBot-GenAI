
# A Generative AI Health and Wellness Chatbot

## Steps to Run the Project

### 1. Create a Conda Environment
```bash
conda create -n mchatbot python=3.8 -y
```

### 2. Activate the Conda Environment
```bash
conda activate mchatbot
```
### 3. Install the requirements

```bash
pip install -r requirements.txt
```

### Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```
### Download the quantized model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin

## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main

```

## Description
This project demonstrates the creation of an end-to-end medical chatbot using Llama2. The chatbot leverages advanced language models to retrieve and answer medical queries based on contextually relevant data.

## Prerequisites
- Python 3.8
- Conda
- Access to required API keys (Pinecone, OpenAI)
- Additional dependencies installed in the created environment

## Usage
1. Follow the steps above to set up the environment.
2. Run the project script as described in the project documentation or scripts folder.

## License
This project is licensed under the [MIT License](LICENSE).

## Author
Dhyey
