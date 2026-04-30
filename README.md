# Yelp Restaurant Rating Predictor
**Project Type:** Machine Learning & Natural Language Processing (NLP)  
**Academic Context:** MBA in Market Research Insights & Analytics (Predictive Modeling Coursework)

## 📌 Executive Summary
This project addresses the challenge of quantifying subjective user experiences. By processing the Yelp Open Dataset, I developed a machine learning pipeline that predicts restaurant star ratings by integrating business metadata with NLP-derived sentiment scores from customer reviews.

Metric: Mean Absolute Error (MAE) of 0.6730 stars.

Technical Stack: Python, Scikit-Learn (Linear Regression), TF-IDF Vectorization.

Scale: Successfully processed a 50,000-row subset of the 5GB+ Yelp Open Dataset using chunking for memory efficiency.

## 🏗️ System Architecture
The pipeline follows a standard ETL (Extract, Transform, Load) and Modeling pattern:
1. **Data Ingestion:** Processed large-scale JSON objects using Python (Pandas/NumPy).
2. **Text Processing:** Utilized NLTK for tokenization, stop-word removal, and sentiment polarity scoring.
3. **Feature Engineering:** Combined numerical business attributes (e.g., price range, check-ins) with text-based sentiment features.
4. **Modeling:** Trained and tuned a Random Forest Regressor to handle non-linear relationships in the data.



## 🚀 Key Technical Challenges
* **Unstructured Data at Scale:** Managed multi-gigabyte JSON files by implementing data chunking and filtering to isolate relevant business categories.
* **Sentiment Nuance:** Improved model accuracy by weighting recent reviews more heavily than older ones, accounting for "service drift."

## 📈 Impact & Results
* Achieved a predictive accuracy within a 0.673-star margin.
* Identified "Review Sentiment" as the primary driver of rating variance, outweighing physical business attributes.
