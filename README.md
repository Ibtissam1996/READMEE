-Installation of Zibbix Server on centos7
 Installation of the web server
 Installation of php
 Installation of the mariadb server
 Zabbix DB creation
 Installation of the Zabbix mysql DB
 Import Zabbix sql file to our database
 Configuration of Zabbix Server conf file
 Configuration of Zabbix agent conf file
 Allow firewall port 10051 / tcp, 10050 / tcp
 Selinux must be deactivated


-Installation of Zabbix Agent on centos 7 and macOs
* On mac:
 Download zibbix agent from this link https://www.zabbix.com/download_agents
 Start the installation wizard
 Configure this composents (Host name, Zabbix server IP/DNS, Agent listen port, Server or proxy for active checks) inside file /usr/local/sbin/zabbix_agentd
* On Centos:
 Add the required libraries
 Install Zabbix Agent 
 Configure Zabbix Agent 
 Open Port 
 Restarting the Zabbix agent


-Add client machines to Zabbix
* Log in to your Zabbix web interface using the administrator account. Follow then the steps below:
 Click on the configuration menu
 Click on the Hosts submenu
 Click on the Create host button on the right
* Now fill in the following information on the remote host, then go to the Templates tab.
 Host name: Enter the host name of the remote system.
 Visible name: Name to display in zabbix
 Group: Select the desired group for your host
 Agent interface: fill in the information about the Zabbix agent running on
the host
 Activated: Check if active
* Select the desired model: you must select carefully, because it will allow all checks for the host.
 Click on add
 Click on the Add button
  
  
 * Screen Shots:
 ![Screen Shot 2020-05-22 at 14 10 01](https://user-images.githubusercontent.com/62620555/83209557-948dd480-a150-11ea-9b37-ee96b1474f2a.png)
![Screen Shot 2020-05-26 at 18 20 07](https://user-images.githubusercontent.com/62620555/83209565-96f02e80-a150-11ea-8824-170ba2891833.png)
![Screen Shot 2020-05-26 at 19 29 29](https://user-images.githubusercontent.com/62620555/83209567-98215b80-a150-11ea-9eef-3fa74aef3c4d.png)
![Screen Shot 2020-05-26 at 19 41 54](https://user-images.githubusercontent.com/62620555/83209570-99528880-a150-11ea-993c-45d94345e26a.png)
![Screen Shot 2020-05-26 at 19 51 20](https://user-images.githubusercontent.com/62620555/83209574-9a83b580-a150-11ea-9cdc-3abe3fc2b761.png)
![Screen Shot 2020-05-26 at 20 21 22](https://user-images.githubusercontent.com/62620555/83209579-9bb4e280-a150-11ea-8b1d-25760fe6a7d6.png)
![Screen Shot 2020-05-26 at 20 22 36](https://user-images.githubusercontent.com/62620555/83209582-9ce60f80-a150-11ea-9faf-c50eaa9f1b74.png)
![Screen Shot 2020-05-26 at 20 31 00](https://user-images.githubusercontent.com/62620555/83209584-9eafd300-a150-11ea-8ef3-8a7a62abac64.png)
![Screen Shot 2020-05-26 at 20 36 24](https://user-images.githubusercontent.com/62620555/83209586-a0799680-a150-11ea-8ac7-dd706606884b.png)
![Screen Shot 2020-05-26 at 20 36 29](https://user-images.githubusercontent.com/62620555/83209589-a1aac380-a150-11ea-9fa6-8c897abfd851.png)
![Screen Shot 2020-05-26 at 20 36 54](https://user-images.githubusercontent.com/62620555/83209594-a40d1d80-a150-11ea-826a-2f928a4fc23b.png)
![Screen Shot 2020-05-26 at 20 37 23](https://user-images.githubusercontent.com/62620555/83209597-a53e4a80-a150-11ea-8a67-1a7d999045d2.png)
![Screen Shot 2020-05-26 at 20 40 23](https://user-images.githubusercontent.com/62620555/83209600-a7080e00-a150-11ea-893c-cde3878c3d8c.png)
![Screen Shot 2020-05-26 at 20 44 07](https://user-images.githubusercontent.com/62620555/83209619-b0917600-a150-11ea-9abe-f2a4b3c8b164.png)
![Screen Shot 2020-05-26 at 20 46 53](https://user-images.githubusercontent.com/62620555/83209624-b25b3980-a150-11ea-8d7a-8c21eaf6fca5.png)
![Screen Shot 2020-05-26 at 20 52 56](https://user-images.githubusercontent.com/62620555/83209627-b2f3d000-a150-11ea-93f2-55ff21ad2b5f.png)
![Screen Shot 2020-05-26 at 21 59 38](https://user-images.githubusercontent.com/62620555/83209630-b4bd9380-a150-11ea-8b46-464fb8087344.jpeg)
![Screen Shot 2020-05-26 at 22 24 19](https://user-images.githubusercontent.com/62620555/83209635-b5eec080-a150-11ea-85d8-56e93c917586.png)
![Screen Shot 2020-05-27 at 01 25 14](https://user-images.githubusercontent.com/62620555/83209646-b8e9b100-a150-11ea-916e-94f2336b30b4.png)
![Screen Shot 2020-05-27 at 01 25 20](https://user-images.githubusercontent.com/62620555/83209648-ba1ade00-a150-11ea-8e24-bd670409e161.png)
![Screen Shot 2020-05-27 at 01 43 26](https://user-images.githubusercontent.com/62620555/83209651-bb4c0b00-a150-11ea-9f89-9df75e082a91.png)
![Screen Shot 2020-05-27 at 01 43 58](https://user-images.githubusercontent.com/62620555/83209653-bbe4a180-a150-11ea-9ad1-7e892fc0171c.png)
![Screen Shot 2020-05-27 at 01 45 31](https://user-images.githubusercontent.com/62620555/83209656-bd15ce80-a150-11ea-89da-6995ee466048.png)
![Screen Shot 2020-05-27 at 01 57 17](https://user-images.githubusercontent.com/62620555/83209661-bf782880-a150-11ea-9c4f-6e06863f3c23.png)
![Screen Shot 2020-05-27 at 01 57 41](https://user-images.githubusercontent.com/62620555/83209663-c141ec00-a150-11ea-80c4-8d7ff8caea45.png)
![Screen Shot 2020-05-28 at 15 39 06](https://user-images.githubusercontent.com/62620555/83209666-c30baf80-a150-11ea-862d-1bb379c2b2da.jpeg)
![Screen Shot 2020-05-28 at 15 43 11](https://user-images.githubusercontent.com/62620555/83209669-c43cdc80-a150-11ea-9abd-c853ff4d20c0.jpeg)
![Screen Shot 2020-05-28 at 15 44 25](https://user-images.githubusercontent.com/62620555/83209672-c606a000-a150-11ea-94ba-3367a576370f.jpeg)
![Screen Shot 2020-05-28 at 16 17 11](https://user-images.githubusercontent.com/62620555/83209674-c868fa00-a150-11ea-9fca-cccee822c004.jpeg)
![Screen Shot 2020-05-28 at 16 31 47](https://user-images.githubusercontent.com/62620555/83209677-c9019080-a150-11ea-8dc6-6a1560f6f701.jpeg)
![Screen Shot 2020-05-28 at 16 46 52](https://user-images.githubusercontent.com/62620555/83209679-ca32bd80-a150-11ea-88c7-2063b1b50413.jpg)
