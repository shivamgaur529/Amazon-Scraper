# Amazon-Scraper
This is a product details scraper.

The following code is written according to the selenium version 3.141.0
And can be changed according to newer or older versions.

# Approach:
  1. To scrape all the details. I first made a loop to loop through every url. To check the availability of url, I checked if it had a product title or not.
  2. If the product was not available or the url threw the 404 error, I printed "{url} not available".
  3. I also checked if there is an accept cookies button and clicked it as it was interfering with details.
  4. I made 4 functions to scrape all 4 different details.
  5. I added every details to the corresponding list out of all the four lists namely titles, image_urls, prices, details.
  6. To scrape all those four details, I made four different functions.
  7. After the details were scraped and appended to the respective lists, I made a dictionary with all the four lists.
  8. Then I converted the dictionary to json file.
  
# Approach for the 4 functions:
  1. get_titles function scraped the titles of the products
  2. get_image_urls function scraped the urls of the products
  3. get_details first checked if there was a see more option to display more details and scraped the details.
  4. get_price function has multiple try and except clauses as there were total 4-5 different ways as to where price was stored in the pages.
  5. It shows no specified price for the ones which have no price.
  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shivamgaur529/Amazon-Scraper/blob/main/ans.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shivamgaur529/Amazon-Scraper/blob/main/BonusTaskCaptcha.ipynb)
