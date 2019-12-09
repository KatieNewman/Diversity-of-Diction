# Diversity-of-Diction
A project using Natural Language Processing to Analyze Mediums of Creative Writing


# Tools

Python3

BeautifulSoup from bs4

requests

os

pandas

pymongo

urlopen from urllib.request

re

numpy

nltk

sqlite3

create_engine from sqlalchemy

Plotly.js

Flask

ObservableHQ


Sites (examples):

https://www.genius.com\

http://www.famouspoetsandpoems.com\

https://www.theguardian.com\

https://www.nytimes.com\



# Data
Three mediums of creative writing were analyzed: song lyrics, poems, and journal articles. Five well-known works for five top artists were selected for analysis. A process of "web scrapping" was used to obtain the words for each of the 75 works. Tools like Beautiful Soup, Python, Urllib, and Requests were used to parse the HTML of the websites containing the works. This gave us a vast amount of text for us to clean.



# Cleaning the Data
Once we had the necessary text, we had to clean it before we could preform any analysis. This included removing stop words (commonly used words that are considered useless) and converting all text to lowercase. The unique, non-stop words remaining after the cleaning were loaded into a csv file, which we then converted into a sqlite database.




