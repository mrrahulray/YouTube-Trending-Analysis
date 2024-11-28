# YouTube Trending Videos Analysis - Data Analytics Project

## Project Overview
This project is part of the Software Development: Programming and Algorithms (SDPA) module at the University of Bristol. The aim is to apply data analytics skills to extract, clean, and analyze data using Python, specifically in a Jupyter notebook environment. The data source selected for this project is the YouTube API, which provides information about trending videos. The goal is to use this data to derive meaningful insights regarding video trends, popularity metrics, and content characteristics.

The project is implemented in Jupyter Notebook using Python, where the dataset is collected through the YouTube API. The dataset consists of several attributes such as Video ID, Title, Views, Likes, Dislikes, Comments, Publish Date, Tags, and Category ID, enabling us to explore various aspects of the trending videos. The complete version control for the project has been managed using Git and is accessible through the linked GitHub repository.

## Project Structure
The project is divided into several key steps to ensure a logical and systematic approach to data analysis:

1. **Data Collection**: This part involves collecting real-time data using the YouTube API. The dataset is saved in CSV format for easier handling.
2. **Data Preparation & Cleaning**: This stage focuses on importing the dataset into a Pandas DataFrame, handling missing values, and preparing the data for further analysis.
3. **Exploratory Data Analysis**: The next step involves analyzing the distribution of key variables, calculating summary statistics, and identifying any interesting patterns in the data.
4. **Question Formulation and Analysis**: In this section, an interesting question is posed regarding the data, and various sub-questions are analyzed to provide a comprehensive answer. Techniques such as aggregation, plotting, and statistical modeling are used.
5. **Conclusion**: A summary of the key findings is provided, along with suggestions for further exploration.

## Files Overview
- **YouTube_Trending_Analysis.ipynb**: The Jupyter notebook that contains the entire workflow, including the data collection, cleaning, analysis, and visualization steps. Markdown cells are included to document the process and explain each part of the analysis.
- **trending_videos_data.csv**: The dataset collected from the YouTube API. It contains information about trending YouTube videos such as title, view count, like count, and publish date.
- **README.md**: This file (current one), which provides a detailed overview of the project structure, code design, classes, methods, and other important details.

## Design Choices
1. **Data Collection Using YouTube API**: The YouTube API was chosen as the data source to provide a fresh, real-world dataset that allows us to explore recent trends. I used Python's requests library to make API calls and save the response data as CSV.

2. **Data Cleaning and Feature Extraction**: Missing values in features like Tags were handled by filling them with placeholders. New columns such as "like-to-view ratio" were created to enrich the data for deeper analysis.

3. **Exploratory Data Analysis Techniques**: Various plots, including histograms and bar charts, were used to visualize distributions. Scatter plots and line graphs were employed to identify correlations between variables like view count and like count.

4. **Handling External Dependencies**: The project uses standard Python packages like `requests`, `pandas`, `matplotlib`, `seaborn`, and `scipy` for data handling, visualization, and analysis. No other external libraries were used.

## How to Run the Project
1. **Dependencies**: The project requires Python 3.x and the following packages:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `requests`
   - `seaborn`
   - `scipy`

   Install dependencies using pip:
   ```sh
   pip install pandas numpy matplotlib requests seaborn scipy
   ```

   Any additional libraries or external sources needed to run the code correctly must be explained in this README file.

2. **Running the Notebook**: Open the Jupyter notebook by running:
   ```sh
   jupyter notebook YouTube_Trending_Analysis.ipynb
   ```
   Follow the cells in the notebook sequentially to understand the complete workflow from data collection to analysis.

## GitHub Repository
The full code and documentation for the project are available in a private GitHub repository. Please make sure to add "SDPA-UoB" as a collaborator as instructed by the university.

Link to GitHub repository: [YouTube Trending Analysis Project](#) (Make sure you have access permissions.)

## Additional Notes
- **Documentation**: Detailed documentation is provided within the Jupyter notebook using markdown cells, which explain each step and process in the project.
- **Version Control**: The project is under version control, with multiple commits highlighting each stage of the implementation. Each commit message provides context about changes made.
- **Technical Challenges**: One of the challenges encountered was rate-limiting by the YouTube API. To address this, API requests were spread across multiple days to ensure full data retrieval.

## Future Work
- **Incorporate Additional Data Sources**: Future extensions can include integrating other APIs like Twitter or Reddit to explore cross-platform trends.
- **Advanced Analysis**: The current analysis can be expanded with machine learning techniques to predict what makes a video trend.

The project demonstrates the effective use of data extraction, cleaning, analysis, and visualization techniques in a data science context.

