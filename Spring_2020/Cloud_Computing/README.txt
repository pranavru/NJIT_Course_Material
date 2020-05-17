Configure your terminal session

1) vim ~/.aws/credentials


2) vim ~/.aws/config
[default]
region = us-east-1 

3) aws s3 ls s3://my-programming-assignment/data/csv_files

4) aws emr list-clusters

5) aws emr list-clusters --active

6) Command to run AWS EMR Cluster

	cd Desktop/Files/NJIT/Spring_2020/Cloud\ Computing
	aws emr ssh --cluster-id j-34ZWFT1GIBBT6 --key-pair-file PranavCCASsign.pem
or 
	ssh -i PranavCCASsign.pem hadoop@ec2-35-173-246-109.compute-1.amazonaws.com

7) to check the configuration of EMR, go to the browser and type
	ec2-35-173-246-109.compute-1.amazonaws.com:50070

8) To check memory of nodes 
	df -h

9) To connect to nodes we need to add the private key using ssh
	history | grep ssh-add
	ssh-add -K PranavCCASsign.pem hadoop@ec2-35-173-246-109.compute-1.amazonaws.com
	ssh -A hadoop@ec2-35-173-246-109.compute-1.amazonaws.com 

10) 



