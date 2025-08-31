## Prerequisites
- JDK 1.8 or later
- Maven 3 or later
- MySQL 5.6 or later

## Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
## Database
Here,we used Mysql DB 
MSQL DB Installation Steps for Linux ubuntu 14.04:
- $ sudo apt-get update
- $ sudo apt-get install mysql-server

Then look for the file :
- /src/main/resources/accountsdb
- accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < accountsdb.sql


kops create cluster --name=kubepro.menradevops.xyz --state=s3://kubpro-mwr --zones=us-east-1a,us-east-1b --node-count=2 --node-size=t3.small --control-plane-size=c7i-flex.large --dns-zone=kubepro.menradevops.xyz --node-volume-size=12 --control-plane-volume-size=12 --ssh-public-key ~/.ssh/id_rsa.pub

kops update cluster --name=kubepro.menradevops.xyz --state=s3://kubpro-mwr --yes --admin