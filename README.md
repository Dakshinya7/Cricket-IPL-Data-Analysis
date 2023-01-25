# Cricket IPL Data Analysis 🏏

The Indian Premier League (IPL), also known as TATA IPL for sponsorship reasons, is a men's T20 franchise cricket league of India. It is annually contested by ten teams based out of seven Indian cities and three Indian states. The league was founded by the Board of Control for Cricket in India (BCCI) in 2007. Brijesh Patel is the incumbent chairman of IPL. It is usually held annually in summer across India between March to May and has an exclusive window in the ICC Future Tours Programme. The IPL is the most-attended cricket league in the world and in 2014 was ranked sixth by average attendance among all sports leagues. In 2010, the IPL became the first sporting event in the world to be broadcast live on YouTube. Over the course of its run starting from its inaugural season in 2008 till the recently concluded one in 2022, there have been various winners with the franchises of Chennai and Mumbai winning the title multiple times. In this project we have taken the IPL data from the years 2008 to 2016 and have applied the concepts of Hadoop and implemented in hive and pig.


## DISCLAIMER ⚠️
This is a POC(Proof of concept) kind-of project. The data used here comes up with no guarantee from the creator. So, don't use it for making sports decisions. If you do so, the creator is not responsible for anything. However, this project is an analysis made based on the data taken and presents the idea that how we can use SQL queries to retrive the required data at large scale and with authentic and verified data.


## AIM 🏹
To find the information of certain players and to find the winner of the IPL editions from 2008 to 2016 on the two given datasets and analyse them using pig and hive in Hadoop.


## DATA SOURCE 📊
Matches dataset (custom built dataset)
Deliveries dataset (custom built dataset)
Two cricket data files with Indian Premier League data from 2008 to 2016 is used as a data source. The files are as follows:
   1.matches.csv – Provides details about each match played
   2.deliveries.csv – Provides details about consolidated deliveries of all the matches
These files are extracted and loaded into Hive. The data is further processed, transformed, and analyzed to get the winner for each season and the top 5 batsmen with maximum run in each season and overall season.


## IMPLEMENTATION 🚀
Implementation is done in both PIG and HIVE.


## APACHE PIG 🐷
Pig represents Big Data as data flows. Pig is a high-level platform or tool which is used to process the large datasets. It provides a high-level of abstraction for processing over the MapReduce. It provides a high-level scripting language, known as Pig Latin which is used to develop the data analysis codes. First, to process the data which is stored in the HDFS, the programmers will write the scripts using the Pig Latin Language. Internally Pig Engine(a component of Apache Pig) converted all these scripts into a specific map and reduce task. But these are not visible to the programmers in order to provide a high-level of abstraction. Pig Latin and Pig Engine are the two main components of the Apache Pig tool. The result of Pig always stored in the HDFS. 


## APACHE HIVE 🐝
Apache Hive is a data warehouse and an ETL tool which provides an SQL-like interface between the user and the Hadoop distributed file system (HDFS) which integrates Hadoop. It is built on top of Hadoop. It is a software project that provides data query and analysis. It facilitates reading, writing and handling wide datasets that stored in distributed storage and queried by Structure Query Language (SQL) syntax. It is not built for Online Transactional Processing (OLTP) workloads. It is frequently used for data warehousing tasks like data encapsulation, Ad-hoc Queries, and analysis of huge datasets. It is designed to enhance scalability, extensibility, performance, fault-tolerance and loose-coupling with its input formats. Initially Hive is developed by Facebook and Amazon, Netflix and It delivers standard SQL functionality for analytics. Traditional SQL queries are written in the MapReduce Java API to execute SQL Application and SQL queries over distributed data. Hive provides portability as most data warehousing applications functions with SQL-based query languages like NoSQL. 


## HOW TO USE 💻
### PRE-REQUISITE 🛍️
· Ubuntu 16.04 or higher version running (install Ubuntu on Oracle VM (Virtual Machine) VirtualBox),
· Run Hadoop on ubuntu (I have installed Hadoop 3.2.1 on Ubuntu 16.04). 

### STEPS TO INSTALL PIG IN HADOOP 🪜
1.  Login into Ubuntu.
2.  Go to https://pig.apache.org/releases.html and copy the path of the latest version of pig that you want to install.
3.  Untar pig-0.16.0.tar.gz file.
4.  Create a pig folder and move pig-0.16.0 to the pig folder.
5.  Now open the .bashrc file to edit the path and variables/settings for pig.
6.  Make the changes effective in the .bashrc file.
7.  Start all Hadoop daemons, navigate to the hadoop-3.2.1/sbin folder.
8.  Launch pig.

### STEPS TO INSTALL HIVE IN HADOOP 🪜
1.  Unzip and Install Hive.
2.  Setting Up Environment Variables.
3.  Setting HIVE_HOME.
4.  Setting Path Variable.
5.  Verify the Paths.
6.  Replacing bins.
7.  Creating File Hive-site.xml.
8.  Editing Configuration Files.
9.  Creating Hive User in MySQL.
10. Creating Metastore.
11. Adding Few More Properties(Metastore related Properties).


## Further Improvements 📈
This was my first big data project so there are lot of things to improve upon.
