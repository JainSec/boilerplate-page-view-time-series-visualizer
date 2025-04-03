# Time Series Data Visualizer

## Project Overview
This project visualizes time series data using line charts, bar charts, and box plots. The dataset contains daily page views on the freeCodeCamp.org forum from May 9, 2016, to December 3, 2019. The visualizations help identify trends and patterns in user engagement over time.

## Dataset Information
**File Name:** `fcc-forum-pageviews.csv`

| Feature | Description |
|---------|-------------|
| Date | The date of recorded page views (Index) |
| Page Views | The number of page views on that date |

## Functionality
### 1. Data Processing
- Import the dataset using Pandas and set the index to the date column.
- **Clean the Data**: Remove records where page views are in the top 2.5% or bottom 2.5% of the dataset to eliminate outliers.

### 2. Line Chart
- **Function:** `draw_line_plot()`
- **Chart Details:**
  - Title: "Daily freeCodeCamp Forum Page Views 5/2016-12/2019"
  - X-axis: "Date"
  - Y-axis: "Page Views"
- **Visualization:** Uses Matplotlib to generate a time-series line plot of daily page views.

### 3. Bar Chart
- **Function:** `draw_bar_plot()`
- **Chart Details:**
  - Groups data by **year** and **month**.
  - X-axis: "Years"
  - Y-axis: "Average Page Views"
  - Legend: Shows month labels with title "Months".
- **Visualization:** Uses Matplotlib to display a grouped bar chart showing monthly trends.

### 4. Box Plots
- **Function:** `draw_box_plot()`
- **Chart Details:**
  - **Year-wise Box Plot (Trend):** Displays data distribution per year.
  - **Month-wise Box Plot (Seasonality):** Displays data distribution per month.
  - X-axis labels: "Years" (for first plot), "Months" (for second plot, starting from Jan).
  - Y-axis: "Page Views".
- **Visualization:** Uses Seaborn to display two adjacent box plots comparing yearly and monthly trends.

## Installation & Setup
### Requirements
- Python 3.x
- Pandas
- Matplotlib
- Seaborn

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo-url.git
   ```
2. Navigate to the project directory:
   ```sh
   cd time-series-visualizer
   ```
3. Install dependencies:
   ```sh
   pip install pandas matplotlib seaborn
   ```
4. Run the script:
   ```sh
   python time_series_visualizer.py
   ```

## Example Output
- **Line Chart:**
  ![Line Chart Example](examples/Figure_1.png)
- **Bar Chart:**
  ![Bar Chart Example](examples/Figure_2.png)
- **Box Plots:**
  ![Box Plot Example](examples/Figure_3.png)

## Author
- Pulkit Jain
- Contact: jain.infosec@gmail.com



This is the boilerplate for the Page View Time Series Visualizer project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-projects/page-view-time-series-visualizer
