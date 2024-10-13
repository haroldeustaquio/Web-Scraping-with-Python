# Worldometers Scraper

## Project Description

This project consists of a **web scraper** that extracts key metrics from the [Worldometers](https://www.worldometers.info/) website, which provides real-time statistics on global population and other critical data. The objective is to capture various **metrics** and their corresponding **counts**, such as the current world population, births, and deaths.

The scraper is built using:
- *Selenium* (for automating the browser interaction and extracting data)
- *Pandas* (for organizing the extracted data into a structured format)

---

## Project Structure

- `scraper.ipynb`: The main notebook containing the code to scrape metrics from Worldometers.
- `data.csv`: The processed data, which includes key metrics and their current counts.
- `README.md`: This file, which explains how the project works and how to use it.

---

## Challenges Faced

Throughout the development of this scraper, several challenges were encountered:

- **Dynamic Content Updates**: Worldometers updates its data in real-time, requiring the scraper to handle frequently changing content. To address this, **Selenium** was used to ensure the data was captured at a specific point in time, allowing for consistent extraction.
  
- **Data Format Handling**: The data extracted from the site was formatted with commas (e.g., "8,181,967,470" for population). **Pandas** was leveraged to clean and format these numbers appropriately for further analysis.

---

## Project Results

The following table shows a sample of the data extracted from Worldometers:

| metric                         | count          |
|---------------------------------|----------------|
| Current World Population        | 8,181,967,470  |
| Births this year                | 103,743,623    |
| Births today                    | 357,297        |
| Deaths this year                | 48,884,482     |
| Deaths today                    | 168,360        |
| Net population growth this year | 54,859,142     |

