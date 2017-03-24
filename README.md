# Project-1--State-Wise-Development-Analysis-In-India1
In scope
This following requirement will be addressed in phase 1 of Project:
 Developing system to handle the incoming log feed and store the information in Hadoop Cluster(Flume)
 Analyze the data and understand the progress
 Store the results in hbase/RDBMS
Step 1:
Copy dataset from local file system to HDFS using flume.

flume-agent agent –n agent1 –c conf –f <path to filecopy.conf>

Solution : filecopy.conf is used for flume import and screen shot of the file is shown in flume_Import_Project2.1_StateWise.png

Step 2: 
Input file is in the XML format use Map reduce or pig to parse the data and get the results for
the below problem statements.
==============================================================================================================================
Problem 1: Find out the districts who achieved 100 percent objective in BPL cards
Solution : Pig script for loading XML file in HDFS is written in 
ProjectProbDist100Pscript_pig.png.
ProjectProbDist100PUDF_java.png
Problem : Export the results to mysql using sqoop. /RDBMS export
Solution :ProjectProbDist100Pmysql_sqoop_output.png
Output in MySQL from sqoop is shown in following screen shot
ProjectProbDist100Pmysql_sqoop_output.png
===================================================================================================================================
Problem 2 : Write a Pig UDF to filter the districts who have reached 80% of objectives of BPL cards.
Solution : PigScript and Java UDF are shown in these screen shot files
ProjectProbDist80Pscript_pig.png
ProjectProbDist80PUDF_java.png
Export the results to mysql using sqoop. /RDBMS export
ProjectProbDist80Pmysql_sqoop_output.png

Output in MySQL from sqoop is shown in following screen shot
ProjectProbDist1Pmysql_sqoop_output.png
