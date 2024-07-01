# Basic-Web-Scraper

import requests
from bs4 import BeautifulSoup

req = requests.get("https://codewithharry.com")

soup = BeautifulSoup(req.content, "html.parser")

print(soup.prettify())
