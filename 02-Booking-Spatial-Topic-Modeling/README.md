# Topic Modeling and Spatial Analysis of Hotel Reviews

## Project Overview

This project combines Natural Language Processing (NLP) and spatial econometrics to analyze negative hotel reviews from Booking.com. The primary objective is to identify recurring themes in customer complaints and determine if these specific topics exhibit spatial patterns or clustering within urban environments. 

## Data

The dataset consists of negative hotel reviews enriched with geographical coordinates (latitude and longitude). 

The analysis focuses on hotels located across six major European tourist destinations:
* Amsterdam
* Barcelona
* London
* Milan
* Paris
* Vienna

## Methodology

This project integrates text mining with geospatial analysis to uncover location-based insights from textual data.

### 1. Text Mining & Topic Modeling

* **Text Preprocessing:** Tokenization and removal of domain-specific stopwords to clean the review data.
* **Topic Extraction:** Multiple algorithms were implemented and compared to extract latent topics from the corpus of reviews:
  * Latent Dirichlet Allocation (LDA)
  * Non-Negative Matrix Factorization (NMF)
  * BERTopic (Transformer-based modeling)

### 2. Spatial Analysis

* **Distance Calculation:** Utilized the Haversine formula to calculate the exact distance between individual hotels and their respective city centers.
* **Spatial Autocorrelation:** Applied Moran's I and Local Indicators of Spatial Association (LISA) to detect spatial clustering of specific complaint topics.
* **Clustering:** Implemented K-Means clustering based on the combination of distance to the city center and the dominant topic of the hotel.
* **Geospatial Visualization:** Mapped the findings using GeoPandas and Plotly to create interactive, visual representations of topic distributions across the cities.

## Key Insights

* The analysis reveals how specific types of complaints (e.g., noise, room size, facilities) are distributed spatially across different city zones.
* Provides a framework for understanding whether proximity to the city center correlates with specific categories of negative guest experiences.