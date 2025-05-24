New York Airbnb EDA Project

Project Overview

This project conducts an Exploratory Data Analysis (EDA) on Airbnb listings in New York City to uncover patterns and relationships between variables such as price, room type, neighborhood, and guest reviews. The analysis aims to provide insights into the Airbnb market, including pricing trends, listing characteristics, and host activity.

Dataset





Source: The dataset is stored in datasets.csv and contains information about Airbnb listings in New York City.



Columns: 22 columns, including:





id, name, host_id, host_name



neighbourhood_group (e.g., Brooklyn, Manhattan), neighbourhood (e.g., Clinton Hill, Hell's Kitchen)



latitude, longitude for geographic analysis



room_type (e.g., Private room, Entire home/apt), price, minimum_nights



Review metrics: number_of_reviews, last_review, reviews_per_month, number_of_reviews_ltm



calculated_host_listings_count, availability_365, license, rating, bedrooms, beds, baths



Sample Insights:





Prices range from $55 (private room in Brooklyn) to $187 (entire home in Manhattan).



Listings vary in availability (0 to 364 days/year) and host activity (1 to 139 listings per host).



Most listings have "No License" or "Exempt" status.

Key Findings





Strong Positive Correlation (0.63): Listings with more reviews tend to have higher reviews per month, indicating active and popular listings.



Moderate Positive Correlation (0.066): Listings with more beds are slightly more expensive, suggesting capacity influences pricing.



Moderate Negative Correlation (-0.12): Longer minimum stays are associated with fewer reviews per month, potentially deterring frequent bookings.

Prerequisites

To run this project, ensure the following Python libraries are installed:





pandas: For data manipulation and analysis



numpy: For numerical operations



matplotlib: For plotting visualizations



seaborn: For enhanced statistical visualizations

Install dependencies using:

pip install pandas numpy matplotlib seaborn

Project Structure





New_York_Airbnb_EDA_Project_.ipynb: Jupyter Notebook containing the EDA code.



datasets.csv: Input dataset with Airbnb listing details.



README.md: This file, providing project documentation.

Setup Instructions





Clone the Repository:

git clone <repository-url>
cd <repository-directory>



Place the Dataset: Ensure datasets.csv is in the project directory or update the file path in the notebook.



Run the Notebook:





Open New_York_Airbnb_EDA_Project_.ipynb in Jupyter Notebook or JupyterLab.



Execute the cells sequentially to load the data and perform the analysis.



Example code to load data:

import pandas as pd
df = pd.read_csv('datasets.csv')
df.head()

Analysis Workflow





Data Loading: The dataset is loaded using pandas from datasets.csv.



Initial Exploration: The df.head() command displays the first five rows to inspect listing details.



Correlation Analysis: Key correlations identified include:





Reviews vs. reviews per month



Beds vs. price



Minimum nights vs. reviews per month



Future Steps (assumed):





Visualizations (e.g., scatter plots, histograms) using Matplotlib/Seaborn.



Geographic analysis using latitude/longitude.



Statistical tests or further feature engineering.

Potential Visualizations





Scatter plots to visualize correlations (e.g., reviews vs. reviews per month).



Histograms for price or availability distributions.



Heatmaps for correlation matrices.



Geographic maps to plot listings by neighborhood.

Limitations





The dataset may contain missing or inconsistent values (e.g., "Not specified" in the baths column), requiring preprocessing.



The provided excerpt lacks full visualization or statistical analysis code, limiting detailed insights.



Regulatory aspects (e.g., licensing) may affect listing availability and need further exploration.

Future Enhancements





Add visualizations to explore price distributions by neighborhood or room type.



Perform statistical tests to validate correlations.



Incorporate geospatial analysis to map listing density or pricing trends.



Clean data for missing values or inconsistent entries (e.g., standardizing bedrooms or baths).

Requirements





Python 3.x



Jupyter Notebook or JupyterLab



Libraries: pandas, numpy, matplotlib, seaborn
