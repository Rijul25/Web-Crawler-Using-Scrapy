# Web-Crawler-Using-Scrapy
Scraping data of websites using Scrapy and shell .

Scrapy is written in Python. If you’re new to the language you might want to start by getting an idea of what the language is like, to get the most out of Scrapy.

## Creating a project
Before you start scraping, you will have to set up a new Scrapy project. Enter a directory where you’d like to store your code and run:

- scrapy startproject tutorial

This will create a tutorial directory with the following contents:
tutorial/
    scrapy.cfg            # deploy configuration file

    tutorial/             # project's Python module, you'll import your code from here
        __init__.py

        items.py          # project items definition file

        middlewares.py    # project middlewares file

        pipelines.py      # project pipelines file

        settings.py       # project settings file

        spiders/          # a directory where you'll later put your spiders
            __init__.py
            
*Spiders are classes that you define and that Scrapy uses to scrape information from a website (or a group of websites). They must subclass Spider and define the initial requests to make, optionally how to follow links in the pages, and how to parse the downloaded page content to extract data.*

## How to run our spider
- scrapy crawl quotes

- pip3 install scrapy
- !scrapy startproject myscrapyproject
- scrapy shell 'http://quotes.toscrape.com/page/1/'
- scrape the data and save it in a json file
- run using scrapy crawl your_file_name , this should be from the directory of your project

## For Further reading and documentation refer to ->
> https://docs.scrapy.org/en/latest/intro/tutorial.html
