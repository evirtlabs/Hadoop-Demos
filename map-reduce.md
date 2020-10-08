# Hadoop Map Reduce Sample

## Create a directory by name input in hdfs file system
### hdfs dfs -mkdir -p  input

## Put data on which we need to apply map reduce in this input directory
###  hdfs dfs -put /hadoop/etc/hadoop/*.xml input

## Run the map reduce program 
### hadoop jar /hadoop/share/hadoop/mapreduce/hadoop-mapreduce-examples-3.3.0.jar grep input output 'dfs[a-z.]+'

