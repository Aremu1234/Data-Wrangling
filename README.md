# WeRateDogs Data Wrangling and Analysis  

This repository documents the wrangling, analysis, and visualization of the tweet archive of Twitter user **@dogrates**, also known as **WeRateDogs**. WeRateDogs is a popular Twitter account that humorously rates people's dogs with an overwhelming majority of ratings above 10/10, such as 11/10, 12/10, etc. The account has gained international media attention and boasts over 4 million followers.  

---

## Project Overview  

### **Wrangle Report**  
The data wrangling process consisted of the following steps:  

#### 1. **Gathering Data**  
Data was gathered from three different sources:  

- **Enhanced Twitter Archive**  
  Contains extracted tweet data, including ratings, dog names, and stages.  

- **Image Prediction File**  
  Generated using a neural network that predicts the breed of dogs from the tweet images. Includes tweet IDs, image URLs, and top-3 predictions for each image.  

- **Additional Data via Twitter API**  
  Contains tweet metrics such as retweet count and favorite count. This data was read into a DataFrame and saved as `tweet_data.csv` for further use.  

#### 2. **Accessing Data**  
Data was assessed both visually and programmatically to identify issues related to tidiness and quality.  

- **Tidiness Issues**  
  - Dog stage data was spread across four columns.  
  - Data was split across three separate DataFrames.  

- **Quality Issues**  
  - **Enhanced Twitter Archive**: Invalid dog names, incorrect data types, and retweets in the dataset.  
  - **Image Prediction File**: Missing photos for some tweet IDs and inconsistent naming formats.  
  - **Tweet API Data**: Missing entries for some tweets.  

#### 3. **Cleaning Data**  
All identified issues were resolved to ensure the data was ready for analysis and visualization.  

---

### **Act Report**  
This report communicates insights and visualizations derived from the cleaned data.  

#### **Storing Data**  
The cleaned data was saved in a CSV file named `twitter_archive_data.csv` for ease of use in analysis and visualization.  

#### **Analyzing and Visualizing Data**  
Key findings and visualizations include:  

1. **Percentage of Dog Stages**  
   - **Pupper** had the highest percentage (68.4%).  
   - **Floofer** had the lowest percentage (0.9%).  
   - Visualized using a pie chart.  

2. **Relationship Between Retweet Count and Favorite Count**  
   - A scatter plot revealed a linear relationship between retweet count and favorite count.  

---

## Key Files in This Repository  

- **`wrangle_report.md`**: Details the wrangling process (gathering, assessing, and cleaning data).  
- **`act_report.md`**: Documents the findings and visualizations from the analysis.  
- **`twitter_archive_data.csv`**: The cleaned dataset ready for analysis and visualization.  
- **`notebook.ipynb`**: Jupyter Notebook containing all wrangling, analysis, and visualization steps.  

---

## Tools and Libraries Used  

- **Data Wrangling**: Python, Pandas, NumPy  
- **Data Visualization**: Matplotlib, Seaborn  
- **Data Access**: Twitter API  

---  

This project highlights the value of clean data in uncovering meaningful insights and relationships within datasets.
