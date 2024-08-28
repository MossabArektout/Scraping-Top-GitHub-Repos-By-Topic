# Top Repos For GitHub Topics

## Overview

This project is designed to scrape information about top repositories related to various GitHub topics. The information collected includes topic titles, descriptions, and URLs, as well as the top repositories for each topic. For each repository, we collect the repository name, username, star count, and repository URL.

## Plan

1. **Scrape Topics Information**
   - Extract the title, description, and URL of each topic from the GitHub Topics page.

2. **Scrape Top Repositories for Each Topic**
   - For each topic, gather the top 18 repositories, including the repository name, username, star count, and repository URL.

## Requirements

- Python 3.x
- `requests` library
- `beautifulsoup4` library
- `pandas` library

## Installation

You can install the required libraries using pip:

```bash
pip install requests beautifulsoup4 pandas
```
## Usage
### 1 - Scrape Topics Information

The `topics()` function scrapes the GitHub Topics page and returns a DataFrame with the topic titles, descriptions, and URLs.

### 2 - Scrape Top Repositories for a Specific Topic

The `get_topic_repos()` function extracts repository information from the topic page. It gathers the repository name, username, star count, and URL.

### 3 - Save Data to CSV

The `scrape_topic()` function saves the top repositories' data for a specific topic to a CSV file.

### 4 - Run the Scraper

The `scrape_topics_repos()` function coordinates the scraping process for all topics and saves the data into separate CSV files in the data directory.

## Notes

- Make sure you have the required libraries installed before running the code.
- The `scrape_topics_repos()` function will create a data directory and save CSV files for each topic in it.

- The code assumes that the structure of the GitHub Topics page remains unchanged. If GitHub updates their page layout, adjustments to the scraping logic may be required.

## License

This project is licensed under the MIT License.


 - Feel free to adjust the content or formatting as needed!
