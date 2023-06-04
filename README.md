# Apache Flink Demo

## Setup

1. Download the flink, the lib folder's files can be added as external JAR to eclipse project in order to compile the file and make a jar file from java.

2. go to bin folder and type : 
```shell
./start-cluster.sh to start locally.
```

### WordCount (batch processing)

1. go to bin folder and type : 
```shell
./flink run "name of the jar file".jar --input "inputfile.txt"
```

### WordCount using socket (real time stream processing)

1. open the socket in the window terminal : 
```shell
nc -l 3003
```

2. go to bin folder and type in a new windows terminal: 
```shell
./flink run "name of the jar file".jar
```

3. To see the result go to the log file and search for the file that has the name :
    ```flink-root-taskexecutor-0-localhost.localdomain.out```

4. once the file found type the following to see the results in real time.
```shell
tail -f "file name on the log folder"
``` 

5. you can start send text on the socket


---

**© 2023 Written by Hichem FARAOUN. All rights reserved.**