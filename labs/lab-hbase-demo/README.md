<h1> Lab - HBase demo hdfs sandbox - csv data to HBase </h1>

* Step 1 - Launch HBase Shell and try few of the commands
	* help to get list of commands
	* Enable Ambari as described in the video "Demo HBase Basic Shell Command". Launch Ambari dashboard
	* Start HBase in Amabari. Now, go back to Command line
	* Try following commands - list, get and put in quering
	* Try scan, disable and drop commands
	* Create a row for user and enter some data
	* Now, update that row data using the same put command
	* Disable and drop that user and run scan to see what you get

* Step 2 - Now lets insert Appl csv values into HBase. You will use pig to write a pig script from hdfs to Hbase. 
	* in your sandbox, locate your app stock values csv file. 
	* launch hbase shell
		* create apple stock table with column name info
		* scan to see if its there. 
		* exit out of Hbase
	* Create pig script (use any text editor like vim or nano or etc)
		* using editor open hbase_pigloader.pig
		* LOAD appl daily stock values using PigStorage
		* STORE the variable where you stored the data into hbase app_stock table. For this, you using HBaseStorage package. This is one of the packages offered in Pig. 
		* Once your script is complete, run your script. 
			* using pig -f script.pig
		* See the output to see if you wrote records and its written into app_stock table. 
	* verify by launch HBase shell
		* scan with LIMIT to 10 ot if you can see the data in HBase
Congratulations. That's your first lab in HBase. 

