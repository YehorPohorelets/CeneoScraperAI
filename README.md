# CeneoScraperAI

## Single opinion structure

|Element|Selector|Variable|Data type|
|-------|--------|--------|---------|
|Opinion|div.js_product-review|opinion|bs4.element.Tag|
|Opinion id|\["data-entry-id"\]|opinion_id|str|
|Author|span.user-post__author-name|author|str|
|Recommendation|span.user-post__author-recomendation > em|rcmd|bool|
|Stars score|span.user-post__score-count|score|float|
|Content|div.user-post__text|content|str|
<<<<<<< HEAD
|List of adventages|div.review__title--positives  ~ div.review-feature__item|pros|str|
|List of disadventages|div.review__title--negatives  ~ div.review-feature__item|cons|str|
=======
|List of adventages|div.review__title--positives  ~ div.review-feature__item|pros|list\[str\]|
|List of disadventages|div.review__title--negatives  ~ div.review-feature__item|cons|list\[str\]|
>>>>>>> 959847afd3dfa024a76aed41ca9802b338febbf7
|Date of posting opinion|span.user-post__published > time:nth-child(1)\["datetime"\]|posted_on|str|
|Date of purchasing product|span.user-post__published > time:nth-child(2)\["datetime"\]|bought_on|str|
|For how many users useful|button.vote-yes > span|useful_for|int|
|For how many users useless|button.vote-no > span|useless_for|int|

  ## Stages of project

   1) Extraction of elements for a single opinion to separate variables
   2) Extraction of elements for a single opinion to one complex variable (dictionary)
<<<<<<< HEAD
   3) Extraction of all opinions form single page to list of dictionaries
   4) Extraction of all opinions for certain product and saving it to a .json file
   5) Code refactoring and optimization
      1) Definition of function for extracting single element of page from HTML code
      2) Creation of dictionary that describes opinions' structure with selectors for particular opinion's elements
      3) Using dictionary comprehension to extraact all opinion's elements on the basis of opinion's structure dictionary
   6) Adjustment of data types for different opinion's elements
   7) Translation of certain opinion's elements into English
   8) Analysis of extracted opinions
      1)Basic statistics
         1) Number of all opinions about the product 
         2) Number of opinions with list of advantages 
         3) Number of opinions with list of disadvantages
         4) Average score based on stars
      2) Plots
         1) Share of recommendations in total number of opinions
         2) Frequency histogram  of stars
=======
   3) Extraction of all opinions form single page to list
   4) Extraction of all opinions for certain product and saving it to a file
   5) Code refactoring and optimization
      a) Definition of function for extracting single element of page from HTML code
      b) Creation of dictionary that describes opinions' structure with selectors for particular opinion's elements
      c) Using dictionary comprehension to extraact all opinion's elements on the basis of opinion's structure dictionary
   6) Adjustment of data types for different opinion's elements
   7) Translation of certain opinion's elements into English
>>>>>>> 959847afd3dfa024a76aed41ca9802b338febbf7
