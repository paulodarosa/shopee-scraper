# Shopee Scraper
A web scraper in python that extract sales, price, avaliable stock, location and more of a given seller in Brazil.

The project was created in python 3 and requires only 3 libraries that may need be installed (in case you don't have any of them).

They are: requests, date and time. Date and Time are default libraries for Linux and Mac users, but if you're running Windows, make sure to install them using pip.

You can easily install requests using the following command:
$ pip install requests

The script runs based on Shopee's public API. Shopee generates a dynamic page that shows products and its information calling a json file. Since it's an API and public, it's easier to just call the json file and extract the data instead of selecing divs, classes and scrolling through the results and using Selenium to simulate a web browser.

# How to use it
1. The first thing you have to do is to find the seller's id. It's present in the product link.

Exemple:
https://shopee.com.br/Camisetas-Bandas-Rock-RHCP-Red-Hot-Chili-Peppers-100-Algodao!!-i.409068735.3983196792
- 409068735 is the seller's id. That's required to run the script.
- 3983196792 is the product's id

2. Before running the code, change the file directory where you want to save the csv file generated what will contain all the data extracted.
- file=open("/YOUR-DIRECTORY/%s-YOUR-FILE-NAME.csv" % data, "a"))
- The %s- right before the file name prints the date when the csv was generated. It's recommended to keep it that way, in order to track down your files.

3. Using the terminal, go to the script's folder and run:
- python3 shopee-scraper.py
- Type in the seller's id you just got from the product link.
- The script will scrape every single product published and the scraper will take 1 sec. per ad. So it may take some time depending on the number of products.

# Why I created this project and who I am?
- I'm a Computer Engineering and Mathematics major in Brazil. I already got a bachelors degree in Marketing and I'm looking for a Data Engineer and Data Scientist position. 
- Currently working for a small company in Brazil as a comercial manager and my main role is to increse the online sales of hydraulic and brass connectors for gas and petroleum
- I love data and statistics. Finding new possibilities and ways of doing things better and faster through the data is a facinating thing, and quoting Carl Sagan I would say that "it's a pleasure to share a planet and an epoch with you", because the humankind don't even know yet what we're capable of. AI and machine learning will show us a new world, a new age.
- I really like the feeling of helping companies to make better data-driven decisions on online sales, marketing and purchasing. Solving problems is pretty much the main motivation of any mathematician or engineer
