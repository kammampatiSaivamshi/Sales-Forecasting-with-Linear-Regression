# Netflix User Behavior Analysis

## Overview

This project aims to analyze Netflix user behavior to provide insights into viewing habits, genre preferences, and binge-watching patterns. By examining a dataset of Netflix viewing data, we aim to:

* Identify top genres and their trends over time.
* Analyze the number of hours watched per user.
* Visualize binge-watching behaviors.
* Explore ratings vs. genres to offer personalized content recommendations.

The insights derived from this analysis can help Netflix or other streaming platforms optimize their content recommendations and improve user engagement strategies.

## Dataset

The dataset used in this project contains information about Netflix viewing habits. The data includes details on user behavior, such as:

* **User ID**: Unique identifier for each user.
* **Genre**: The genre of the movie or TV show watched.
* **Watch Hours**: Total watch hours per user or per title.
* **Rating**: User ratings for the titles watched.
* **Date**: Date of the viewing session.
* **Other Features**: Information like device type, location, or subscription status (if available).

## Files

* `Netflix_User_Behavior_Analysis.ipynb`: Jupyter notebook that contains all the analysis, visualizations, and model building.
* `netflix_user_data.csv`: The CSV file containing Netflix viewing behavior data.

## Requirements

To run this project, you will need the following Python libraries:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* plotly

## Installation

You can install the required dependencies by using the following command:

```bash
pip install -r requirements.txt
```

If you don’t have `requirements.txt`, you can manually install the necessary libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly
```

## Usage

1. **Load the Data**: Start by loading the dataset into a pandas DataFrame for exploration.

```python
import pandas as pd

data = pd.read_csv('netflix_user_data.csv')
```

2. **Data Preprocessing**: Clean the dataset by handling missing values, converting categorical features, and preparing the data for analysis.

3. **Exploratory Data Analysis (EDA)**: Explore the dataset by visualizing trends, such as top genres, viewing hours, and user ratings.

4. **User Behavior Analysis**:

   * Identify binge-watching behaviors (e.g., users who watched multiple episodes or movies in a short time frame).
   * Analyze watch hours per user and compare it with their genre preferences.
   * Visualize ratings vs. genres to understand user satisfaction.

5. **Modeling (Optional)**: If relevant, build recommendation models or predictive models for content suggestions based on user behavior.

## Example: Visualizing Top Genres

Here’s an example of how to visualize the top genres watched:

```python
import matplotlib.pyplot as plt

# Group by genre and calculate total watch hours
genre_data = data.groupby('Genre')['Watch Hours'].sum().sort_values(ascending=False)

# Plot top genres
plt.figure(figsize=(10,6))
genre_data.head(10).plot(kind='bar', color='skyblue')
plt.title('Top 10 Genres by Watch Hours')
plt.xlabel('Genre')
plt.ylabel('Watch Hours')
plt.xticks(rotation=45)
plt.show()
```

## Insights

This analysis allows the following key insights:

* **Top Genres**: Understanding which genres are most popular among users.
* **Binge-Watching Trends**: Identifying users' binge-watching habits based on viewing patterns.
* **Content Recommendation**: By understanding genre preferences and ratings, personalized content suggestions can be made to users.

## Contributing

Feel free to contribute to this project by submitting bug reports, features, or enhancements through issues or pull requests.

### 🙋‍♂️ Author

**Vamshi K**
*Aspiring Data Scientist*
📫 Reach me on [LinkedIn](https://www.linkedin.com)


