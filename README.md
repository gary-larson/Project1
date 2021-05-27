# Sample Hive Project
## Description
This project is mainly for learning and practicing simple HIVE commands in real time scenarios. Here we have taken some sample coffee shop data and processed some essential queries to demonstrate HDFS & HIVE commands.
## Technologies Used
* Ubuntu - 20.4
* Hadoop - 3.3.0
* Hive - 2.3.8
## Features
* Utilized Beeline for the connection from the command line
* Used HiveQL to solve scenarios
## To-Do List
* Future use SBT to write a Scala program
## Getting started - for images see presentation
1. Git Clone: ``` https://github.com/gary-larson/Project1.git ```
1. Open Windows Terminal
1. Open a ubuntu terminal
1. ``` ssh localhost ```
1. edit the hive configuration file
    1. ``` sudo nano apache-hive-2.3.8-bin/conf/hive-site.xml ```
        1. Add the following within the configuration tags
        ``` 
        <property>
        <name>hive.cbo.enable</name>
        <value>true</value>
        </property>
        <property>
        <name>hive.compute.query.using.stats</name>
        <value>true</value>
        </property>
        <property>
        <name>hive.stats.fetch.column.stats</name>
        <value>true</value>
        </property>
        <property>
        <name>hive.stats.fetch.partition.stats</name>
        <value>true</value>
        </property> 
        ```
        1. save and exit
1. Start hadoop File System 
    1. ``` startdfs ``` OR
    1. ``` ~/hadoop/hadoop-3.3.0/sbin/start-dfs.sh ```
1. Start Yarn
    1. ``` startyarn ``` OR
    1. ``` ~/hadoop/hadoop-3.3.0/sbin/start-yarn.sh ```
1. start beeline
    1. ``` beeline -u jdbc:hive2:// ```
## Usage - for usage see presentation
Enter the command from the presentation at the beeline prompt and you will see the results when the command has completed
## Contributors
Gary Larson
## License
This project uses the following license: 
