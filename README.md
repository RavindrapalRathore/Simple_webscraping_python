# Simple_webscraping_python
This is a Python script that uses BeautifulSoup to scrape book data from a website and store it in a list called "books". 

Here's how it works:

- The script starts by creating an empty list called "books".
- It then uses a for loop to iterate through pages 1-50 of the website. For each page, it creates a URL that includes the page number and sends a request to that URL using the requests library.
- Once it receives a response, it extracts the content of the page and passes it to BeautifulSoup to parse it as HTML.
- It then finds the "ol" tag on the page, which contains all the book articles, and extracts all the articles using the "find_all" method.
- For each book article, it extracts the book's title, star rating, and price, and adds them to the "books" list as a new sublist.
- Finally, the script returns the "books" list, which contains the book data for all 50 pages of the website.
