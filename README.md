last use: march of 2023

# Welcome to my first scrape. Despite being simple, it worked like a charm. 

https://www.reclameaqui.com.br/ 

ReclamAaqui is a brazilian website that is highly used by either Organizations and consumers to measure they're client satisfaction rate by reporting complaints. 

What I've found so far: 
- the website has an anti-scraper. Use it wisely
- the page limit is 500
- there are 10 complaints per page
- maximum extraction by now is: last 5000 (five thousand) complaints of the selected organization


Written in Python

The main idea is to have to parts.
Part A:
When select an Organization, go to complaints, you can see the a list with 10 last complaints. 
Save all these complaints infos. Such as: url, title, description, date and tag (with the anwser status).
Then I'll save all theses 10 complaints infos in a .csv or a .xslx file and then loop through the next page and on and on. 
It will create a dataset with the main complain topic, if it has been anwsered or not, how long ago it has been made, the status and it's url.

Part B:
Iterate over all URL gathered in part A to get every detail from the complain such as the location, tags, date, answers, and so on.

So, by the end, it'll create to datasets, one is the raw info and their url. The second one is the full info gathered. 



