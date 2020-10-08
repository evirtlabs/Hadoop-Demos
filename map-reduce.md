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

## Total output is given below
02098693387_0002 completed successfully
2020-10-08T06:20:50,833 INFO [main] org.apache.hadoop.mapreduce.Job - Counters: 54
        File System Counters
                FILE: Number of bytes read=131
                FILE: Number of bytes written=529457
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=376
                HDFS: Number of bytes written=85
                HDFS: Number of read operations=9
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=2
                HDFS: Number of bytes read erasure-coded=0
        Job Counters
                Launched map tasks=1
                Launched reduce tasks=1
                Data-local map tasks=1
                Total time spent by all maps in occupied slots (ms)=2958
                Total time spent by all reduces in occupied slots (ms)=4378
                Total time spent by all map tasks (ms)=2958
                Total time spent by all reduce tasks (ms)=4378
                Total vcore-milliseconds taken by all map tasks=2958
                Total vcore-milliseconds taken by all reduce tasks=4378
                Total megabyte-milliseconds taken by all map tasks=3028992
                Total megabyte-milliseconds taken by all reduce tasks=4483072
        Map-Reduce Framework
                Map input records=5
                Map output records=5
                Map output bytes=115
                Map output materialized bytes=131
                Input split bytes=135
                Combine input records=0
                Combine output records=0
                Reduce input groups=1
                Reduce shuffle bytes=131
                Reduce input records=5
                Reduce output records=5
                Spilled Records=10
                Shuffled Maps =1
                Failed Shuffles=0
                Merged Map outputs=1
                GC time elapsed (ms)=146
                CPU time spent (ms)=1590
                Physical memory (bytes) snapshot=487202816
                Virtual memory (bytes) snapshot=6057779200
                Total committed heap usage (bytes)=384303104
                Peak Map Physical memory (bytes)=286560256
                Peak Map Virtual memory (bytes)=3024887808
                Peak Reduce Physical memory (bytes)=200642560
                Peak Reduce Virtual memory (bytes)=3032891392
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=241
        File Output Format Counters
                Bytes Written=85
(base) [hdeveloper@hadoop mapreduce]$
