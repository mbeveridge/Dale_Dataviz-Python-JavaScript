# Data Visualization with Python & JavaScript
#### Scrape, Clean, Explore & Transform your Data
###### Kyran Dale

---

Publisher's [web page for this book](http://shop.oreilly.com/product/0636920037057.do), including [errata](https://www.oreilly.com/catalog/errata.csp?isbn=0636920037057)

[Page xi] Author's [GitHub repo](https://github.com/Kyrand/dataviz-with-python-and-js) ...includes "Note - D3 version 4" comments


| Directory or file (in root) | Explanation |
| --- | --- |
| dataviz-with-python-and-js-master/ | [Chapter1] Latest version of author's GitHub repo, on 9/5/2019 |
| README.md | This document |

---

### 01. Development Setup *[P.1-8]*

## Part I. Basic ToolKit *[P.9-123]*

### 02. A Language-learning Bridge between Python & JavaScript *[P.11-55]*

*P.51-54 : "A Cheat Sheet" : "a set of cheat sheets to translate basic operations between Python and JavaScript"*

Summary : *"most common idioms and patterns from one of the languages can be expressed in the other without too much fuss. The meat and potatoes of programming, iteration, conditionals, and basic data manipulation is simple in both languages, and the translation of functions is straightforward"*


### 03. Reading & Writing Data with Python *[P.57-84]*

Summary : *"This chapter aimed to make you comfortable using Python to move data around the various file formats and databases that a data visualizer might expect to bump into ... [Y]ou should now be comfortable with basic reading and writing for the large majority of dataviz use cases."*


### 04. Webdev 101 *[P.85-123]*

* P.107-122 : *Primer in SVG*

Summary : *"This chapter provided a basic set of modern web-development skills for the budding data visualizer. ... We also covered Chrome’s Elements and Sources tabs, which are the key browser development tools. Finally we had a little primer in SVG."*


## Part II. Getting Your Data *[P.125-190]*

### 05. Getting Data off the Web with Python *[P.127-156]*

Summary : *"In this chapter, we’ve seen examples of the most common ways in which data can be sucked out of the Web and into Python containers, databases, or Pandas datasets. Python’s `requests` library is the true workhorse ... For the more awkward APIs, such as those with potentially complicated authorization, a wrapper library like `Tweepy` (for Twitter) can save a lot of hassle. ... We also started our first forays into data scraping"*


### 06. Heavyweight Scraping with Scrapy *[P.157-190]*

Summary : *"In this chapter we produced two `Scrapy` spiders ... Although the workflow requires more effort to implement than doing some hacking with `BeautifulSoup`, Scrapy has far more power and comes into its own as your scraping ambitions increase"*



## Part III. Cleaning and Exploring Data with Pandas *[P.191-317]*

### 07. Introduction to NumPy *[P.193-202]*

Summary : *"This chapter laid the foundations of NumPy, focusing on its building block, the NumPy array or `ndarray` ... Although Pandas hides its NumPy arrays behind data containers such as its `DataFrame` and `Series`, which are adapted to deal with heterogeneous data, these containers behave for the most part like NumPy arrays ... Now that we’ve got its building blocks in place, let’s see how Pandas extends the homogeneous NumPy array into the realm of heterogeneous data, where much of data visualization work takes place"*


### 08. Introduction to Pandas *[P.203-222]*

* P.203 : *"There are certainly visualizations, like network graphs, for which row-columnar data is not the best form, but they are in the minority"*
* P.207-208 : *"There are three ways to select a row from the `DataFrame` ... `ix` is a convenient method, but there is scope for confusion when it’s used with integer axes. If in doubt, it’s best to be explicit and use either `loc` or `iloc`"*
* P.220 (and others) : *shows use of backslash `\`, which is (one way) to wrap long lines in Python*

Summary : *"The core concepts of Pandas —the `DataFrame`, `Index`, and `Series` — were discussed and we saw why Pandas is such a good fit with the type of real-world data that data visualizers deal with, extending the NumPy `ndarray` by allowing the storage of heterogeneous data and adding a powerful indexing system."*


### 09. Cleaning Data with Pandas *[P.223-253]*

* P.225-228 : *"`DataFrame` has a number of methods and properties that give a quick overview of the data" : `info`, `describe`, `head`, `tail`*
* P.229-233 : *Recap of basic Pandas data selection*
* P.241 : *"[T]o change the `country` field of a row ... best practice, which is to use the `ix` (or the more specific `loc` and `iloc`) method" : ` df.ix[709, 'country'] = 'France'` not `df['country'][709] = 'France'`*

Summary : *"In this chapter, you learned how to clean a fairly messy dataset ... [A] number of new Pandas methods and techniques were introduced to extend the last chapter’s introduction to basic Pandas"*


### 10. Visualizing Data with Matplotlib *[P.255-284]*

Summary : *"This chapter introduced Matplotlib, Python’s plotting powerhouse. It’s a big, mature library with lots of documentation and an active community ... We saw how Seaborn extends Matplotlib with some useful statistical methods and that it has what many consider to be superior aesthetics"*


### 11. Exploring Data with Pandas *[P.285-317]*

Summary : *"In this chapter, we explored our Nobel Prize dataset ... We used a fair number of Matplotlib (by way of Pandas) and Seaborn’s plots ... We found more than enough stories in the data to suggest a web visualization. In the next chapter we will imagine and design just such a Nobel Prize winner visualization, cherry-picking the nuggets gained in this chapter"*



## Part IV. Delivering the Data *[P.319-357]*

### 12. Delivering the Data *[P.321-337]*

* P.322 : *"A good rule of thumb is to aim to do as much data manipulation as possible with Python - it’s much less painful than equivalent operations in JavaScript. Following from this, the data delivered should be as close as possible to the form it will be consumed in (ie. for D3 this will usually be a JSON array of objects"*
* P.328 : *"Static pages are easy to cache, meaning their delivery can be much faster. It can also be more secure"*
* P.336 : *"As a rough rule of thumb, any dataset less than 200 KB should be fine with purely static delivery"*

Summary : *"This chapter explained the rudiments of static data delivery of files on the web server, and dynamic delivery of data, sketching the basis of a simple Flask-based RESTful web server"*


### 13. RESTful Data with Flask *[P.339-357]*

Summary : *"This chapter showed how Python and Flask can combine with ease to deliver your data to the web browser with a flexible, RESTful API ... [B]eing able to negotiate fine-grained access to a server-side database extends the realm of web dataviz enormously ... We also saw how we’ll use Flask Eve to deliver the winners’ data ... In the next chapter we’ll see how that data is used"*


## Part 5. Visualizing Your Data with D3 *[P.359-]*

### 14. Imagining a Nobel Visualization *[P.361-370]*

Summary : *"In this chapter, we imagined our Nobel visualization, establishing a minimal set of visual elements necessary to tell the key stories discovered during our explorations of the last chapter"*


### 15. Building a Visualization *[P.371-397]*

Summary : *"In this chapter, we sketched out how to implement the visualization we imagined in Chapter 14. The backbone was assembled from HTML, CSS, and JavaScript building blocks and the data feed to the app and data flow within it described"*


### 16. Introducing D3 - The Story of a Bar Chart *[P.399-438]*




### 17.
### 18.
### 19.
### 20.
### 21.