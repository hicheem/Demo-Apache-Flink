# FLINK EXAMPLES
## First setup
- 1 - Download the flink, the lib folder's files can be added as external JAR to eclipse project in order to compile the file and make a jar file from java.
- 2 - go to bin folder and type : ./start-cluster.sh to start locally.
## WordCount (batch)
go to bin folder and type : ./flink run "name of the jar file".jar --input "inputfile.txt"

## WordCount using socket
- 1 - open the socket : nc -l 3003
- 2 - go to bin folder and type : ./flink run "name of the jar file".jar
- 3 - To see the result go to the log file and search for the file that has the name " flink-root-taskexecutor-0-localhost.localdomain.out"
- 4 - once the file found type : tail -f "file name on the log folder" to see the results in real time.
- 5 - you can start send text on the socket