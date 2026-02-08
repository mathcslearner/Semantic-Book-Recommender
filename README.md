# Semantic Book Recommender

A Python-based book recommendation system that uses semantic embeddings to suggest books based on meaning and emotions. The technologies used in this project are Python, OpenAI, LangChain, HuggingFace and Gradio.

## How It Works

1. Text data is cleaned and processed using pandas
2. Books are classified into "fiction" vs "non-fiction" using zero-shot classification in LLMs
3. Sentiment analysis is run on book descriptions using LLMs, extracting the most prominent emotions from text
4. Books are stored in a vector database where semantic search is applied to find the most similar books to a natural language query
5. The final step is a web application using Gradio for users to get book recommendations

## Installation

### Prerequisites

- Python 3.9 or higher
- pip
- Git

### Clone the repository

```bash
git clone https://github.com/mathcslearner/Semantic-Book-Recommender.git
cd Semantic-Book-Recommender
```

### Install dependencies

In order to run the project, the following dependencies are required:

- pandas
- numpy
- python-dotenv
- langchain-community
- langchain-opencv
- langchain-chroma
- transformers
- gradio

### Environment variables

Create a .env file in the project with your own OpenAI API key:

```env
OPENAI_API_KEY=your_api_key_here
```

### CLI Usage

```bash
python gradio-dashboard.py
```