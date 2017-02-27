Session 4
Assignment 6
(i) If 7TB is the available disk space per node (9 disks with 1 TB, 2 disk for operating system etc. were excluded.). Assuming initial data size is 600 TB. How will you estimate the number of data nodes (n)?
    
•	Available disk Space/node d = 7TB
•	Initial data size H=600 TB
•	The formula to estimate the number of data nodes is, 
•	n=H/d
•	n=600/7
•	n=86
	The number of data nodes are 86.
(ii) Imagine that you are uploading a file of 500MB into HDFS.100MB of data is successfully uploaded into HDFS and another client wants to read the uploaded data while the upload is still in progress. What will happen in such a scenario, will the 100 MB of data that is uploaded will it be displayed?

•	According to this scenario, the file will be spitted into 4 blocks (3 blocks each of size 128 MB and one block of size 116 MB) and gets stored in HDFS. 
•	As only 100 MB of the file is uploaded and it doesn't fulfill a single block, the client can't read the file. 
•	If 128MB of the file is successfully uploaded in HDFS (1 block gets over) the client can read the uploaded content successfully (BASED ON COHERENCY MODEL).
•	So, the client can't read the file unless one block gets completely occupied.
