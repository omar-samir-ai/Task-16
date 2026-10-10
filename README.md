Web Scraping and Browser Automation with Selenium

This repository contains two small projects built with Python and Selenium. The first collects product data from a Carrefour Egypt category page. The second automates posting a text message on Facebook.

Task 1: Carrefour Products Scraper

The scraper opens the “Fruits and Vegetables” category page on Carrefour Egypt, scrolls down so all products load, and collects the data for each product.

Collected data:

Product name
Product price
Product URL

Bonus data:

Product image links
Discount products, with the old price and the price after the discount
Product category

The main data is saved to a CSV file and a JSON file.

Files:

source_code_task1.ipynb: the code
requirements_task1.txt: required libraries
carrefour_products_task1.csv and carrefour_products_task1.json: the output
screenshots_task1: screenshots of the output
Task 2: Facebook Post with Selenium

The script opens Facebook, logs in to an account I own, opens the post box, writes a text post, and publishes it. Facebook may ask for login approval from another device. In that case the code pauses until the approval is done.

Files:

source_code_task2.ipynb: the code
requirements_task2.txt: required libraries
screenshots_task2: screenshots of each step

Note: the email and password in the code are placeholders. Replace them with your own account details before running.

Libraries Used
selenium
time, csv, and json (built into Python)
How to Run
Install Python and Mozilla Firefox.
Install the required libraries:
pip install -r requirements_task1.txt
Open the notebook of the task you want in Jupyter Notebook or VS Code.
Run the cells in order.
For Task 2, put your own email and password in the login cell, and approve the login from your phone if Facebook asks.
Example Output

Task 1 produces records like this:

Product Name: تفاح من رويال جالا
Old Price: 52.50
New Price: 47.50
Category: الخضار والفواكه

Task 2 publishes this post on the account:

I am taking the AI course with Eng.Ahmed Hafez
Notes
Facebook and Carrefour change their page structure from time to time, so some selectors may need to be updated.
Use only an account you own or are authorized to use.
