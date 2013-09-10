hadoop-example-jobs
===================

A bunch of hadoop jobs, examples

- Also, we will keep the libraries in here synchronized with what is expected 
- add runners for mapred jobs that synch deps to the DC where necessary. 
- add examples of running pig/hive tasks programmatically
- add sample mahout jobs for iterative clustering which is very common
- add sample custom output formats to dump outputs into useable sinks (solr/riak/hbase) 

To play in this framework, there are only a few simple steps: 

0) git clone <this project>

1) mvn eclipse:eclipse 

2) Write a mapreduce job and place it in the src/main/java directory 

3) Write a test for it in the corresponding tests/ director 

4) mvn clean package 

5) scp the target/*jar folder into the head node on your cluster 

6) run this command "hadoop jar hadoop-examples-1.0-SNAPSHOT.jar org.rhbd.others.MultiFileWordCount /a_folder_in_my_dfs /output7"

And of course, replace "org.rhbd.others.MultiFileWordCount" with the fully qualified jar name. 


