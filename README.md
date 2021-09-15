## Web Scraper Project

### Date created
September 15th, 2021

### Required Software and Packages
python --version 3.8
  bs4 from BeautifulSoup,
  pandas,
  datetime,
  time,
  csv,
  requests,
  smtplib

### Description
This project was done using Python 3.8 in Jupyter Notebooks. In this project, I utilized the BeautifulSoup package to web scrape an ecommerce website to collect a few data points on a product I am watching; then alert me via email when the price has dropped below my target price range.

I started this project by first using bs4 (from the BeautifulSoup package) and the requests package to extract the data that I desired to monitor; which in this case was: date, title (of the product), price, and rating (out of 5 stars). I then cleaned and exported that data into a csv dataset using the Python csv package. Then I built a function that uses a timer to automatically initiate another web scrape every 24 hours (can easily be changed to any time designation) and append the csv file with the updated data from that day. For convenience, I used the smtplib package to write a function that would send me an email only if the price of the product dropped below my desired price range.

I only used the pandas package in this project to check what I was writing to the csv file without having to open it each time I ran my code.

### Project Objectives
1. Web scrape an ecommerce site to collect the desired data from a product.
2. Clean that data into a more desirable format.
3. Export that data into a csv file.
4. Write a function that uses a timer to automatically append the csv file.
5. Write a function that sends an email when the price has dropped below a    desired price point.

### Files Used
SpikeballWebScraperDataset.csv (created in program)

### Credits
AlextheAnalyst on YouTube
