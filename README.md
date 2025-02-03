# Assessable_Activity2_WAD_2024_25
To create and configure the EC2 instance I first started the lab in aws Academy learner.
I selected EC2 and clicked on launch instance I called the instance my-ubuntu-server, selected the Ubuntu image version 24.04 LTS 64bits arm, the instance type is t4g.micro, the key pair vockey, and for the security group I previously edited the existing one that had the ssh rules on port 22 and added the http rule that listens on port 80.
I configured the elastic ip, by clicking on assign elastic ip address, left it selected as default and hit assign, then in the elastic ip address panel I hit associate elastic ip address and selected the instance I had created earlier.
Once the instance was up and running and the ip address assigned I connected to it using ssh with the command:
ssh -i labsuser.pem ubuntu@52-86-211-190
Once inside I installed node.js, pm2 and npm.
I cloned the project repository and once inside I did the npm install to make sure I have all the dependencies.
I installed apache and configured it as Proxy, activated the modules and configured the virtualHost, saved the comabios, restarted apache and tested its operation by accessing the elastic ip.
