# Book Recommender System

A sophisticated book recommendation system that uses semantic search and machine learning to suggest books based on user queries, categories, and preferred reading tone. This implementation was inspired by the freeCodeCamp tutorial on building recommendation systems (https://www.freecodecamp.org/news/how-to-build-a-book-recommendation-system/)

## Features

- **Semantic Search**: Utilizes advanced NLP techniques to understand and match user queries with book descriptions
- **Category Filtering**: Filter recommendations by book categories
- **Tone-based Matching**: Find books that match your preferred reading tone
- **Rich Book Information**: Displays book covers, titles, authors, and truncated descriptions
- **Interactive Interface**: Built with Gradio for a user-friendly experience

## Dataset

The system uses the "7k Books with Metadata" dataset by Dylan Castillo from Kaggle (https://www.kaggle.com/datasets/dylanjcastillo/7k-books-with-metadata) that includes approximately 7,000 books with rich metadata such as:
- Book titles and authors
- Detailed book descriptions
- Categories and genres
- Cover image URLs
- Publication dates
- Ratings and reviews

## Technical Stack

### Core Dependencies
- Python >= 3.11
- Gradio >= 5.25.2 (Web Interface)
- LangChain (Semantic Search)
- CUDA PyTorch (Vector Operations)
- Pandas (Data Processing)
- Transformers (NLP Models)
- kagglehub (Dataset Management)
- langchain-community (LLM Integration)
- langchain-opencv (Image Processing)
- langchain-chroma (Vector Database)
- python-dotenv (Environment Management)

### Additional Libraries
- Hugging Face Hub integration
- Matplotlib & Seaborn for data visualization
- Jupyter Notebook support

## Setup

1. Clone the repository:
```bash
git clone [repository-url]
cd book-recommender
```

2. Set up the environment and install dependencies using UV (a modern Python package installer):
```bash
uv venv
source .venv/bin/activate  # On Unix/macOS
.venv\Scripts\activate     # On Windows
uv pip install .
```

3. Create a `.env` file with required API keys (if necessary)

## Usage

1. Start the Gradio interface:
```bash
python gradio-dashboard.py
```

2. Access the web interface through your browser (typically at `http://127.0.0.1:7860`)

3. Enter your query, select a category, and specify your preferred tone to get personalized book recommendations

## Data Exploration

The `data-exploration.ipynb` notebook contains detailed analysis of the book dataset, including:
- Data preprocessing steps
- Feature analysis
- Distribution of books across categories
- Rating patterns