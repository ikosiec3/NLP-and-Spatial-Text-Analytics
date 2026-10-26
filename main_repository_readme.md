# NLP and Spatial Text Analytics


This repository showcases projects where I apply advanced text mining, natural language processing (NLP), machine learning, and spatial econometrics to extract actionable business insights from unstructured customer review data.

##  Repository Structure

This repository contains two main projects, organized into separate directories:

### [1. Disneyland Reviews Sentiment Analysis](./01-Disneyland-Sentiment-Analysis)
* **Goal:** To analyze visitor satisfaction and sentiment across different global Disneyland locations using unstructured review data.
* **Key Techniques:** Text preprocessing, Sentiment Analysis (VADER, SentiWordNet), Transformer models (BERT), Supervised Machine Learning (Logistic Regression, SVC, XGBoost), and TF-IDF.
* **Highlights:** Evaluated multiple ML models to predict review ratings based on textual features, addressing dataset imbalances and identifying location-specific pain points.

### [2. Booking.com Spatial Topic Modeling](./02-Booking-Spatial-Topic-Modeling)
* **Goal:** To identify latent topics in negative hotel reviews and analyze their spatial distribution and clustering across popular European tourist cities.
* **Key Techniques:** Topic Modeling (LDA, NMF, BERTopic), Spatial Econometrics (Moran's I, LISA), K-Means Clustering, Haversine Distance, and Geospatial Data Visualization (GeoPandas, Plotly).
* **Highlights:** Combined NLP with geographic coordinates to uncover how specific customer complaints (e.g., noise, room size) correlate with a hotel's distance from the city center.

## ️ Technologies & Libraries Used
Across these projects, I utilized a variety of tools and libraries:
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **NLP:** NLTK, Scikit-learn, Transformers (Hugging Face), BERTopic, Gensim
* **Machine Learning:** Scikit-learn, XGBoost
* **Spatial & Geospatial:** GeoPandas, PySAL, Plotly, Haversine
* **Visualization:** Matplotlib, Seaborn, WordCloud

##  How to Navigate
Feel free to explore the individual project folders. Each folder contains its own `README.md` with a detailed explanation of the dataset, methodology, and key findings, along with the source code and visual exports.