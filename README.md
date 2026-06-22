# Netflix-Analysis

# Netflix Dataset Analysis

This repository contains a comprehensive exploratory data analysis (EDA) of the Netflix dataset. The analysis aims to uncover trends, patterns, and insights into the content available on Netflix, including distribution of content types, ratings, release trends over years, and geographical content production.

## Table of Contents

1.  [Project Overview](#project-overview)
2.  [Dataset](#dataset)
3.  [Analysis Steps](#analysis-steps)
4.  [Key Findings](#key-findings)
5.  [Setup and Usage](#setup-and-usage)

## Project Overview

This project delves into the Netflix content library using Python's pandas, matplotlib, and seaborn libraries. We perform data cleaning, handle missing values, and then visualize various aspects of the dataset to gain a better understanding of Netflix's content strategy and evolution over time.

## Dataset

The dataset used for this analysis is `netflix_titles.csv`, which contains information about movies and TV shows available on Netflix. It includes columns such as `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in` (genres), and `description`.

## Analysis Steps

The analysis covered the following key steps:

1.  **Data Loading & Initial Inspection**: Loaded the CSV into a pandas DataFrame and examined its basic structure and information.
2.  **Data Preprocessing & Cleaning**:
    *   Removed entries with 'min' in the 'rating' column (likely duration information).
    *   Handled missing values in `director`, `cast`, `country`, `date_added`, `rating`, and `duration` columns through imputation (filling with 'unknown', 'not available', or mode).
    *   Checked for and confirmed the absence of duplicate rows.
    *   Cleaned string data by trimming whitespace and converting all text to lowercase for consistency.
3.  **Exploratory Data Analysis & Visualization**:
    *   **Content Type Distribution**: Visualized the proportion of movies versus TV shows.
    *   **Content Rating Distribution**: Explored the distribution of content ratings using a pie chart.
    *   **Release Trends Over Years**: Analyzed the number of releases annually to identify growth patterns.
    *   **Duration Distribution**: Illustrated the distribution of content durations (both movies and TV shows).
    *   **Top 10 Countries by Content Production**: Identified and visualized countries with the highest content contributions.
    *   **Movie and TV Show Releases vs. Years**: Separately tracked the annual release trends for movies and TV shows.

## Key Findings

*(This section can be populated with specific insights you gained from your analysis after reviewing the generated plots. For example:)*

*   Netflix has a higher volume of movies compared to TV shows.
*   The platform primarily features content with `TV-MA` and `TV-14` ratings.
*   There has been a significant increase in content releases, particularly in the last decade, with a peak around 2018-2020.
*   The United States is overwhelmingly the top contributor of content, followed by India and the UK.
*   While movie releases peaked and have slightly declined recently, TV show production has shown a more consistent upward trend.

## Setup and Usage

To run this analysis, you will need a Python environment with the following libraries installed:

*   `pandas`
*   `matplotlib`

YouYou can install these using pip:

```bash
pip install pandas matplotlib 
```

Once the dependencies are installed, you can open and run the `Netflix_Analysis.ipynb` notebook in a Jupyter environment (like Google Colab or Jupyter Notebook/Lab).
```
