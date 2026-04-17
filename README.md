# Project Name: Image 1993 Web Scraper

### 1. Project Overview

* **Target Website:** https://pk.image1993.com/collections/ready-to-wear
* **Data Fields Extracted:** Title, Product Link, Page Number
* **Tools Used:** Python, requests, BeautifulSoup, pandas, time

---

### 2. Setup Instructions

1. Clone this repository:
https://github.com/mubashranoor04/image-1993-web-scraper

2. Install dependencies:
pip install -r requirements.txt

3. Run the script:
python scraper.py

### 3. Challenges & Solutions

* One challenge was that the website contains many repeated links and unnecessary elements such as navigation items.  
To solve this, I filtered only product-related links using `"/products/"` and removed duplicates using a dictionary based on unique URLs.

* Another challenge was handling pagination.  
I solved this by dynamically generating URLs for multiple pages using a loop.

* The script also includes basic error handling to manage failed requests and ensure the scraper continues running without interruption.

---

### 4. Output

The scraped data is saved in a CSV file named `data.csv`, which contains:

* Product Title
* Product Link
* Page Number

---

### 5. Ethical Considerations

To follow ethical scraping practices, a delay of 1 second (`time.sleep(1)`) was used between requests to avoid overloading the website server and ensure responsible scraping behavior.

---

### 6. Notes

This project was built as part of a Data Science assignment to demonstrate web scraping, data extraction, and GitHub workflow management.