# MHN---Modern-Honey-Network

MHN is a centralised server for honeypot management and data collection. It enables users to quickly deploy honeypot sensors or scripts to collect attack data points. The gathered data or statistics can be viewed via an MHN dashboard or web interface. Several standard honeypot scripts, such as Snort, Cowrie, Dionaea, and glastopf, as well as a few others, are available under the “Deploy script” option.
MHN incorporates a collection of sensors to collect data on network attacks. MHN analyses the attack and its parameters, which are displayed on a World Map, while retaining a wealth of information about the attack.

Installation of MHN Server on AWS EC2 Instance are as follows:
1. Select Ubuntu 16.04 ec2 instance (Instance Type: t2.small)
2. sudo apt-get update && sudo apt-get upgrade
3. sudo apt-get install git –y
4. sudo git clone https://github.com/threatstream/mhn.git
5. cd mhn
6. sudo ./install.sh
7. Deploy script of honeypot sensor and keep tcp port 10000 open for sensors to communicate intrusion data with MHN server.

MHN inbound rules
![InkedMHN inbound rule 1_LI](https://user-images.githubusercontent.com/73482919/114271727-8aa35600-9a30-11eb-9a86-456be8fc25a5.jpg)



MHN Installation
![MHN Installation Selected Choices](https://user-images.githubusercontent.com/73482919/114271592-ca1d7280-9a2f-11eb-8d78-2011131cd071.png)

To ensure that everything is in order, run these three commands, and the output should be "Running."
1. sudo /etc/init.d/nginx status
2. sudo /etc/init.d/supervisor status
3. sudo supervisorctl status


Deploy Script i.e. honeypot sensors using the Deploy option from dashboard
![Deploy Script 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271944-8fb4d500-9a31-11eb-8400-09c308e5013d.png)


MHN Dasboard

![Attack Stats 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271775-c8a07a00-9a30-11eb-9a35-c806ced007bc.png)

![DionaeaConnections and ConpotEvents 2020-06-08](https://user-images.githubusercontent.com/73482919/114271803-e968cf80-9a30-11eb-9972-5ca3781803b4.png)

![MHN MAP 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271824-000f2680-9a31-11eb-9bd0-11948b38b041.png)

![Sorts alerts (Payload Reports) 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271843-174e1400-9a31-11eb-852c-50e980e3e124.png)

![Top Attackers 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271828-06050780-9a31-11eb-82cf-77f4efd64ab3.png)

![Top passwords 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271833-0a312500-9a31-11eb-8f4e-da4e95328923.png)

![Top User-Password 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271837-0dc4ac00-9a31-11eb-92a3-5018e2cab52a.png)

![Top Users 2020-06-08 ](https://user-images.githubusercontent.com/73482919/114271838-10bf9c80-9a31-11eb-95a7-2d3362d80cac.png)
