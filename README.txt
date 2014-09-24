____________________________________________________
Apache Hadoop 2.5.1 Native  Built for Ubuntu 14.10
____________________________________________________

Enjoy....................................................


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
