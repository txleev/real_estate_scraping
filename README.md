# Apartment Scraping

A Python project to scrape apartment listings from [House.kg](https://www.house.kg/kupit-kvartiru), extract key details (rooms, area, floor, address, prices in USD and Kyrgyz Som), and save the results to a CSV file.

---

## Table of Contents

1. [Features](#features)  
2. [Prerequisites](#prerequisites)  
3. [Installation](#installation)  
4. [Usage](#usage)  
5. [Notebook Structure](#notebook-structure)  
6. [Configuration](#configuration)  
7. [Output](#output)  
8. [Author](#author)  
9. [License](#license)  

---

## Features

- Fetch multiple pages (default: first 5 pages) of apartment listings  
- Parse HTML with BeautifulSoup (`lxml` parser)  
- Extract:
  - Number of rooms  
  - Area (m²)  
  - Floor (handles basement “цоколь”)  
  - Address (split by comma)  
  - Price in USD and in Kyrgyz Som  
- Store data in a `pandas` DataFrame  
- Export to CSV  

---

## Prerequisites

- Python 3.6+  
- `requests`  
- `beautifulsoup4`  
- `lxml`  
- `pandas`  

You can install all dependencies with:

```bash
pip install requests beautifulsoup4 lxml pandas
