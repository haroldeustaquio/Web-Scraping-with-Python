# Hacker News Scraper

## Project Description

This project consists of a **web scraper** that extracts basic information from posts on the [Hacker News](https://news.ycombinator.com/) homepage. The goal is to capture the **titles**, **href**,**points**, **rated by**, **hours ago**, **comments**.

This scraper is designed as a basic web scraping project using:
- *Pandas*
- *numpy*
- *BeautifulSoup*
- *Requests*

---
## Project Structure

- `scraper.ipynb`: The main scraper file, which contains the code to extract data.
- `data.csv`: The processed data obtained from the page
- `README.md`: This file that explains how the project works and how to use it.

---
## Challenges Faced

During the development of this web scraper, several challenges were encountered:

- `Handling Page Failures`: Some pages returned errors or did not load properly. This required the implementation of error handling to ensure the scraper could continue functioning even when a particular page failed to load. By checking the status of the page, the scraper could skip failed attempts and move on to the next page.

- `Data Extraction Issues`: Not all posts contained the same metadata, and some elements were missing from the HTML structure. To address this, a robust error handling strategy using `try-except blocks` was implemented to ensure that missing data did not cause the entire scraping process to fail. Instead of halting, the scraper would assign `NaN` values to any missing information, allowing for a more complete dataset.

---

## Project Results

The following table illustrates a sample of the data extracted from Hacker News:

| title                                                                                                   | href                                                   | points | by          | hours ago | comments |
|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------|--------|-------------|-----------|----------|
| DeskPad – A virtual monitor for screen sharing                                                          | (https://github.com/Stengo/DeskPad)            | 873    | geerlingguy | 18        | 121      |
| Nurdle Patrol                                                                                          | (https://www.nurdlepatrol.org/app/)             | 43     | amar-laksh  | 5         | 2        |
| The Copenhagen Book: general guideline on implementing auth in web applications                       | (https://thecopenhagenbook.com/)               | 528    | sebnun      | 16        | 129      |
| AAA Gaming on Asahi Linux                                                                              | (https://rosenzweig.io/blog/aaa-gaming-on-m1.html) | 699    | 6a74        | 21        | 233      |
| Scuda – Virtual GPU over IP                                                                             | (https://github.com/kevmo314/scuda)            | 84     | kevmo314    | 7         | 15       |

