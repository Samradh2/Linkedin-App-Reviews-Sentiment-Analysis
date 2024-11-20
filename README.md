# Linkedin-App-Reviews-Sentiment-Analysis


This Python script performs exploratory data analysis (EDA) and sentiment analysis on a dataset containing LinkedIn reviews. The script includes the following steps:

---

## **Features of the Script**

### 1. **Dataset Overview**
- **Input**: A CSV file named `linkedin reviews.csv` containing reviews and their corresponding ratings.
- **Output**: 
  - Initial overview of the data using `.head()` and `.info()`.
  - Visualization of the distribution of ratings.

### 2. **Exploratory Data Analysis**
- **Review Length Analysis**:
  - Calculates the length of each review and visualizes the distribution of review lengths.
  - This provides insights into whether reviews tend to be short or long.

### 3. **Sentiment Analysis**
- **Sentiment Categorization**:
  - Sentiments of reviews are analyzed using the TextBlob library.
  - Reviews are classified into:
    - **Positive** (Polarity > 0.1)
    - **Neutral** (-0.1 ≤ Polarity ≤ 0.1)
    - **Negative** (Polarity < -0.1)
  - Sentiment counts are plotted for visualization.

### 4. **Sentiment Distribution Across Ratings**
- Visualizes how sentiment is distributed across different review ratings.

### 5. **Word Clouds**
- **Purpose**:
  - Generates word clouds for Positive, Neutral, and Negative reviews.
  - This highlights the most frequent words associated with each sentiment.

---

## **Dependencies**

Ensure the following Python libraries are installed:
- `pandas`
- `matplotlib`
- `seaborn`
- `textblob`
- `wordcloud`

You can install them using:
```bash
pip install pandas matplotlib seaborn textblob wordcloud
```

---

## **Code Explanation**

### **Step-by-Step Execution**

1. **Load Dataset**
   - Reads the `linkedin reviews.csv` file into a DataFrame and displays the first few rows.
   - Prints dataset info to understand its structure.

2. **Rating Distribution**
   - Uses a count plot to show the number of reviews for each rating.

3. **Review Length Analysis**
   - Adds a new column, `Review Length`, to store the character count of each review.
   - Plots the distribution of review lengths.

4. **Sentiment Analysis with TextBlob**
   - Applies the `TextBlob` library to classify reviews into Positive, Negative, and Neutral.
   - Adds a new column, `Sentiment`, to store these classifications.
   - Visualizes sentiment distribution using bar plots.

5. **Sentiment Across Ratings**
   - Uses a grouped bar plot to show the sentiment distribution for each rating.

6. **Word Clouds**
   - Generates word clouds for Positive, Negative, and Neutral reviews, visualizing the most common words in each sentiment category.

---

## **Visualizations**

1. **Distribution of Ratings**  
   A count plot showing the number of reviews per rating.

2. **Distribution of Review Lengths**  
   A histogram showing how review lengths are distributed.

3. **Sentiment Distribution**  
   A bar plot visualizing the number of Positive, Neutral, and Negative reviews.

4. **Sentiment Distribution Across Ratings**  
   A grouped count plot illustrating sentiment distribution for each rating.

5. **Word Clouds**  
   Separate word clouds for Positive, Negative, and Neutral reviews.

---

## **Usage Instructions**

1. Clone this repository:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. Ensure the `linkedin reviews.csv` file is in the same directory as the script.

3. Run the script:
   ```bash
   python linkedin_reviews_analysis.py
   ```

4. The script will generate several visualizations and print data insights.

---

## **Potential Enhancements**

1. **Improved Sentiment Analysis**: Replace `TextBlob` with more advanced sentiment analysis models like `VADER` or Hugging Face Transformers.
2. **Interactivity**: Use tools like Plotly or Dash to make visualizations interactive.
3. **Additional EDA**: Explore relationships between review length and sentiment or rating.

---

This documentation should provide a clear understanding of your code and how to run it for anyone exploring your GitHub repository! Let me know if you want help drafting a `README.md` file specifically. 😊
