Executing same command on multiple ec2 instances simultaneously using Mobaxterm
- This tutorial was done on a Windows 11 Machine

![](./images/execute-command-multiple-instances.png)

This is what we shall be doing
1. Downloading and installing Mobaxterm on out local computer
2. Launch 4 ec2 ubuntu servers in AWS
3. SSH into the 4 servers using Mobaxterm
4. Running a single curl command to return the public ipv4 address of each instance

### 1. Download latest stable version of Mobaxterm and install it.

Download Mobaxterm from official [Mobaxterm website](https://mobaxterm.mobatek.net/download-home-edition.html)


### 2. Launch 4 Ubuntu Servers and label them A, B, C and D

Choose 4 Ubuntu Instances on the free tier - Ubuntu Server 22.04 

![Choose Instance1](./images/launch1.png)

For Instance Type, select t2.micro which is on the free tier to avoid costs

Choose an existing keypair or create one.
I created one called testkeypair.pem

![Choose Instance1](./images/launch2.png)

For the firewall settings, allow SSH traffic as we shall need to SSH into our instances to get the public IP addresses later.

![Choose Instance1](./images/launch3.png)


Leave other settings as default and click on Launch Instance

![Choose Instance1](./images/launch4.png)

Rename each Instance as ServerA,ServerB,ServerC, and ServerD

![Choose Instance1](./images/launch5.png)





