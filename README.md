# Search Engine using DFS
The **Search Engine** is a Java-based Desktop web application with basic search engine functions.
The web application has the following primary features:
  # 1. Search:
      For a searched query, the most relevant webpages will be displayed in a ranked manner. The top 30 most relevant results will be displayed by default.
      The search results would be obtained from a given SQL database to which a connection should be established first. The Java-based WebCrawler is made use of to obtain webpages from the _Worlwide Web_ using Depth Limited Search, a variation of Depth First Search (DFS). These webpages would be stored in the database and can be accessed for seach queries.
  # 2.  Search History:
      The search queries will be stored in the database and can be obtained using the **history** feature whenever required. There is also the option to clear all search history from the database.
