# Cinematic Insights Dashboard Project

## Overview
This project involves creating an interactive dashboard to explore trends and insights from movie ratings data. The goal is to analyze user engagement, top-rated genres, yearly distribution of ratings, and top movies, providing an intuitive visualization for users.

### Dataset Source
The dataset for this project was obtained from [**MovieLens**](https://grouplens.org/datasets/movielens/), a research project run by the GroupLens research lab at the University of Minnesota. It contains user ratings, movie metadata, and timestamped interactions, making it ideal for exploring trends in movie engagement, genre popularity, and rating patterns.

## Project Steps

### 1. Data Preparation (Python)
We started by cleaning and preprocessing the raw data using Python.
- **Tools used:** Pandas, NumPy
- **Steps:**
  - Imported the movie ratings dataset from **MovieLens**.
  - Parsed and converted timestamp fields to date formats.
  - Split genres into separate rows for easier analysis.
  - Exported the processed data to CSV files named `processed_movie_ratings.csv` and `user_activity_by_hour.csv`.

### 2. Data Import (Tableau)
- Imported the cleaned CSV files into Tableau.
- Verified that fields such as `Genres Split`, `User Id`, `Rating`, and `Timestamp` were correctly formatted.
- Joined the `processed_movie_ratings.csv` with `user_activity_by_hour.csv` using **User Id** and **Timestamp**.

### 3. Data Exploration
Several visualizations were designed to extract meaningful insights from the data:

#### User Engagement by Hour
- Visualizes the number of ratings by the hour of the day.
- Includes filters for time range and AM/PM segmentation.
- Highlights peak engagement hours with reference lines.

#### Top Rated Movies by Genre
- Displays a tree map with genres sized and colored by the average rating.
- Includes tooltips showing key details about each genre.

#### Ratings Distribution by Year
- A dual-axis line chart showing both the average rating and count of ratings over time.
- Filters allow selection by genre and specific years.

#### Top 10 Movies of the Year
- Displays a ranked bar chart of the top 10 movies for a selected year.
- Includes a combined ranking feature based on average rating and count of ratings.

### 4. Dashboard Creation
We designed an interactive dashboard titled **Cinematic Insights** with the following features:
- A sleek horizontal navigation bar with clickable buttons for each key section.
- Filter options for time range, genres, and year.
- Custom-designed banners to enhance the user experience.

### 5. Enhancements and Customizations
- Added descriptive tooltips to provide users with more context.
- Implemented filters and calculated fields to support dynamic interactions.
- Created reference lines to highlight key metrics like average engagement and ratings.

### 6. Tableau Publishing Limitation
   - When attempting to publish the workbook to Tableau Public, an error occurred due to the data size exceeding Tableau Public's limit of **15,000,000 rows**.
   - As a result, the workbook was not uploaded to Tableau Public. Alternatives include using Tableau Server, Tableau Online, or reducing the data volume.

## Project Files
- `processed_movie_ratings.csv`: Cleaned dataset used in Tableau.
- `user_activity_by_hour.csv`: Activity-based dataset created from Python.
- `dashboard_user_engagement.twbx`: Tableau workbook file containing the visualizations.
- `EDA_Data_cleaning.ipynb`: Python notebook for preprocessing and cleaning the data.
- `Cinematic_Insights_Dashboard_Report.pdf`: Detailed project report with dashboard screenshots and descriptions.
- `README.md`: Project documentation (this file).

## Usage Instructions
1. Open the Tableau workbook.
2. Navigate through the dashboard using the buttons on the navigation bar.
3. Use the available filters to customize your view and explore the data.

## Technologies Used
- **Python:** Data cleaning and preprocessing.
- **Tableau:** Data visualization and dashboard creation.
- **CSV:** Data storage format.

## Project Insights
- Peak engagement occurs in the evening hours.
- Genres like Drama and Thriller consistently receive high average ratings.
- Movie ratings trends show fluctuations over the years, influenced by various factors.

## Future Improvements
- Integrate additional data sources, such as box office performance or audience reviews.
- Implement predictive analytics to forecast future trends.
- Enhance interactivity with more dynamic filters and drill-down capabilities.

## Acknowledgments
This project was made possible with the support of various open-source libraries and visualization tools. Special thanks to the Python and Tableau communities for their invaluable resources and documentation.

## Contact Information
For further information or inquiries, please reach out to me:

- **Name:** Nikhita Shankar
- **Email:** nikhita4@illinois.edu
- **LinkedIn:** [Nikhita Shankar](https://www.linkedin.com/in/nikhitashankar)
