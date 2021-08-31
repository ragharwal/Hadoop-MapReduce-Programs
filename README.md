### How to run Hadoop MapReduce Programs in Eclipse ?
1. Star and Clone the repository 
2. Export the folder `foldername` as a JAR File
3. Select the export destination `/home/cloudera/foldername.jar`
4. Open the terminal in directory `/home/cloudera`
5. Run the following commands (Step-By-Step):
  ```
cat > /home/cloudera/inputfile.txt
hdfs dfs -put /home/cloudera/inputfile.txt /inputFolder
hdfs dfs -cat /inputFolder/inputfile.txt
hadoop jar /home/cloudera/foldername.jar ClassName /inputFolder/inputfile.txt /output
hdfs dfs -ls /output
hdfs dfs -cat /output/part-r-00000

  ```
