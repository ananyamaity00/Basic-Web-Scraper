# Basic-Web-Scraper 
# A basic web scraper in Python extracts data from websites for analysis or automation tasks.

import requests

from bs4 import BeautifulSoup

req = requests.get("https://codewithharry.com")

soup = BeautifulSoup(req.content, "html.parser")

print(soup.prettify())
