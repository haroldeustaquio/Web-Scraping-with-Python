# GitHub Scraper

## Project Description

This project consists of a **web scraper** that extracts user information and repository details from a GitHub profile page. The goal is to capture the **full name**, **description** of the user, and repository data such as **name**, **URL**, **description**, **programming language**, **stars**, **forks**, **license**, and **last update**.

This scraper is designed as a basic web scraping project using:
- *Pandas*
- *NumPy*
- *Selenium*
- *WebDriver*

---

## Project Structure

- `scraper.ipynb`: The main scraper file, which contains the code to extract data.
- `user_info.csv`: The processed user data obtained from the GitHub profile.
- `repos_info.csv`: The processed repository data obtained from the profile.
- `README.md`: This file explains how the project works and how to use it.

---

## Challenges Faced

During the development of this web scraper, several challenges were encountered:

- **Handling Page Failures**: Occasionally, pages would not load properly or time out. To handle this, the script includes error-handling mechanisms to continue execution even if a page fails. Selenium's `WebDriverWait` was used to manage page loads and ensure that key elements were present before attempting data extraction.

- **Incomplete Data**: Not all repositories contained the same metadata (e.g., some lacked descriptions, stars, or licenses). A robust error-handling strategy was implemented using `try-except` blocks to assign `NaN` values to any missing information. This ensured that the scraping process could continue without halting due to incomplete data.

---

## Project Results

The following table illustrates a sample of the data extracted from the GitHub profile:

### Preview User Information

| full_name       | description                                                                                             |
|-----------------|---------------------------------------------------------------------------------------------------------|
| Harold Eustaquio | "Electronic and Computer Engineering student, passionate about Data Analysis, Machine Learning, Deep Learning, and Big Data 💻" |

### Preview Repositories Information

| repo_name                            | repo_url                                                           | repo_desc                                                                                                                       | repo_lenguaje    | stars | forks | license      | last_update                  |
|--------------------------------------|--------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|-----------------|-------|-------|--------------|-----------------------------|
| SQL-Coding-Challenges                | https://github.com/haroldeustaquio/SQL-Coding-Challenges            | "Repository dedicated to solving SQL problems from HackerRank and other challenges. Contains solutions to improve skills..."    | TSQL            | 5     | 1     | MIT License  | Oct 13, 2024, 3:10 PM CST   |
| Python-Coding-Challenges             | https://github.com/haroldeustaquio/Python-Coding-Challenges         | "Repository dedicated to solving Python problems from LeetCode, DataLemur and other programming challenges."                   | Jupyter Notebook | 6     |       | MIT License  | Oct 13, 2024, 5:00 AM CST   |
| Melody-Lyric-Generator-from-Sheet-Music | https://github.com/haroldeustaquio/Melody-Lyric-Generator-from-Sheet-Music |                                                                                                                                 | Python          |       | 1     |              | Oct 13, 2024, 2:31 AM CST   |
| Machine-Learning                     | https://github.com/haroldeustaquio/Machine-Learning                 | "This repository contains Machine Learning mini-projects focused on different predictive models, from linear regression to..."  | Jupyter Notebook | 6     |       | MIT License  | Oct 13, 2024, 2:13 AM CST   |
| Web-Scraping-with-Python             | https://github.com/haroldeustaquio/Web-Scraping-with-Python         |                                                                                                                                 | Jupyter Notebook |       |       |              | Oct 12, 2024, 11:51 PM CST  |