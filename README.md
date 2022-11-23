# Amazon Scraper

An application that returns an amazon.com top search result through a discord bot.

<img width="631" alt="Screen Shot 2022-11-23 at 2 22 18 AM" src="https://user-images.githubusercontent.com/69515228/203491338-679093f1-6787-4108-a42f-337fa257d105.png">

## Usage

Try it out: https://discord.gg/hsBSpKdjuf

Enter in textbox: !amazon 'search-query'


## How

The following application pareses amazon.com's code base using the BeautifulSoup python package to parse the HTML.

The HTML code of a search query is turned into a parse tree and navigated for information about the product through identifying HTML tags and classes used to encompass the desired data.

Through this, product title, price, image, ratings, number of ratings, and link to the product are collected.

Through discord.py packages, an asynchronous function returns product information that is displayed in a discord channel upon the event a user types !amazon 'search-query'.
  
Error cases are handled for invalid searches, where 'An error occurred with your request.' is returned
  
Application is deployed on Heroku for 24/7 application responsivity.

## Future Plans
  
The plan is to expand this project into returning products from other websites such as Target, Walmart, and more.

## Note

Code in this repository does exclude the bot token and channel code for safety reasons (as seen in config.py). A duplicate repository, that is private, contains the bot token and channel id, and is the actual repository that is being hosted.
