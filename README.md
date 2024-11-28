# YouTube Trending Videos Analysis - Data Analytics Project

## Project Overview
This project is part of the **Software Development: Programming and Algorithms (SDPA)** module at the University of Bristol. The objective is to apply data analytics skills to extract, clean, and analyze data using Python, specifically in a Jupyter notebook environment. Using the YouTube API, real-time data about trending videos has been collected to derive meaningful insights about video trends, popularity metrics, and content characteristics.

The project dataset includes several attributes such as Video ID, Title, Views, Likes, Dislikes, Comments, Publish Date, Tags, and Category ID. This enables a comprehensive analysis of trending videos. The complete version control for the project is managed using Git and is accessible through the [GitHub repository](https://github.com/mrrahulray/YouTube-Trending-Analysis.git).

---

## Project Structure
The project is divided into key steps to ensure a systematic approach to data analysis:

1. **Data Collection**: Real-time data is collected using the YouTube API and saved in CSV format for easy handling.
2. **Data Preparation & Cleaning**: Data is imported into Pandas DataFrames, missing values are handled, and the data is prepared for analysis.
3. **Exploratory Data Analysis (EDA)**: Key variables are analyzed for trends, distributions, and relationships using descriptive statistics and visualizations.
4. **Question Formulation and Analysis**: Specific questions regarding trending videos are addressed, using sub-questions, aggregation, plotting, and statistical modeling.
5. **Conclusion**: A summary of insights, findings, and future possibilities for exploration is provided.

---

## Files Overview
- **YouTube_Trending_Analysis.ipynb**: The Jupyter notebook containing the entire workflow, including data collection, cleaning, analysis, and visualization. Markdown cells document each step.
- **trending_videos_data.csv**: The dataset collected via the YouTube API, containing details about trending videos.
- **README.md**: This file, providing an overview of the project structure, methodology, and key components.

---

## Design Choices
### 1. Data Collection Using YouTube API
The YouTube API was used as the data source for its real-world, up-to-date data about trending videos. API calls were made using Python's `requests` library, and the responses were saved as CSV files.

### 2. Data Cleaning and Feature Extraction
- Missing values in fields like Tags were handled using placeholders.
- New features, such as "like-to-view ratio," were created for deeper analysis.

### 3. Exploratory Data Analysis Techniques
Visualizations such as histograms, bar charts, scatter plots, and line graphs were used to identify patterns and relationships.

### 4. Handling Dependencies
Standard Python libraries (`requests`, `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scipy`) were used for data handling, visualization, and analysis.

---

## How to Run the Project

### 1. Install Dependencies
Ensure Python 3.x is installed. Install the required packages using:
```sh
pip install pandas numpy matplotlib requests seaborn scipy
```

### 2. Running the Notebook
To execute the project, run the following command to open the Jupyter notebook:
```sh
jupyter notebook YouTube_Trending_Analysis.ipynb
```
Follow the notebook cells sequentially to replicate the analysis process.

---

## GitHub Repository
The full codebase and detailed documentation are available in the GitHub repository. Visit the link below:

[YouTube Trending Videos Analysis - GitHub Repository](https://github.com/mrrahulray/YouTube-Trending-Analysis.git)

---

## Additional Notes
### Documentation
Detailed documentation is provided within the notebook, explaining each step of the process.

### Version Control
The project is under version control in Git, with multiple commits representing different stages of implementation. Each commit includes descriptive messages for context.

### Challenges and Solutions
- **API Rate Limiting**: Requests were spaced across multiple days to overcome YouTube API rate limits.

---

## Future Work
1. **Incorporate Additional Data Sources**: Integrate data from platforms like Twitter or Reddit to analyze cross-platform trends.
2. **Advanced Analysis**: Use machine learning to predict the factors contributing to a video's popularity.

---

This project demonstrates effective use of data extraction, cleaning, analysis, and visualization techniques in the field of data science.

