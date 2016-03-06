<h1> Lab - Apache Pig Demo in Hdfs sandbox </h1>

* Step 1 - HDFS sandbox comes with pig latin shell installed. Launch pig grunt shell
* Step 2 - Type help to see all the commands available for you. Try out few of the HDFS commands you have already learned in the past labs. 
https://github.com/vsistla/bigdata-visa/tree/master/data
* Step 3 - Set up data for the pig demo. For that you need load data from HDFS. 
	* move apple daily stock and nasdaq daily csv into tmp directory. You might already have apple csv. 
	* get the nasdaq data file from github data folder. 
	* Launch pig grunt shell
	* using LOAD and PigStorage commands, load Appl daily csv file
	* Follow instructions in the video "Demo: Querying Data with Pig" video to follow rest of the instructions. 
	* DUMP to see the output variable. 
	* Similarly folow instructions for loading nasdaq data
	* 
* Step 4 -  write JOIN in Pig Latin. We are going to join them based on the date and high value in both the data set. 
	* use FOREACH to load date and high in a new variable for appl
	* Do the same for nasdaq
	* Use JOIN command to join both the data sets. 
	* DUMP to see the combined variable data. 

	
* Step 5 -  Store results in HDFS
	* Use STORE function to store the combined data INTO your user a/c. Use PigStorage for this action
	* once stored, quit out of Pig grunt shell
* Step 6 - Run ls to see if the newly created directory exits
* Step 7 - Open the newly created directory and run cat on the PART* file to see the data
Congratulations - you have managed to merge two data sets in Pig and merged them based on certain criteria.
