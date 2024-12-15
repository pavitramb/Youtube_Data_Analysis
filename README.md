# YouTube Trending Videos Analysis

This project provides an analysis of trending YouTube videos using Python and Pandas. The dataset used contains metadata about trending YouTube videos, such as views, likes, dislikes, comment counts, and other relevant information. The goal is to explore the data and uncover patterns and insights.

## Features

- Data Cleaning: Handle missing values and preprocess the dataset.
- Descriptive Statistics: Summary statistics and visualization of numerical and categorical data.
- Insights Extraction: Analyze trends, such as most viewed categories, title length correlation with views, and more.
- Data Visualization: Use histograms, scatter plots, and bar charts to visualize trends.
- Aggregations: Group data by category and year for deeper insights.

## Dataset
The dataset used is named `INvideos.csv`, representing trending YouTube videos in India. The file should be placed in the specified path: `D:/Youtube/INvideos.csv`.

### Columns in the Dataset
- **video_id**: Unique identifier for each video
- **trending_date**: The date the video trended on YouTube
- **title**: Title of the video
- **description**: Video description
- **views**: Number of views
- **likes**: Number of likes
- **dislikes**: Number of dislikes
- **comment_count**: Number of comments
- **category_id**: Category of the video
- **comments_disabled**: Whether comments are disabled
- **ratings_disabled**: Whether ratings are disabled
- **video_error_or_removed**: Whether the video has been removed or had errors

## Analysis Steps

1. **Data Exploration**
    - Load and explore the dataset.
    - Check for missing values and fill `description` with an empty string where null.

2. **Data Insights**
    - Year-wise distribution of trending videos.
    - Percentage of videos trending in each year.
    - Videos with views, likes, dislikes, and comments below or above specific thresholds.
    - Descriptive statistics of numerical and non-numerical columns.

3. **Visualizations**
    - Histograms for `views`, `likes`, `dislikes`, and `comment_count`.
    - Boxplot for title length.
    - Scatter plot for title length vs. views.
    - Bar charts for category-wise `views` and `likes`.

4. **Correlation Analysis**
    - Correlation between numerical features.

5. **Category Analysis**
    - Sum of views, likes, and dislikes grouped by category.
    - Identify the category with the highest views and likes.

6. **Additional Insights**
    - Percentage of videos with comments disabled.
    - Percentage of videos with ratings disabled.
    - Count of videos with both comments and ratings disabled.
    - Count of videos that were removed or had errors.

## Key Findings

- **Year-wise Video Trends**: Most videos trended in the year extracted from the `trending_date`.
- **Popular Categories**: Categories with the highest views and likes were identified.
- **Impact of Title Length**: A scatter plot revealed the relationship between title length and views.
- **Disabled Features**: A significant percentage of videos had comments or ratings disabled.

## Usage

To run the analysis, make sure the following dependencies are installed:

```bash
pip install pandas numpy matplotlib
```

Execute the script in your Python environment:

```bash
python analysis.py
```

## File Structure

- `analysis.py`: Main script containing the code.
- `D:/Youtube/INvideos.csv`: Dataset file (update the path if necessary).

## Dependencies

- Python 3.x
- Pandas
- NumPy
- Matplotlib

## Visualizations

### Sample Outputs

- **Year-wise video trends**: Bar chart of trending videos by year.
- **Category-wise analysis**: Bar charts for views and likes.
- **Title Length vs Views**: Scatter plot showcasing the relationship.

---

**Happy Coding!** 🎉
