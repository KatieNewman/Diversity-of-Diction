<img width="695" alt="DiversityofDiction" src="https://user-images.githubusercontent.com/46386265/72846560-d1136600-3c6e-11ea-8cb3-dd0196dff19a.PNG">

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
Three mediums of creative writing were analyzed: song lyrics, poems, and journal articles. Five well-known works for five top artists were selected for analysis. A process of "web scrapping" was used to obtain the words for each of the 75 works. Tools like Beautiful Soup, Python, Urllib, and Requests were used to parse the HTML of the websites containing the works. This gave us a vast amount of text to clean.


# Cleaning the Data
Once we had the necessary text, we had to clean it before we could preform any analysis. This included converting all text to lowercase (to ensure all words were counted as the same word, regardless of capitalization) and removing stop words (commonly used words that are considered useless). The words remaining after the cleaning process were counted for frequency of use per work, which we then converted into a csv file and a sqlite database. 

<img width="798" alt="text to csv" src="https://user-images.githubusercontent.com/46386265/72860358-8efd1b00-3c94-11ea-9b80-b7e3ce6503e6.PNG">


# Analysis
Using Python, pandas, and ObservableHQ, we were able to create visualizations to display the answers to our questions.


  1. Which form of creative writing appears to have the broadest vocabulary?

We calculated the ratio of unique words out of the total words used for each work, then used this to make comparisons across both works and groups of works. We chose to use this ratio as a method of normalization prior to comparison because we expected and verified that the word count of journalists' articles was far greater than that of the other groups. We obtained the following scores for percentage of unique words out of total words used:

Journalists: approx. 42.966%
Poets: approx. 33.086%
Songwriters: approx. 21.687%


  2. What are the most commonly used words among creative writing groups? Authors?
  
We created a bubble chart to visually show which words were most frequently used across all works.

<img width="569" alt="new bubble chart" src="https://user-images.githubusercontent.com/46386265/72952912-57a87000-3d61-11ea-9cdf-1a8a0a0b78a7.PNG">
  
Blue = journal articles

Green = poems

Orange = song lyrics

Each circle size corresponds to the frequency of a words usage in a work. Please note, that words may appear more than once as each bubble shown only represents one word per work.

Below is a collapsible tree which shows the most frequently used words per writer per work.

![collapsible-tree](https://user-images.githubusercontent.com/46386265/72837485-8be63880-3c5c-11ea-99d6-67870ca9e0e9.png)

# In Conclusion

Journalists had the widest vocaublary among the three creative writing medium, using over 300 words per text on average.  
