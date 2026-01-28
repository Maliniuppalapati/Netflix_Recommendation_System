# 🎬 Netflix Recommendation System & EDA

An end-to-end Data Science project that analyzes the Netflix dataset and implements a **Content-Based Filtering** recommendation engine. The system suggests similar movies and TV shows based on titles, genres, and plot descriptions.

## 🚀 Live Demo
**[Insert your GitHub Pages Link Here]**

---

## 📊 Project Overview
This project is divided into two main parts:
1.  **Exploratory Data Analysis (EDA):** Visualizing content distribution by country, rating, release year, and duration using `Plotly`, `Seaborn`, and `WordClouds`.
2.  **Recommendation Engine:** A recommendation system built using **Natural Language Processing (NLP)** to calculate similarity between titles.

## ✨ Key Features
* **Automated Data Cleaning:** Handles missing values for directors, cast, and countries.
* **Interactive Visualizations:** * **Choropleth Maps:** Visualizing content production by country.
    * **Pie & Bar Charts:** Distribution of Movies vs. TV Shows.
    * **Word Clouds:** Most frequent terms in Netflix titles and descriptions.
* **Content-Based Recommender:** Uses **TF-IDF Vectorization** and **Cosine Similarity** to recommend the top 10 most relevant titles based on a user's input.

## 🛠️ Tech Stack
* **Language:** Python
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn, Plotly, WordCloud
* **Machine Learning:** Scikit-Learn (TfidfVectorizer, Cosine Similarity)

## ⚙️ How the Recommendation Works
The system uses the following mathematical approach to find similar content:

1.  **Feature Combination:** Combines `title`, `listed_in` (genres), and `description` into a single string.
2.  **TF-IDF Vectorization:** Converts text data into a numerical matrix representing word importance.
3.  **Cosine Similarity:** Calculates the cosine of the angle between two vectors to determine how similar they are. 

$$\text{similarity} = \cos(\theta) = \frac{A \cdot B}{\|A\| \|B\|}$$

## 📖 How to Use
1.  Ensure you have the `netflix_data.csv` file in your directory.
2.  Run the Jupyter Notebook or Python script.
3.  Use the function `recommend_movies("Title Name")` to get instant suggestions.
    * *Example:* `recommend_movies("Kota Factory")`

---

## 👤 Author
**Geya Malini Uppalapati**
*Computer Science Student & Data Science Enthusiast*

---
*This project was developed to demonstrate skills in data preprocessing, visualization, and building recommendation systems.*
