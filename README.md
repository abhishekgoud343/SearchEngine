# Search Engine using DFS
The **Search Engine** is a Java-based Desktop web application with basic search engine functions.
The web application has the following primary features:
  # 1. Search:
  For a searched query, the most relevant webpages will be displayed in a ranked manner. The top 30 most relevant results will be displayed by default.
  The search results would be obtained from a given SQL database to which a connection should be established first.
  The Java-based WebCrawler is made use of to obtain webpages from the _Worlwide Web_ using Depth Limited Search, a variation of Depth First Search (DFS). These webpages would be stored in the database and can be accessed for seach queries.
  # 2.  Search History:
  The search queries will be stored in the database and can be obtained using the **history** feature whenever required.
  There is also the option to clear all search history from the database.

## Instructions to run the Project locally
### Web Scarping to your MySQL database using _WEB CRAWLER_
1. Create a MySQL database and an appropriate table to store the _page title_, _page link_, and _page text_ obtained from web pages through web scraping.  
2.  Open the ```Web Crawler``` project folder in any IDE or code editor such as IntelliJ IDEA, VS Code, Eclipse etc.  
3. Install the ```jsoup``` library from Maven repository in the IDE.  
4. Download the ```MySQL Connector``` archive file from [here](https://dev.mysql.com/downloads/connector/j/) and extract it. Install  the ```mysql-connector``` library as a java library in the IDE; select the jar file from the extracted folder as source for the library.
5. Make appropriate changes to the code in the java files ```DataBaseConnection.java``` and ```Indexer.java``` as per the instructions in the comments int the respective files; add the respective username, password, database name, table name etc from your MySQL database to establish a connection to your MySQL database.  
6. Open the java file at the location ```WebCrawler\src\main\java\org\accio\Crawler.java```. In the main function of this java program, add the required URLs so that web data can be scraped from the respective webpages, in this manner: ```crawler.getTextsAndLinks("url", 1);``` (replace ```url``` with the desired URL). For example: ```crawler.getTextsAndLinks("https://javatpoint.com", 1);```. A deeper web scraping can be performed by icreasing the ```MAX_DEPTH``` parameter in the ```Crawler.java``` program file (initially set to ```2```.)  
7.  The java file at ```WebCrawler\src\main\java\org\accio\Crawler.java``` contains the _main_ function and therefore the project can be thus run by running the aforementioned java file.
8.  On succesfully urunning the ```Web Crawler``` project, the required webpage data will be scraped from the given webpages and added to your MySQL database.

### Running the _Search Engine_ project
1. Open the ```SearchEngine``` project folder in your IDE or code editor.
2. 
