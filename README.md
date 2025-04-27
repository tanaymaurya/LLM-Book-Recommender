# LLM-Book-Recommender

## Description

This project provides a **book recommendation system** using **Large Language Models (LLMs)**, **emotional tone analysis**, and a **Gradio dashboard** for interactive user experience. The system uses a dataset of 7,000 books from Kaggle to provide book recommendations based on user preferences, emotional tone, and genre.

### Dataset Used:
- **[7K Books with Metadata Dataset](https://www.kaggle.com/datasets/dylanjcastillo/7k-books-with-metadata)**
  - This dataset contains metadata for 7,000 books, including titles, authors, genres, descriptions, and more.

## Features

- **Text Data Cleaning:**  
  - Code for cleaning the text data is available in the notebook `data-exploration.ipynb`.
  
- **Semantic (Vector) Search:**  
  - Built a vector search system and a vector database, allowing users to find similar books based on a natural language query.  
  - Code in the notebook `vector-search.ipynb`.
  
- **Text Classification:**  
  - Applied **zero-shot classification** using LLMs to classify books into categories like "fiction" or "non-fiction".  
  - Code in the notebook `text-classification.ipynb`.

- **Sentiment Analysis & Emotional Tone Extraction:**  
  - Used LLMs to analyze the sentiment and emotional tone of book descriptions (e.g., suspenseful, joyful, sad).  
  - Code in the notebook `sentiment-analysis.ipynb`.

- **Gradio Web Application:**  
  - Created a user-friendly web app using Gradio where users can input book descriptions and get recommendations based on their emotional tone and category preferences.  
  - Code in `gradio-dashboard.py`.

## ⚙️ Tech Stack

| Tool / Library             | Purpose                                      |
|----------------------------|----------------------------------------------|
| **Python**                 | Core programming language                    |
| **pandas & numpy**         | Data handling & manipulation                 |
| **transformers**           | Emotion classification model                 |
| **langchain**              | Document management & retrieval              |
| **OpenAIEmbeddings**       | Embedding generation                         |
| **Chroma**                 | Vector similarity database                   |
| **Gradio**                 | Frontend UI                                  |
| **dotenv**                 | Secure environment config                    |
| **requests**               | API requests                                 |
| **json**                   | Data serialization                           |
| **PyCharm**                | IDE for development                          |

## 💻 How to Run

### 1. Clone the repository:
```bash
git clone https://github.com/tanaymaurya/LLM-Book-Recommender.git
cd LLM-Book-Recommender
```
### 2. Install dependencies:
```
pip install -r requirements.txt
```
3. Set up environment variables:

    Create a .env file in the root directory of the project.

    Add your OpenAI API key to the .env file:
```
OPENAI_API_KEY=your_openai_key
```
4. Run the app:
```
python gradio-dashboard.py
```

5. Input your preferences:

    Enter a book description, select an emotional tone, and choose a category to get recommendations.

6. Explore the results:

    Browse through the recommended books and their details.

    Enjoy discovering your next favorite book with our LLM-powered recommendation system!

📑 Acknowledgements

HuggingFace: For the Transformers library and pre-trained models.

   Langchain: For document management and integration with language models.

   OpenAI: For providing powerful language models.

   ChromaDB: For vector database management.

   Gradio: For building the user interface.
