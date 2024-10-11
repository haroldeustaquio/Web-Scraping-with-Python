# IMDb Top 250 Scraper

## Project Description

This project consists of a **web scraper** that extracts basic information from the [IMDb Top 250](https://www.imdb.com/chart/top/) movies list. The goal is to capture the **title**, **year**, **duration**, **star rating**, **number of reviewers**, and **image URL**.

The scraper is built using:
- *Selenium* (for navigating the website and extracting data)
- *Pandas* (for organizing the data into a structured format)

---

## Project Structure

- `scraper.ipynb`: The main notebook containing the code to scrape the IMDb Top 250 movies.
- `data.csv`: The processed data with information about the top 250 movies.
- `README.md`: This file, which explains how the project works and how to use it.

---

## Challenges Faced

During the development of this IMDb scraper, a few challenges arose:

- **Dynamic Content Handling**: IMDb loads its page dynamically, so traditional scraping methods using libraries like `Requests` and `BeautifulSoup` were insufficient. To handle this, we used **Selenium** to interact with the page as if a user was navigating, ensuring all elements were loaded before extraction.

- **Data Structure Variations**: While most movie entries followed a consistent format, some slight variations in how movie data was displayed required conditional logic in the extraction process. This was addressed using structured XPath selectors to ensure we accurately captured all movie details.

---

## Project Results

The following table illustrates a sample of the data extracted from IMDb:

| title                     | year | duration | stars | people  | image_url                                                                 |
|---------------------------|------|----------|-------|---------|--------------------------------------------------------------------------|
| Cadena perpetua            | 1994 | 2h 22m   | 9.3   | 2.9 M   | [Image](https://m.media-amazon.com/images/M/MV5BMTA1MjE0Nzk4MDleQTJeQWpwZ15BbWU4MDA0NjIxMjAx._V1_QL75_UY207_CR6,0,140,207_.jpg)  |
| El padrino                 | 1972 | 2h 55m   | 9.2   | 2.1 M   | [Image](https://m.media-amazon.com/images/M/MV5BNWYxYzc1ZTAtNzM4Ni00MTUwLTliYmMtNWUwOWMzM2M3MjY3XkEyXkFqcGc@._V1_QL75_UY207_CR3,0,140,207_.jpg) |
| El caballero oscuro        | 2008 | 2h 32m   | 9.0   | 2.9 M   | [Image](https://m.media-amazon.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_QL75_UX140_CR0,0,140,207_.jpg)  |
| El padrino parte II        | 1974 | 3h 22m   | 9.0   | 1.4 M   | [Image](https://m.media-amazon.com/images/M/MV5BMjQ5MzQxZTEtMmE1Yy00NjZlLTk5ODItNjI3MWIxMjk1M2U5XkEyXkFqcGc@._V1_QL75_UY207_CR10,0,140,207_.jpg) |
| 12 hombres sin piedad      | 1957 | 1h 36m   | 9.0   | 887 mil | [Image](https://m.media-amazon.com/images/M/MV5BYThhOGFhODktNGEwNi00MzY2LTg3YWYtNzAzZTE0MTFlMWQxXkEyXkFqcGc@._V1_QL75_UY207_CR2,0,140,207_.jpg) |
