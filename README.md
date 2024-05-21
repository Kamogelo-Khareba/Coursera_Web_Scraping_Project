# Coursera_Web_Scraping_Project

## Errors I encountered and how I dealt/ran away from them
-> connectionerror: ('connection aborted.', connectionreseterror(10054, 'an existing connection was forcibly closed by the remote host', none, 10054, none))
Given that this is my first webscraping project, I kept on adding new functions and with new functions, I need to re-run the code, that's is whe this error poped up.
It takes approximately 3 hours to be able to reconnect with the website once more. I could not handle that so I ran to "RAPIDAPI.COM", where I found a free LinkedIn API, to which I can connect to and access the data.

-> The LinkedIn_jobs function only scrapes the job card data and not the job descriptions. What you can find joy in is, that the job cards contain a url that leads to the job descriptions. So you have to web scrape those links too, in order to get the job descriptions. My ideal case was running a *for loop* to scape the urls and convert each response to a dictionary using ".json()", I could not achieve that. So I used BeautifulSoup to convert the responses.
