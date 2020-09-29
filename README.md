# WeRateDogs Wrangling
## by Moahmed A. Desouky

## Introduction

[**Data wrangling**](https://en.wikipedia.org/wiki/Data_wrangling) or sometimes referred to as data munging, is the process of transforming and mapping data from one "raw" data form into another format with the intent of making it more appropriate and valuable for a variety of downstream purposes such as analytics.

**Note:** In this project there will be two notebooks, this one [**Wrangle WeRateDogs**](#top) that contains the `data wrangling` process and [**Analyze and Visualize WeRateDogs**](01_analyze_visualize.ipynb) that contains the visualization process.

In the **first notebook**, I will start with **Data Wrangling** techniques, e.g. `Gather`, `Assess` and `Clean` the dataset. 

While, in the **second notebook**, I will use Python visualization libraries to systematically `explore` a selected dataset, starting from plots of single variables and building up to plots of multiple variables, then `communicate` the interesting properties, trends, and relationships that I discovered through aesthetic and polished visuals.

**Note:** I have included a slideshow (`2_slideshow.slides.html`) as a presentation that displays the explantory visualizations and the summary of my findings, also I have included the review (`Udacity Review.pdf`) from Udacity on my project and I have already take the reviewer's suggestions and notes into consideration.

## Dataset

**The dataset** we will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs). WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10 (`11/10`, `12/10`, `13/10`, etc).

This **dataset** has 3 tables:
- **enhanced_archive** with `2356` records and `17` variables.
- **image_predictions** with `2075` records and `12` variables.
- **retweet_favorite_counts** with `2331` records and `3` variables.

## Summary of Findings
1. The order of dog stages average rate are **Puppo**, **Floofer**, **Doggo** and **Pupper** respectively.
2. The most favorite dog stages in WeRateDogs tweets are **Puppo**, **Doggo**, **Floofer** and **Pupper** respectively.
3. We have a good neural network with almost **0.73%** accuracy in predicting dog breeds.
4. **Golden Retriever**, **Labrador Retriever** and **Chihuahua** are our top 3 frequent breeds.


## Key Insights for Presentation
- There were some missing values in variable `name` in tweet archive data, and after checking the original retweets I found that those dogs have no name from the beginning, thus, I couldn't do anything and I decided to replace the string `None` values with `Null` values for all the records in this table.
- Also, I found that the 4 dog stages (**Doggo**, **Floofer**, **Pupper** and **Puppo**) are separated in `4 variables`, but they are one variable `stage`.

## Resources
The resources I have used in this project:
- [**Data wrangling**](https://en.wikipedia.org/wiki/Data_wrangling)
- [**@dog_rates**](https://twitter.com/dog_rates)
- [**WeRateDogs**](https://en.wikipedia.org/wiki/WeRateDogs)
- [**Gathering data**](https://ori.hhs.gov/education/products/n_illinois_u/datamanagement/dctopic.html)
- [**web scraping**](https://en.wikipedia.org/wiki/Web_scraping)
- [**requesting URLs**](https://requests.readthedocs.io/en/master/)
- [**APIs**](https://www.mulesoft.com/resources/api/what-is-an-api)
- [**Pandas API**](https://pandas.pydata.org/docs/reference/index.html)
- [**Cleaning Data**](https://en.wikipedia.org/wiki/Data_cleansing)
- [**SQLAlchemy**](https://www.sqlalchemy.org/)
