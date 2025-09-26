# Global Movie Database Analysis: Data Cleaning & Exploratory Data Analysis

## Project Overview

This project involves an in-depth analysis of the "Global Movie Database: A Comprehensive Overview" dataset, obtained from Kaggle. The primary objective was to demonstrate proficiency in fundamental data science skills: data cleaning, wrangling, and exploratory data analysis (EDA). The project involved transforming a raw, messy dataset into a clean, structured format, and subsequently extracting meaningful insights through various visualizations.

## Dataset

The dataset used is `movies_metadata.csv` from Kaggle's "Global Movie Database: A Comprehensive Overview". It contains detailed information about a vast collection of movies, including:
-   Movie title, original title
-   Release date, runtime
-   Genres, production companies, production countries, spoken languages
-   Budget, revenue, popularity, vote average, vote count
-   Overview/synopsis

## Goals

1.  **Data Cleaning & Wrangling:**
    *   Load the raw dataset using Pandas.
    *   Handle missing values across various columns (e.g., `runtime`, `overview`).
    *   Address mixed data types and convert columns (`popularity`, `budget`, `release_date`, `id`) to appropriate numerical or datetime formats.
    *   Parse complex JSON-like string columns (`genres`, `production_companies`, `production_countries`, `spoken_languages`) into usable list formats.
    *   Drop irrelevant or highly sparse columns.
2.  **Exploratory Data Analysis (EDA):**
    *   Identify and visualize key trends and patterns within the movie database.
    *   Answer specific questions about movie production and characteristics.
3.  **Reporting:**
    *   Present findings clearly in a structured Jupyter Notebook report, supported by data visualizations.

## Key Findings (from EDA)

The exploratory data analysis revealed several interesting insights into the global movie landscape:

1.  **Dominant Genres:** The most prevalent genres across the database are **Drama**, **Comedy**, and **Thriller**, indicating their enduring appeal and high production volume.
2.  **Top Producing Countries:** The **United States (US)** overwhelmingly leads in movie production, followed by significant contributions from the United Kingdom (GB) and France (FR), reinforcing their status as major hubs in the film industry.
3.  **Growth in Movie Production Over Time:** Analysis of release dates showed a clear upward trend in the number of movies produced annually, with a substantial increase observed from the early 2000s to the mid-2010s. This highlights a period of significant expansion in the global film industry. *(Note: The dataset shows a drop in very recent years, likely due to incompleteness for those specific periods rather than a genuine decline.)*

## Technologies Used

*   **Python:** Programming language for data analysis.
*   **Pandas:** For data manipulation and cleaning.
*   **NumPy:** For numerical operations.
*   **Matplotlib:** For static data visualizations.
*   **Seaborn:** For enhanced statistical data visualizations.
*   **Jupyter Notebook:** For creating the interactive report.
*   **(Optional: pycountry):** Used for mapping ISO country codes to full country names.

## How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/YourGitHubUsername/Global-Movie-EDA.git
    cd Global-Movie-EDA
    ```
    *(Replace `YourGitHubUsername` and `Global-Movie-EDA` with your actual GitHub username and repository name.)*
2.  **Download the Dataset:**
    *   Go to [Kaggle: Global Movie Database](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)
    *   Download the `movies_metadata.csv` file.
    *   Place the `movies_metadata.csv` file in the same directory as the Jupyter Notebook.
3.  **Install Dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn jupyter # pycountry (if desired for full country names)
    ```
4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
5.  **Open the Notebook:**
    *   Open `Global_Movie_Analysis_Report.ipynb` (or whatever you named your notebook) in your browser.
    *   Run all cells sequentially to reproduce the analysis and visualizations.
