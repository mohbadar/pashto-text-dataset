# Dataset for Pashto Language

Applying machine learning (ML) techniques, especially, deep learning heavily depends on data.  It is most crucial aspect that makes training algorithm possible. It describes why machine learning is becoming so popular in these years. ML algorithms try to identify and extract patterns from the existing data. So, more data means more patterns for identification and extraction. 

Regardless of how much data you have, if ML algorithms cannot make sense of it; the data is useless and perhaps even harmful.  The issue is that every dataset has flaws. That is why data preparation is such a significant step in the machine learning process. 

We have developed a framework to prepare dataset for summarization and other NLP tasks. The preparation is set of procedures and guidelines that help to make more suitable datasets. This framework consist of data collection and data cleaning.


## Data Collection

Data gathering is the process of collecting data from sources. It is the most challenging and effort consumer process in dataset building. Inaccurate data collection could lead my research to invalid result and effect result of study. In order to collect more data with less resources I have written multiple scripts to read articles from sources and add them to the central repository of articles. The scripts are written by Python and have the flexibility of reading data from any website add to repository. The central repository of documents consists of 35000 of documents.

1.	Script sends a request for a specific URL web content.
2.	Web server receives the request and send a request to data source.
3.	Data source get the specific document and send it back to web server.
4.	Web server sends the document data gathering.
5.	The script stores the document to the central repository of documents.

<img src="/asset/data-collection.PNG" />

## Data Cleaning 

Data Cleaning is the process of detecting and correcting of any inaccurate, corrupted, duplicated, null or empty records from dataset. In my case, as soon as I got the dataset I start the cleaning process. The process consist of following:
•	Rename columns name to appropriate names
•	Detect all inaccurate, corrupted, duplicated, null and empty records
•	Remove the improper records

<img src="/asset/data-cleaning.PNG" />

To clean the data I have written a script to apply our data cleaning procedure. 

1.	The script sends a request for the dataset.
2.	It receives the dataset from the central repository of documents.
3.	Rename column names in dataset.
4.	Detect inaccurate, corrupted, duplicated, null, and empty records of documents.
5.	Remove the incorrect records.
6.	 Store back to central repository of documents.
