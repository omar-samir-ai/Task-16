# Web Scraping and Browser Automation with Selenium

This repository contains two small projects built with Python and Selenium. The first collects product data from a Carrefour Egypt category page. The second automates posting a text message on Facebook.

---

## Task 1: Carrefour Products Scraper

**What it does:** Opens the "Fruits and Vegetables" category page on Carrefour Egypt, scrolls down until all products load, then collects the data for each product and saves it to files.

**Collected data:**
- Product name
- Product price
- Product URL

**Bonus data:**
- Product image links
- Discount products, with the old price and the price after the discount
- Product category

**Libraries used:** `selenium`, plus `time`, `csv`, and `json` (built into Python).

**How to run:**
1. Install Python and Mozilla Firefox.
2. Install the requirements:
```
   pip install -r requirements_task1.txt
```
3. Open `source_code_task1.ipynb` in Jupyter Notebook or VS Code.
4. Run the cells in order.

**Example output:**
```
Product Name: تفاح من رويال جالا
Old Price: 52.50
New Price: 47.50
Category: الخضار والفواكه
```

**Files:**
- `source_code_task1.ipynb`: the code
- `requirements_task1.txt`: required libraries
- `carrefour_products_task1.csv` and `carrefour_products_task1.json`: the saved output
- `screenshots_task1/`: screenshots of the output

---

## Task 2: Facebook Post with Selenium

**What it does:** Opens Facebook, logs in to an account I own, opens the post box, writes a text post, and publishes it. If Facebook asks for login approval from another device, the code pauses until the approval is done.

**Steps performed:**
- Open Facebook
- Log in
- Click the post box
- Type the text
- Publish the post

**Libraries used:** `selenium`, plus `time` (built into Python).

**How to run:**
1. Install Python and Mozilla Firefox.
2. Install the requirements:
```
   pip install -r requirements_task2.txt
```
3. Open `source_code_task2.ipynb` in Jupyter Notebook or VS Code.
4. Put your own email and password in the login cell. The values in the code are placeholders.
5. Run the cells in order, and approve the login from your phone if Facebook asks.

**Example output:**
```
Post published: I am taking the AI course with Eng.Ahmed Hafez
```

**Files:**
- `source_code_task2.ipynb`: the code
- `requirements_task2.txt`: required libraries
- `screenshots_task2/`: screenshots of each step

---
