# Amazon Scraper

An application that returns an amazon.com top search result through a discord bot.

<img width="631" alt="Screen Shot 2022-11-23 at 2 22 18 AM" src="https://user-images.githubusercontent.com/69515228/203491338-679093f1-6787-4108-a42f-337fa257d105.png">

Try it out: https://discord.gg/gsQP7UXZ6E

## How

The following application pareses amazon.com's code base using the BeautifulSoup python package to parse the HTML.

The HTML code of a search query is turned into a parse tree and navigated for information about the product through identifying HTML tags and classes used to encompass the desired data.

Returns top search result from amazon search
