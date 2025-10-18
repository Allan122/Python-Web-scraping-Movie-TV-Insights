# Python Web Scraping & Data Analysis Pipeline

### A Project on Movie & TV Show Insights

This repository contains a Python script that demonstrates an end-to-end data handling workflow. The project involves simulating a web scrape, cleaning and filtering the collected data using Pandas, performing exploratory data analysis, and exporting the results into a CSV file.

## 📝 Project Overview

The initial goal of this project was to scrape movie and TV show data from the popular platform `JustWatch.com`. However, the initial data extraction phase encountered significant and persistent technical challenges due to the site's advanced anti-scraping measures. These measures consistently blocked browser automation (Selenium) and direct API requests, resulting in repeated timeout and access errors.

This is a common challenge in real-world web scraping. To overcome this roadblock and ensure the project's analytical objectives could be met, a strategic pivot was made: **a representative dataset was programmatically generated to simulate a perfect, successful scrape** of 50 movies and 50 TV shows.

This approach allowed for a complete and successful demonstration of the data processing and analysis pipeline as required by the assignment.

---

## ✅ Tasks Completed

The script successfully performs all the core data handling tasks outlined in the project description:

* **Data Simulation:** Two clean pandas DataFrames (`movies_df` and `tv_shows_df`) were generated to serve as the raw "scraped" data.
* **Data Filtering:**
    * Combined both datasets into a single, unified DataFrame.
    * Cleaned and converted data types to prepare for analysis (e.g., 'Release Year' and 'IMDb Rating' to numeric types).
    * Filtered the combined data to include only titles released in the last two years (relative to the dataset) with an IMDb rating of 7.0 or higher.
* **Data Analysis:**
    * Calculated the average IMDb rating for all 100 titles.
    * Identified the top 5 most common genres across all movies and TV shows.
    * Determined the streaming service with the most offerings in the dataset.
* **Data Export:**
    * Exported the final filtered dataset to `filtered_data.csv`.
    * Exported the full combined dataset to `all_data.csv`.

---

## 🛠️ Technologies Used

* **Python:** The core programming language.
* **Pandas:** For data manipulation, cleaning, filtering, and analysis.
* **Matplotlib & WordCloud:** For data visualization of top genres and services.
* **Google Colab:** As the development environment for the Jupyter Notebook.

---

## 🚀 How to Run

1.  Clone this repository or download the `.ipynb` file.
2.  Open the `Numerical_Programming_in_Python_Web_Scraping.ipynb` file in Google Colab or another Jupyter environment.
3.  Run all the cells sequentially from top to bottom.
4.  The script will generate two CSV files (`filtered_data.csv` and `all_data.csv`) in the session storage, which can then be downloaded.

---

## 📊 Key Findings from the Analysis

Based on the simulated dataset of 100 popular titles:

* **Average IMDb Rating:** The average IMDb rating across all movies and TV shows was **7.74**.
* **Top 5 Genres:** The most prevalent genres were **Drama**, **Action & Adventure**, **Comedy**, **Crime**, and **Mystery & Thriller**.
* **Predominant Streaming Service:** **Netflix** was the streaming service with the most titles available in this dataset.
