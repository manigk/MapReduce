# Mapreduce java program
#### First Load the code from eclipse
### Step 1:
Create jar file 
### Step 2:
#### Load txt file into HDFS
#### Create Directory
mkdir BigData
### Step 4:
#### Move file from Local to HDFS
Go to Local terminal
Give Permission
sudo -s
#### Move text file from local to HDFS
hdfs dfs -put root/bigdata/wordcountfile1.txt /user/BigData
### Step 6:
#### Run jar file
(hadoop jar jarfilename.jar packageName.ClassName  PathToInputTextFile PathToOutputDirectry)

hadoop jar bigdata/MapR.jar com.mapReduce.MapWordCount /user/BigData/wordcountfile1.txt /user/BigData/out
### Step 7:
#### View the Out file Folder
hadoop fs -ls /user/BigData/out1
### Step 8:
#### View the Output file
hadoop fs -cat /user/BigData/out1/part-r-00000
## End..
