Amazon Apparel Recommendation System

This project implements an Amazon Apparel Recommendation System using data analysis and machine learning techniques. The goal is to create personalized apparel recommendations based on product data provided by Amazon.

Overview

The dataset consists of product information from Amazon's apparel category, including details such as unique identifiers, brands, colors, product types, prices, and more. The project involves data preprocessing, exploration, and the development of a recommendation system using similarity metrics.

Dataset Description

The dataset (tops_fashion.json) contains 183,138 data points and 19 features. For this project, six key features were used:

asin: Amazon Standard Identification Number
brand: Brand of the product
color: Color(s) of the apparel (e.g., "red and black stripes")
product_type_name: Type of apparel (e.g., "SHIRT", "TSHIRT")
medium_image_url: URL of the product image
title: Product title
formatted_price: Price of the product
Key Steps and Findings

Data Exploration and Preprocessing:
Reduced the dataset to 28,385 data points after filtering for non-null price and color information.
Removed products with short titles or duplicate entries.
Product Insights:
Most frequent product type: SHIRT (91.62% of data).
Most common color: Black (7.2% of products).
Price data was available for 15.5% of the products.
Final Dataset:
Cleaned dataset with 27,949 data points.
Saved intermediate and final datasets as pickle files.


Methodology

Libraries Used:
Data Handling and Analysis: pandas, numpy
Data Visualization: matplotlib, seaborn, plotly
Text Processing: nltk, BeautifulSoup
Machine Learning: scikit-learn
Preprocessing Steps:
Loaded dataset using pandas.read_json.
Cleaned missing, inconsistent data and removed duplicates.
Filtered relevant features for analysis and saved intermediate datasets.
Recommendation System:
Implemented similarity-based recommendations using:
CountVectorizer
TfidfVectorizer
Cosine similarity metrics
Visualization and Insights
Distribution of product types, brands, and colors.
Price analysis for identifying trends.
Insights from frequent titles and keywords.


How to Run the Project

Clone the repository:
git clone <repository_url>
Install required dependencies:
pip install -r requirements.txt
Place the tops_fashion.json file in the project directory.
Run the Jupyter Notebook or Python script to analyze the data and generate recommendations.
Future Work


Integrate additional features from the dataset.
Experiment with advanced recommendation techniques like collaborative filtering.
Deploy the recommendation system as a web application.
Acknowledgments


Inspired by the Applied AI Workshop.
Thanks to Amazon for providing the dataset used in this analysis.