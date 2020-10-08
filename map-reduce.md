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
02098693387_0002 completed successfully <br/>
2020-10-08T06:20:50,833 INFO [main] org.apache.hadoop.mapreduce.Job - Counters: 54 <br/>
        File System Counters <br/>
                FILE: Number of bytes read=131 <br/>
                FILE: Number of bytes written=529457  <br/>
                FILE: Number of read operations=0  <br/>
                FILE: Number of large read operations=0  <br/>
                FILE: Number of write operations=0  <br/>
                HDFS: Number of bytes read=376  <br/>
                HDFS: Number of bytes written=85  <br/>
                HDFS: Number of read operations=9  <br/>
                HDFS: Number of large read operations=0  <br/>
                HDFS: Number of write operations=2  <br/>
                HDFS: Number of bytes read erasure-coded=0  <br/>
        Job Counters  <br/>
                Launched map tasks=1  <br/>
                Launched reduce tasks=1  <br/>
                Data-local map tasks=1  <br/>
                Total time spent by all maps in occupied slots (ms)=2958  <br/>
                Total time spent by all reduces in occupied slots (ms)=4378  <br/>
                Total time spent by all map tasks (ms)=2958  <br/>
                Total time spent by all reduce tasks (ms)=4378  <br/>
                Total vcore-milliseconds taken by all map tasks=2958  <br/>
                Total vcore-milliseconds taken by all reduce tasks=4378  <br/>
                Total megabyte-milliseconds taken by all map tasks=3028992  <br/>
                Total megabyte-milliseconds taken by all reduce tasks=4483072  <br/>
        Map-Reduce Framework  <br/>
                Map input records=5  <br/>
                Map output records=5  <br/>
                Map output bytes=115  <br/>
                Map output materialized bytes=131  <br/>
                Input split bytes=135  <br/>
                Combine input records=0  <br/>
                Combine output records=0  <br/>
                Reduce input groups=1  <br/>
                Reduce shuffle bytes=131  <br/>
                Reduce input records=5  <br/>
                Reduce output records=5  <br/>
                Spilled Records=10  <br/>
                Shuffled Maps =1  <br/>
                Failed Shuffles=0  <br/>
                Merged Map outputs=1  <br/>
                GC time elapsed (ms)=146  <br/>
                CPU time spent (ms)=1590  <br/>
                Physical memory (bytes) snapshot=487202816  <br/>
                Virtual memory (bytes) snapshot=6057779200  <br/>
                Total committed heap usage (bytes)=384303104  <br/>
                Peak Map Physical memory (bytes)=286560256  <br/>
                Peak Map Virtual memory (bytes)=3024887808  <br/>
                Peak Reduce Physical memory (bytes)=200642560  <br/>
                Peak Reduce Virtual memory (bytes)=3032891392  <br/>
        Shuffle Errors  <br/>
                BAD_ID=0  <br/>
                CONNECTION=0  <br/>
                IO_ERROR=0  <br/>
                WRONG_LENGTH=0  <br/>
                WRONG_MAP=0  <br/>
                WRONG_REDUCE=0  <br/>
        File Input Format Counters  <br/>
                Bytes Read=241  <br/>
        File Output Format Counters  <br/>
                Bytes Written=85  <br/>
(base) [hdeveloper@hadoop mapreduce]$
