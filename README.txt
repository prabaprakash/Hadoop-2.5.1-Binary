____________________________________________________
Apache Hadoop 2.5.1 Native  Built Version for Ubuntu 14.10
____________________________________________________

Enjoy...................Follow Me..................

Step to Install.:
1. Install JDK 1.7 x64

2. extract the files in /usr/local/hadoop-2.5.1

3.download the config file in https://github.com/prabaprakash/Hadoop-2.5.1-Config-Files

4. $sudo gedit ~/.bashrc   // addd the follwing lines

#HADOOP VARIABLES START
export JAVA_HOME=/usr/java/jdk1.7.0_67 
export HADOOP_INSTALL=/usr/local/hadoop-2.5.1 
export PATH=$PATH:$HADOOP_INSTALL/bin
export PATH=$PATH:$HADOOP_INSTALL/sbin
export HADOOP_MAPRED_HOME=$HADOOP_INSTALL
export HADOOP_COMMON_HOME=$HADOOP_INSTALL
export HADOOP_HDFS_HOME=$HADOOP_INSTALL
export YARN_HOME=$HADOOP_INSTALL
export HADOOP_COMMON_LIB_NATIVE_DIR=$HADOOP_INSTALL/lib/native
export HADOOP_OPTS="-Djava.library.path=$HADOOP_INSTALL/lib"
#HADOOP VARIABLES END
5. source ~/.bashrc

6. hadoop namenode -format
7. enjoy

How I Built ?

follow the steps if you like to built.....

Need Hadoop 2.5.1 Source Files
then
1.Maven 3.3

2.Protocal Buffer 2.5

3.Cmake  - for Native

4.sudo apt-get install zlib1g-dev

5.sudo apt-get install libssl-dev

6.JDK 1.7 64 BIN


final command

mvn package -Pdist,native -DskipTests -Dtar

for native with Documentation


mvn package -Pdist,native,docs -DskipTests -Dtar
