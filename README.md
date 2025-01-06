# WeRateDogs Data Wrangling and Analysis

## Introduction

Real-world data is rarely clean, and this project focuses on the process of data wrangling — gathering, assessing, and cleaning data to make it suitable for analysis. Using Python and its libraries, this project works with the tweet archive of the popular Twitter account [@dog_rates](https://twitter.com/dog_rates), also known as **WeRateDogs**.

WeRateDogs is a Twitter account that humorously rates people's dogs, with ratings often exceeding the usual 10-point scale (e.g., 12/10, 13/10). The account has over 4 million followers and has received international media attention. For this project, we analyze and visualize the data shared by WeRateDogs to gain insights into their tweets and ratings.

---

## Project Overview

This project involves the following key steps:
1. **Gathering Data**:
   - Data is collected from multiple sources in various formats.
2. **Assessing Data**:
   - Data is assessed for quality (issues affecting data integrity) and tidiness (issues with data structure).
3. **Cleaning Data**:
   - Identified issues are fixed programmatically to ensure the data is ready for analysis.

Finally, the cleaned data is analyzed and visualized to showcase insights.

---

## Datasets

This project uses the following datasets:

1. **Twitter Archive Dataset**:
   - Provided by WeRateDogs via email, this dataset contains basic tweet data (e.g., tweet ID, timestamp, text) for 5000+ tweets as of August 1, 2017.

2. **Image Predictions Dataset**:
   - Extracted using Python's `requests` library via Udacity's provided URL. This dataset contains image predictions for dog breeds (and other objects) using a neural network.

3. **Additional Data from Twitter API**:
   - Data such as retweet count and favorite count are collected programmatically by querying the Twitter API.

---

## Tools and Libraries

- **Python Libraries**:
  - `pandas`: For data manipulation and cleaning.
  - `numpy`: For numerical operations.
  - `matplotlib` and `seaborn`: For data visualization.
  - `requests`: For gathering data via HTTP requests.
  - `tweepy`: For accessing the Twitter API.
- **Jupyter Notebook**: For documenting the data wrangling process.
- **SQL**: For additional analyses, if applicable.

---

## Project Steps

### 1. Gathering Data
- **Twitter Archive File**: Downloaded manually and loaded into a Pandas DataFrame.
- **Image Predictions File**: Programmatically downloaded from a Udacity-provided URL.
- **Twitter API Data**: Queried using `tweepy` to gather additional tweet metadata.

### 2. Assessing Data
- **Visual Assessment**: Manually inspecting datasets in a Jupyter Notebook.
- **Programmatic Assessment**: Using Pandas to detect:
  - Missing data
  - Duplicates
  - Invalid or inconsistent entries
  - Issues with data structure

### 3. Cleaning Data
- **Define, Code, and Test Framework**:
  - Define: Document each data issue identified during assessment.
  - Code: Programmatically fix each issue using Pandas.
  - Test: Validate that each fix was successful.

### 4. Storing Clean Data
- Cleaned data is saved to CSV files for easy sharing and future analysis.

### 5. Analyzing and Visualizing Data
- Insights into the popularity of tweets, trends in ratings, and dog breed predictions are explored through Python visualizations.

---

## Key Insights

Here are some questions the project explores:
1. What are the most popular dog breeds according to WeRateDogs' neural network predictions?
2. What types of tweets (based on rating or text) get the most retweets and favorites?
3. Are there patterns in tweet ratings over time?
4. How often do ratings exceed the typical 10-point denominator?

---

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/WeRateDogs-Wrangling.git
   ```

2. **Run the Jupyter Notebook**:
   - Open the notebook to see the step-by-step wrangling process.

3. **Explore the Cleaned Data**:
   - The cleaned datasets are saved as CSV files in the repository for further analysis.

4. **View the Visualizations**:
   - The notebook includes insights and visualizations based on the cleaned data.

---

## Future Enhancements

- Extend the analysis to identify trends in tweet engagement over time.
- Build a machine learning model to predict tweet popularity based on content and ratings.
- Incorporate SQL queries for advanced analysis.
