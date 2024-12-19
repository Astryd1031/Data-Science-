# Extracting and Visualizing Stock Data

## Description

Extracting essential data from datasets and visualizing it effectively is a key skill in data science. This project demonstrates how to retrieve stock data using APIs and web scraping, process it, and visualize the results through graphs. The main focus is on Tesla and GameStop stocks, showcasing their historical share prices and revenues.

## Table of Contents

1. **Define a Function that Makes a Graph**
2. **Question 1: Use `yfinance` to Extract Stock Data**
3. **Question 2: Use Web Scraping to Extract Tesla Revenue Data**
4. **Question 3: Use `yfinance` to Extract Stock Data**
5. **Question 4: Use Web Scraping to Extract GameStop Revenue Data**
6. **Question 5: Plot Tesla Stock Graph**
7. **Question 6: Plot GameStop Stock Graph**

---

## Prerequisites

If you're working locally with Anaconda, ensure the required libraries are installed. Use the following commands:

```bash
# Install yfinance
pip install yfinance==0.1.67

# Install required libraries
mamba install bs4==4.10.0 -y
mamba install html5lib==1.1 -y
pip install lxml nbformat
```

Ensure your Python environment satisfies these dependencies:
- Python version: 3.7
- Libraries:
  - `yfinance`
  - `pandas`
  - `bs4` (BeautifulSoup)
  - `html5lib`
  - `lxml`
  - `plotly`

---

## Project Tasks

### 1. Define a Function that Makes a Graph
This reusable function creates a dual-subplot graph:
- Top plot: Historical Share Prices
- Bottom plot: Historical Revenues

The function takes:
- A DataFrame containing stock data with `Date` and `Close` columns.
- A DataFrame containing revenue data with `Date` and `Revenue` columns.
- A string indicating the stock's name.

### 2. Extract Stock Data Using `yfinance`
Retrieve historical stock data for Tesla and GameStop, including:
- Dates
- Closing prices
- Volume

### 3. Extract Revenue Data Using Web Scraping
Utilize `BeautifulSoup` to scrape revenue data for Tesla and GameStop from financial websites. Process the data into clean DataFrames for visualization.

### 4. Plot Tesla and GameStop Stock Graphs
Using the data collected in the previous steps, visualize the historical share prices and revenues for Tesla and GameStop. 

---

## Ignoring Warnings
To suppress unnecessary warnings (e.g., `FutureWarning`), include the following in your code:
```python
import warnings
warnings.filterwarnings("ignore", category=FutureWarning)
```

---

## Outputs

The program generates interactive graphs for:
1. Tesla's historical stock prices and revenues.
2. GameStop's historical stock prices and revenues.

Each graph provides valuable insights into the companies' performance over time.

---

## Estimated Time Needed

**30 minutes**

---

## Notes
- The project uses `plotly` for creating visually appealing and interactive graphs.
- Ensure consistent formatting of your data before plotting to avoid errors.
