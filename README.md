## Auto Sammir Rayan Dispatcher
This project is the dispatcher portion of a web scraping automation for Auto Samir Rayan's car website.

## Process map
![process map](https://github.com/nourshoreibah/AutoSamirRayanDispatcher/blob/main/processMap.png)

## Improvements Over Original Process
-	Handles multiple emails at once, reducing processing time and duplicate queue transactions
-	Filters brands before scraping links instead of scraping every brand then filtering, significantly increasing efficiency
-	Goes directly to new cars link (which can be changed in config) instead of relying on website navigation
-	Dispatches one queue item per brand, containing brand name and a comma separated string of all its links, reducing number of queue transactions required
- -  Note: This is safe since commas are not valid characters in link
-	 Tracks which emails were valid and contributed to the hash set, then replies to each of them
-	Note: Some error handling is excluded from process map for simplicity

