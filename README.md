# YouTube Trending Video Analysis

## Overview
This project analyzes YouTube trending videos using data collected from the YouTube API. The analysis focuses on understanding patterns in video views, likes, comments, and categories to identify key trends and insights.

### Key Features
- **Data Collection**: Data was collected using the YouTube API, containing columns such as Video ID, Title, Views, Likes, Dislikes, Comments, Publish Date, Tags, and Category ID.
- **Data Preparation**: Handled missing values, normalized data, and enriched it with additional columns like the day of the week.
- **Exploratory Analysis**: Examined distributions, relationships, and top categories by average views.
- **Statistical Testing**: Conducted hypothesis testing to explore differences in views between weekdays and weekends.
- **Visualization**: Generated insightful visualizations to represent key findings.

---

## How to Obtain YouTube API Data
To access YouTube data, follow these steps:
1. **Create a Google Developer Account**:
   - Visit the [Google Cloud Console](https://console.cloud.google.com/).
   - Create a new project or select an existing one.
2. **Enable the YouTube Data API**:
   - Navigate to the API Library in the Google Cloud Console.
   - Search for "YouTube Data API v3" and enable it for your project.
3. **Create API Credentials**:
   - Go to the **Credentials** tab.
   - Create a new API key and copy it for use in your scripts.
4. **Setup API Requests**:
   - Use libraries like `googleapiclient.discovery` in Python to interact with the API.
   - Example: Fetch trending videos for a region.
     ```python
     from googleapiclient.discovery import build
     
     api_key = "YOUR_API_KEY"
     youtube = build("youtube", "v3", developerKey=api_key)
     
     request = youtube.videos().list(
         part="snippet,statistics",
         chart="mostPopular",
         regionCode="US",
         maxResults=50
     )
     response = request.execute()
     ```

---

## Project Files

### 1. Jupyter Notebook
- **`SDPA assignment part 2.ipynb`**:
  - Contains the complete data collection, preparation, analysis, and visualization code.
  - Markdown cells provide detailed explanations for each step, including:
    - Data cleaning processes.
    - Exploratory data analysis.
    - Hypothesis testing.
    - Insights and conclusions.

### 2. Data Files
- **`data.csv`**:
  - Raw data extracted from the YouTube API.
- **`mean_views_by_day.csv`**:
  - Aggregated data showing average views by day of the week.
- **`mean_views_by_category.csv`**:
  - Aggregated data showing average views by category.

### 3. Output Visualizations
- Visualizations include:
  - Distribution of views, likes, and comments.
  - Bar charts of top categories by average views.
  - Scatter plots showing relationships between variables.

---

## How to Run the Project
1. Clone the repository and navigate to the project directory:
   ```bash
   git clone https://github.com/mrrahulray/YouTube-Trending-Analysis.git
   cd YouTube-Trending-Analysis
