# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk:

Single-Node Configuration

1.	Create a dedicated user account for hadoop

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/ab25ccda-7ba2-41e8-b36a-0f560bbc08e3)

2.	Install java1.8 in folder /usr/local

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/5c6b51c1-911d-4a07-8cdb-43ab41a3897b)

3.	Install Hadoop

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/da575d7a-81a6-4809-8ac0-cb0e8b0c5103)

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/75b4af39-82a3-4468-97ee-131d624b6b94)

 
5.	Set hadoop environment variables: Include the following lines /etc/profile file

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/462f3759-63e4-4155-a025-72e213aa2b34)


6.	Run the.bashrc & profile files from the $ prompt for updating the changes

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/9322a872-5504-42ba-9bed-15a040c2a2cb)

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/1cff69b7-8b2a-4116-a680-66eed6ca0bf2)


$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/4fa9e2f7-6ae0-466a-9928-c7f87a584f48)


b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/bc8cc3db-b1fe-4471-9a91-d840b682d8f1)


 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/5c8a3479-89b3-403c-ba78-cffb647fbec3)


c)	mapred-site.xml

 ![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/31610b15-c30e-430c-8319-cb2f273285b0)


Include the following lines in mapred-site.xml file
 
 ![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/cc3222d3-816a-43f0-855e-68dc52203161)


d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/b07c1ac9-9654-4f45-aebc-b3c5bd3e10a5)


e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/0517fb1a-75ab-4729-805d-ea9b00ab89fc)

8.	Format the Hadoop File system implemented on top of the local file system using

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/98b871f4-f5d4-4d65-aed5-06c431128039)

9.	Start Hadoop using

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/3440e85f-50f5-4556-8bc8-13936362d3f8)


Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/ca16dd10-64b1-425c-b549-067fc8b3aa02)


11.	Create a directory ‘/input’ in HDFS

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/696f49ef-6d18-4e15-a5b6-762569389545)


12.	Copy the input files into the distributed file system

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/a64a5c97-f267-4348-888a-da404d3ded1c)

13.	Run some of the examples provided

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/d13f02e0-2ec1-498a-b0b2-1ea10ebe9199)


14.	Examine the output files

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/c421def4-63fb-4cd3-8c9a-f6e7ac42c5d5)


Copy the output files from the distributed file system to the local file system and examine them:

 ![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/426ada55-14f2-4c59-84f9-1bd2bd766246)

or
View the output files on the distributed file system

![image](https://github.com/priyarajmohan777/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119475942/458fb46f-6d18-4406-94fb-80e431419064)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
