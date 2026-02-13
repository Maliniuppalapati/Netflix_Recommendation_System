🎬 Netflix Recommendation System
Personalized Movie & TV Show Discovery Engine

📌 Overview
This project implements a Content-Based Recommendation System that suggests media based on metadata similarity. By processing 8,800+ records, the engine identifies the "closest" titles using text vectorization and spatial geometry.

🚀 Key Features
Metadata-Based Filtering: Analyzes titles, genres, and descriptions to find hidden relationships between shows.

Performance Boost: Utilizes NumPy vectorization to reduce query latency by ~30%, ensuring fast responses for large datasets.

Interactive EDA: Features interactive visualizations of content distributions and ratings using Plotly and Seaborn.

WordCloud Analytics: Visualizes high-frequency keywords to understand Netflix's content trends.

🛠️ Technical Implementation
1. Data Processing
Missing Value Handling: Replaced nulls in critical columns (Director, Cast) with "Unknown" to maintain dataset integrity.

Feature Engineering: Combined multiple metadata fields into a single "Combined Features" string to capture maximum context.

2. The NLP Pipeline
TF-IDF Vectorization: Converted text descriptions into a numerical matrix, highlighting rare but meaningful words.

Cosine Similarity: Calculated the cosine of the angle between vectors to determine similarity, regardless of text length.

📂 Project Structure
Plaintext
Netflix-Recommendation-System/
├── netflix_data.csv          # 8,807 Movies & TV Shows records
├── netflix_recommender.ipynb # Complete analysis & logic
├── requirements.txt          # Dependency list (Pandas, Scikit-learn, etc.)
└── README.md                 # Project documentation
📊 Sample Output
Top-5 Recommendations for "Kota Factory":

Cheese in the Trap

Criminal Minds

Single Ladies Senior

The Great Train Robbery

The Politician
(Results based on genre and thematic description matches)

💻 How to Run
Clone: git clone https://github.com/your-username/Netflix-Recommender.git

Install: pip install -r requirements.txt

Run: Open netflix_recommender.ipynb in Jupyter and execute all cells.

📈 Future Enhancements
[ ] Hybrid Filtering: Combine content-based results with user rating data.

[ ] Weighting: Apply higher weights to "Title" and "Genre" vs "Description" for better accuracy.

[ ] Web Deployment: Create a real-time recommendation interface using Streamlit.
