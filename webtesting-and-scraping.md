---
layout: page
title: Web Testing and Scraping with Modern Python Tools
permalink: /web-testing/
---

This course is a one day course on learning the basics of functional web testing and web
scraping with industry standard courses. It can be taught on-site or premises. The course
contents can be tailored to your specific needs and requirements.

This course assumes a basic knowledge of Python scripting but it doesn't require full knowledge of
the lanugage or object oriented programmers. It's suitable for beginner programmers or
those migrating from a testing role to a web programming role. It's often delivered as a
follow-on course form [Practical Python](/practical-python) or
[Beginning Python](/beginning-python).

I've been building web applications commercially for four years, and working with web apis
interating with sites via selenium for even longer that that. The techniques on this
course will teach you to make and fetch API requests for API testing, using selenium to
interact with a website as a user and extract all the useful information
from this, even from Javascript generated sites, using ``BeautifulSoup``.

* [Contact Details for Webtesting Tools and Techniques](mailto:michael@python.org)

An essential part of testing any modern web application is "black box testing", sometimes called "fucntional testing".
Interacting with the website as if you were a user. This gives you two insights:

1. What hoops do our users actually have to jump through to use our website, could they
   be easier or bettter designed for a better user experience (UX)?
2. Does our website acutally work! Can users perform the actions they need without bugs!

Finding bugs on your staging website with an automated testing suite using selenium is
*waaaay* less embarrassing than having your customers discover them live on site. Minimal
sets of tests can even be deleloped as "gating checks" for commits to master, making  it
less likely that fundamentlly broken code can be delivered to production.

For for functional tests speed of test run is always a trade-off against how much detail
to test functionality in. This trade-off is one of the things we discuss and consider in
this course.

The same, or similar, tools and techniques can be used for testing web apis.

The Python ecosystem has several powerful tools for working with websites and examining the
results. They can be used both for the testing of web applications and for scraping data
from live websites. Even though they're Python tools they can be used for working with
websites built in any lanugage or system.

The three powerful and easy to learn Python tools for these tasks are:

* [Requests](http://docs.python-requests.org/en/master/)

  A simple and powerful library for handling http requests and responses, including
  full json and authentication support, making it excellent for API testing.

* [Selenium Webdriver](https://selenium-python.readthedocs.io/)

  Selenium provides a very powerful API for communicating from Python with a real
  browser. The full details are very rich and complex, but the basic principles
  are very easy to learn. Selenium works well with dialogs, fully Javascript generated
  sites and sites in iframes.

* [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)

  Selenium provides a wonderful way of interacting with websites, but a terrible way
  of looking extesnively into the data they contain and pulling out the useful parts
  in a structured way. Fortunately ``BeautifulSoup`` is excellent for this and plays
  very well with ``Selenium``.

This course teaches these three tools and how to use them together for both powerful
web functional testing, including interacting with all the standard form elements
and even how to use it for a Test Driven Development tool. It also covers pulling out
and organising structured data from webpages, useful for both web testing and web
scraping. It includes looks at both XPATH and CSS queries which are essential for
finding and navigating elements on a web page.

We'll cover the Python csv module for outputting data and as an added bonus we may look
at the combination of [Pandas](https://pandas.pydata.org/pandas-docs/stable/)
and [openpyxl](https://openpyxl.readthedocs.io/en/stable/) for writing data out as Excel
compatible files.


Web Testing  with BeautifulSoup and Selenium
---------------------------------------------

The goal of this day is to teach the principles and nuts and bolts of interacting with
Javascript rendered sites using Python and third party library. By the end of the day attendees will be able to create simple scripts and programs that can visit websites, interact with them by entering search terms and navigating the site, and pull out structured data that can be written to data files on the computer. The advanced details of using CSS selectors and XPATH to pull out the data won’t be covered in full, as these are huge topics, but enough information to work with most websites will be provided. Along the way tips and techniques will be delivered to enable attendees to self-teach and work out for themselves, with a little help from google, more complex scenarios. Sample data will be provided for attendees to wrestle with some moderately complex examples.

BeautifulSoup
-------------

* Making a web request with the requests module
* Making and receiving JSON API requests with requests
* Understanding web pages with BeautifulSoup
* Extracting data by tag and the tag type
* A note about parsers (html_parser, lxml and html5lib)
* Navigating the DOM (Document Object Model)
* Where’s my data? Attributes on tags
* Pulling data out into Python objects and writing it to files

Selenium
--------

* Launching a real browser from Python and the interactive interpreter
* The basic API: navigating a site, finding elements, extracting data
* More advanced interactions: clicking links and buttons, entering text, selecting radio buttons, scrolling into view, iframes (etc)
* Navigating a website from a Python program
* CSS selectors and XPATH. View source is your friend
* Why do we have to wait? Javascript rendered sites, some practical techniques
* Show me the source: how we view real html (the DOM) from a Javascript website

Best of Friends: BeautifulSoup with Selenium
--------------------------------------------

In this section we will pull together what we’ve learned of the Python programming
language, and both BeautifulSoup and selenium to extract structured data from complex
websites.

* Fetching a page with selenium and handling it with BeautifulSoup
* Pulling out data into Python collections and re-structuring the data with simple loops and data processing
* Formatting the data for output and writing files
* Debugging techniques and exploratory sessions
* Further examples of using the selenium API to navigate and interact with websites and using the combination of CSS selectors, XPATH and the BeautifulSoup API to work only with the data we’re interested in
* Better ways to work with structured data using the pandas library and different output formats (optional topic)
