# Hadoop Map Reduce Sample

Step: 1Create a directory by name input in hdfs file system
### hdfs dfs -mkdir -p  input

Step 2: Put data on which we need to apply map reduce in this input directory
###  hdfs dfs -put /hadoop/etc/hadoop/*.xml input

Step 3: Verify map reduce program jar in respective directory

![Alt text](/images/Screenshot_1.png?raw=true "Simple Code on IPython Notebooks")

Step 4: Run the map reduce program 
### hadoop jar /hadoop/share/hadoop/mapreduce/hadoop-mapreduce-examples-3.3.0.jar grep input output 'dfs[a-z.]+'

![Alt text](/images/Screenshot_2.png?raw=true "Simple Code on IPython Notebooks")
