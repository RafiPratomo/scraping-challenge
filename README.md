# Mars Weather Data Scraping and Analysis

This repository contains a Python script to scrape and analyze Mars weather data from a static web page. The task includes web scraping using `Splinter` and `BeautifulSoup`, data processing with `Pandas`, and data visualization using `Matplotlib`.

## Deliverable 1: Scrape Titles and Preview Text from Mars News

### Steps:
1. **Visit the Website:**
   - Automated browsing to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html).
2. **Scrape the Website:**
   - Create a Beautiful Soup object and extract text elements from the website.
3. **Store the Results:**
   - Extract titles and preview text of news articles.
   - Store each title and preview pair in a dictionary and add it to a list.

## Deliverable 2: Scrape and Analyze Mars Weather Data

### Steps:
1. **Visit the Website:**
   - Automated browsing to visit the [Mars weather data site](https://static.bc-edx.com/data/web/mars_facts/temperature.html).
2. **Scrape the Table:**
   - Create a Beautiful Soup object and scrape the data in the HTML table.
3. **Store the Data:**
   - Assemble the scraped data into a Pandas DataFrame with the appropriate column headings.
4. **Prepare Data for Analysis:**
   - Examine and change data types for each column to appropriate `datetime`, `int`, or `float` data types.
5. **Analyze the Data:**
   - Analyze the dataset to answer specific questions about Mars weather data.
   - Visualize the results using Matplotlib.
6. **Save the Data:**
   - Export the DataFrame to a CSV file.

### Usage

1. **Setup:**
   - Ensure you have `chromedriver` installed and the path set correctly in the script.
   - Install required Python packages:
     ```sh
     pip install splinter beautifulsoup4 pandas matplotlib
     ```

2. **Run the Script:**
   - Execute the script to scrape and analyze the Mars weather data.
     ```sh
     python mars_weather_scraping.py
     ```

3. **View Results:**
   - The script will output the results of the analysis and save the data to `mars_weather_data.csv`.

### Script Explanation

- **Scrape Titles and Preview Text:**
  - Uses `Splinter` to automate browser actions and `BeautifulSoup` to parse HTML and extract text data.
- **Scrape and Analyze Weather Data:**
  - Visits the specified URL, scrapes the weather data table, processes the data into a Pandas DataFrame, and performs various analyses including data type conversion, average calculations, and visualizations.
