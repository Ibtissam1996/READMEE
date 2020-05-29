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
