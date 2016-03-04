<h1> Lab3 - Move local csv to hdfs and then import to mysql in hdfs sandbox </h1>

* Step 1 - Make sure you have a tool to move local files to remote - example WinSCP if you are using PC. 
* Step 2 - Pull the data/nasdaq.csv file from the github under bigdata-visa folder. 
https://github.com/vsistla/bigdata-visa/tree/master/data
* Step 3 - using WinSCP on PC or some other tool on PC/Mac, move the local csv file to sandbox as shown in the video. 
* Step 4 - Make hdfs-course directory under your user directory.
* Step 5 - Move the uploaded csv file to the hdfs-course directory
* Step 6 - sandbox comes with mysql installed. import the csv file to mysql table
* Step 7 - run with few of following queries
	* use database
	* SELECT
	* SELECT with LIMIT(10)
	* describe
* STEP 8 - Import the nasdaq table from mysql into sqoop using jdbc:mysql driver
	* Import all the rows
	* Then ....try to import with a criteria to smaller set




