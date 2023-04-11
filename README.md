# Simple Web Crawling⚙️
This code is a simple web scraper that fetches the contents of a Wikipedia page on web crawlers and prints the page's title, the number of links on the page, and all external links found on the page.

The code first sends a GET request to the specified URL using the requests library and checks if the response code is 200, which indicates that the request was successful. If the request was successful, the code uses the BeautifulSoup library to parse the HTML content of the page and extract the page's title.

Next, the code uses find_all() method to find all the a tags on the page which represent links. It then prints the total number of links found on the page. The code then loops through all the links and checks if each link has an href attribute and if it is an external link. If both conditions are met, the link is printed.

If the request was not successful, the code prints an error message indicating the status code returned by the server.
