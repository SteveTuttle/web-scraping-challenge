# web-scraping-challenge
UNC_data_bootcamp_module_11

## Challenge Description
### Background
> You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

***from the UNC Bootcamp instructions for this challenge***

## Deliverables
This Challenge is comprised of two main parts:
* Deliverable-1: Scrape titles and preview text from Mars news articles.
* Deliverable-2: Scrape and analyze Mars weather data, which exists in a table.

### Deliverable-1: Scrape Titles and Preview Text from Mars News
For this Deliverable, I first opened the Jupyter Notebook I extracted from the starter code folder called __part_1_mars_news.ipynb__ and renamed it __part_1_mars_news_SDT.ipynb__. Then followed the steps from both this code and challenge instructions listed below, to scrape the _Mars News_ website.

1) Use automated browsing (created during setup) to visit the [Mars News site](https://static.bc-edx.com/data/web/mars_news/index.html) and inspect the page to identify which elements to scrape.

    * __Hint:__ To identify which elements to scrape, you might want to inspect the page by using Chrome DevTools.

2) Create a Beautiful Soup object and use it to extract __text elements__ from the website.

3) Extract the __titles and preview text__ of the news articles that you scraped. Store the scraping results in Python data structures as follows:

* Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: _title_ and _preview_.

***An example is this would be:***

```
{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
```

* Store all the dictionaries in a Python list.

* Print the list in your notebook.

4) Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file.


### Deliverable-2: Scrape and Analyze Mars Weather Data
For the next Deliverable, I opened  the Jupyter Notebook from the starter code folder named __part_2_mars_weather.ipynb__ and renamed it __part_2_mars_weather_SDT.ipynb__. Again following the steps from both this code and challenge instructions listed below to scrape and analyze Mars weather data.

1) Again, use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html) to inspect the page and identify which elements to scrape. Note that the URL is _https://static.bc-edx.com/data/web/mars_facts/temperature.html_.

    * __Hint:__ To identify which elements to scrape, you might want to inspect the page by using Chrome DevTools to discover whether the table contains usable classes.

2) Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas _read_html_ function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

3) Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
  * __id__: the identification number of a single transmission from the Curiosity rover
  * __terrestrial_date__: the date on Earth
  * __sol__: the number of elapsed sols (Martian days) since Curiosity landed on Mars
  * __ls__: the solar longitude
  * __month__: the Martian month
  * __min_temp__: the minimum temperature, in Celsius, of a single Martian day (sol)
  * __pressure__: The atmospheric pressure at Curiosity's location

4) Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate _datetime_, _int_, or _float_ data types.

    * __Hint:__ You can use the Pandas _astype_ and _to_datetime_ methods to accomplish this task.

5) Analyze your dataset by using Pandas functions to answer the following questions:
  * How many months exist on Mars?
  * How many Martian (and not Earth) days worth of data exist in the scraped dataset?
  * What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    * Find the average minimum daily temperature for all of the months.
    * Plot the results as a bar chart.
  * Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    * Find the average daily atmospheric pressure of all the months.
    * Plot the results as a bar chart.
  * About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    * Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    * Visually estimate the result by plotting the daily minimum temperature.

6) Export the DataFrame to a CSV file.



## Resources
### Bootcamp References
Module 11 Instructions

starter_code
* part_1_mars_news.ipynb
* part_1_mars_weather.ipynb

Example Data:


***Special Thanks:***
* Jamie Miller
* Mounika Mamindla
* Lisa Shemanciik

### External References
_(where possible will provide link to website)_
* [pandas documentation](https://pandas.pydata.org/docs/reference/general_functions.html)
* [Beatiful Soup documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
* [Splinter documentation](https://splinter.readthedocs.io/en/latest/)
* [Mozilla: HTML documantion](https://developer.mozilla.org/en-US/docs/Learn/HTML)
* [Mozilla: Element documantion](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
* [Mozilla: CSS documantion](https://developer.mozilla.org/en-US/docs/Learn/CSS)
* [Google](https://www.google.com)
* [YouTube](https://www.youtube.com)

