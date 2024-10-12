# Beginner Scraping

Welcome to the **Beginner Scraping** section of this repository. Here, you'll find projects that introduce the basic concepts of web scraping using Python. The goal of this section is to help you get started with scraping static web pages and simple APIs. I will use beginner-friendly tools and libraries to extract data and process it efficiently.

## 🚀 Tools and Libraries

In this section, I'll focus on three main tools:

1. **`requests`**: 
   - Used for sending HTTP requests to websites. It allows us to retrieve HTML pages or data from APIs.
   - [Documentation](https://docs.python-requests.org/)

2. **`BeautifulSoup`**: 
   - A library for parsing HTML and XML documents. It makes it easy to navigate, search, and modify HTML content.
   - [Documentation](https://www.crummy.com/software/BeautifulSoup/)

3. **`pandas`**: 
   - A powerful data manipulation library used to store and organize the scraped data in structured formats like DataFrames.
   - [Documentation](https://pandas.pydata.org/)

4. **`numpy`**: 
   - A fundamental package for numerical computing in Python. It supports large, multi-dimensional arrays and matrices, and provides a collection of mathematical functions to operate on these arrays.
   - [Documentation](https://numpy.org/)

5. **`selenium`**: 
   - A tool for automating web browsers. It allows you to navigate through web pages, interact with elements, and perform dynamic content scraping.
   - [Documentation](https://www.selenium.dev/documentation/)


## 📂 Project Structure

This directory contains the following projects:

### 1. Hacker News Scraper
- **Goal**: Extract basic information from posts on the [Hacker News](https://news.ycombinator.com/) homepage, including titles, links, points, rated by, hours ago, and comments.
- **Tools Used**: `Pandas`, `numpy`, `BeautifulSoup`, `Requests`.
- **Project Path**: `hacker-news/`

### 2. IMDb Top 250 Scraper
- **Goal**: Extract movie details from [IMDb Top 250](https://www.imdb.com/chart/top/)  (title, year, duration, rating, reviews, and image URL) from IMDb's Top 250 movies page.
- **Tools Used**: `Selenium`, `pandas`
- **Project Path**: `IMDb/`

Each project has its own directory with a detailed `README.md` explaining how the scraper works and how to run the code.

