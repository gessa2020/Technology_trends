# Technology Trends Analysis
## A project to analyze technology trends using data obtained from an API, Web Scraping and Survey data
![](IMAGES/toptrendsjpg.jpg)
## Introduction
To stay ahead in today's fast-paced technological landscape, organizations must constantly analyze data to identify current and future skill requirements. This project aims to conduct a comprehensive technology trend analysis by collecting data from various sources and cleaning it up for analysis. By doing so, we hope to provide valuable insights that will help organizations remain competitive and adapt to changing technologies.

##  Problem statement 
1. __What are the skill requirements for future?__
2. __What are the top programming languages in demand?__
3. __What are the top database skills in demand?__
 
 
## Skills demonstrated.
- I used python and its associated libraries for web scrapping and data retrival from an api
- I used jupyter notebooks and vscode as IDEs for the project
- I used IBM Cognos dashboard tool for survey data visualization.

## Data sourcing
We scrape data of the **name of the programming language** and **average annual salary** from the <a href="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DA0321EN-SkillsNetwork/labs/datasets/Programming_Languages.html">URL</a>  provided by skills network labs. 
We then write the scraped data into an csv file

We then use the <a href="https://developer.adzuna.com/">Adzuna API</a> to scrape data of number of technology jobs in some selected US cities and store them in an excel file 

We also use the Stack Overflow Developer Survey 2019 data to create a dashboard with IBM Cognos visualization tool to visualize and present our analysis<br>
Note:This randomised subset contains around 1/10th of the original data set.<br> Our Conclusions drawn after analyzing this subset may not reflect the real world scenario<br>
To access this dataset from IBM cloud <a href="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DA0321EN-SkillsNetwork/LargeData/m1_survey_data.csv">Click_HERE</a>

## Data transformation and cleaning.
1.  The survey dataset goes through various cleaning processes before being visualized in the IBM Cognos tool.
2.  Data from both the Api and scraped web page also undergoes cleaning and reformating before being visualized.

## Data analysis and visualization
Graph showing number of jobs generated by each technology![](IMAGES/tech_jobs.png)
### key take ways from the graph above
- Java technology had the most number of job opportunities among all the languages
- The next three languages that followed according to job opportunities created were GO, SQL and Python

Graph showing salaries for different technologies![](IMAGES/salary_langauge.png)
### Key observations from the graph above
- The swift language had the highest annual salary followed by Python, C++, Javascript, Java and then Go
- Apart from Java creating the most job opportunities, it does not top the table of the highest annual salaries but it takes the 5th position

Graph showing different number of jobs by each technology across various selected cities![](IMAGES/job_lists.jpg)

Graph showing Top 10 databases  currently in use![](IMAGES/Top10DatabasesCurrent.jpg)

Graph showing Top 10 databases  Desired Next![](IMAGES/Top10DatabasesNext.jpg)
### key take aways from the graphs above
- MySQL most popular
- Microsoft SQL comes next in popularity after Mysql
- MongoDB and Redis are upcoming favorites
- New kid on the block: Elasticsearch
- Open source databases are still preferable in companies
- NoSQL databases are must have databasese for storing non relational data
- Redis supports abstract data types
- Postgre databases is most likely to become very popular than MySQL in coming years

# Sample Cognos dashboards
Dashboard showing current technology usage![](IMAGES/TAB1.jpg)

Dashboard showing future technology usage![](IMAGES/TAB2.jpg)

To access all the dashboards on IBM cloud <a href="https://dataplatform.cloud.ibm.com/dashboards/ae87c5b9-0315-45aa-a793-45ab09ef70e0/view/7013a12a34f1179e73fcb1e407cc2a062866215ab6bb800bd3807b495c657797a86b1493c8794d53df440c65f1e8125998">Click_HERE</a>

## Conclussion
- With AI and ML in rising demand, Python is the language to look out for because of it’s vast libraries and ecosystem.
- Open source databases are here to stay with us for all forms of tabular data
- NoSQL databases are the standard for unstructured data
- Big Data technology in companies still requires SQL





