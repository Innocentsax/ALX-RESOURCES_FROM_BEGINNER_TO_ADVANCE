# Materials for Month 6

Sprint 3 starts in Month 6 and it is the most hands on part of the Foundations training. For many it will be uncharted territory as there will be lots to learn and execute as quickly as possible. Lots of Linux-based tasks, software installation and configuration. Hopefully these materials will be useful to you and will help you get up to speed very quickly. This is not meant to be a replacement for the materials already provided on the intranet, but to augument them and possibly cover areas that need more attention and clarity.

I would like some feedback if you have any. Send me an email at onchemoses38@gmail.com

### Table of Contents
1. [Node.js](#JavaScript)
2. [SSH](#SSH)
3. [Load balancer](#Load-Balancer)
4. [HTTPS/SSL(Domain Zone Config)](#Configure-Your-Domain-Zone)
5. [HTTPS/SSL(Certbot and HAProxy Config)](#HAproxy-SSL-termination)
6. [MySQL Replica](#MySQL-Replica)

## JavaScript
[Back to the top](#Table-of-Contents)

What is Node.js? Unlike other general purpose programming languages, Javascript was first developed as a special purpose language for web browsers. So it only ran in web browsers for a while. Node.js was then developed to be a runtime environment for Javascript which allows you to write and run Javascript outside a browser like other mainstream languages. Node.js provides the platform for Javascript to be used as a backend language to build server applications and even write command-line scripts. It comes preinstalled in some of the sandboxes that we are given, and also on Linux if you are using WSL or Virtual Box.
More [here.](https://www.educative.io/blog/what-is-nodejs)


## SSH
[Back to the top](#Table-of-Contents)

What is SSH? SSH is a short form for Secure Shell, just as 'bash' is short for Bourne Again Shell. A shell is terminal-based program that allows you to give direct instructions as well as run precoded instructions written in a script. Simply put, it conveys your instructions to the kernel. More on that [here.](https://www.geeksforgeeks.org/what-is-terminal-console-shell-and-kernel/)

ssh enables you to securly execute commands and programs in a computer that is physically out of your reach. Your webserver is most likely in another country on another continent. SSH helps you connect to its terminal so you can run scripts, deploy programs and so on. Most of what you need to know about ssh is provided in the material of the task. There was however an issue where ssh keys were missing from sandbox terminals. [Follow this guide if you ever run into such an issue.](https://www.baeldung.com/linux/copy-ssh-keys)


## Load Balancer
[Back to the top](#Table-of-Contents)

### How to configure web-02 to be like web-01:
1. Use 4-not_found_page_404 script from task 4 in [this project.](https://intranet.alxswe.com/projects/266)
2. In your terminal, go into the appropriate repo using cd. The filepath should be alx-system_engineering-devops/0x0C-web_server
3. Copy it using scp command as follows:
```
scp 4-not_found_page_404 ubuntu@your_web-02_server_ip:~
```
Note that 'your_web-02_server_ip' is just a placeholder name. Use your correct web-02 server IP.
4. Now ssh into web-02 and run the script. If done correctly, web-02 nginx will now be configured just like web-01.
5. Exit by typing 'exit' or pressing Ctrl + D. Now cd back into the task folder '0x0F-load_balancer'. Don't forget to create a readme file.

After you do this, you write another script to configure a custom header in nginx in both web-01 and web-02
1. Create the 0-custom_http_response_header script in the task folder '0x0F-load_balancer'.
2. Use scp to copy this script to both web-01 and web-02 servers
```
scp 0-custom_http_response_header ubuntu@your_web-01_server_ip:~
```
```
scp 0-custom_http_response_header ubuntu@your_web-02_server_ip:~
```
3. ssh into web-01, run the script. Exit back to your terminal.
4. ssh into web-02, run the script. Exit back to your terminal.
5. Test your configuration using the example shown in the task.

### How to install HAProxy:
1. Write a script to install and configure HAProxy with the specs given in the task. Follow the task material for guidelines.
2. Using what you have learnt above use scp to copy the script '1-install_load_balancer' to your load balancer
```
scp 1-install_load_balancer ubuntu@your_lb-01_server_ip:~
```
3. ssh into your load balancer and run the script.
4. Exit the ssh and test using the example shown in the task.
5. Always take note of the terminal prompt in the examples. Some tests are run on the server itself, others are run from your terminal.

## Configure Your Domain Zone
[Back to the top](#Table-of-Contents)

Configuring your domain zone to point your subdomain to your load balancer is easy.
You should have your domain name by now.
1. Got to get.tech
2. Login to your account

![login page](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/2ae345bc-71b6-41bb-83c9-ccdb624a6f96)

3. When logged in, at the top right hand corner, click on account.

![acount](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/5ebfa10d-450b-44a3-95ef-bb88a22e543d)

4. The account management page will appear. In the 'Jump to Domain' window, type your domain name and click on the '>>' button.

![jump to domain](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/ca42ac75-b097-4893-8293-0b8c0d949aa1)

5. A new page will appear. Scroll to the bottom of the page or click on 'DNS Management' on the side menu. Then click on 'Manage DNS'

![manage dns](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/adb78a7a-24af-4829-bd45-8994a56f98a0)

6. A new window will open. This is your domain zone. All you are required to do here is to create A records according to how they are specified in the tasks. Click on 'Add A record'.

![domain zone](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/295c32a9-e758-40b8-ba10-29e0148adabc)

7. An A record page will appear. In 'Host Name', type 'www'. In 'Destination IPv4 address' type your lb-01 IP address. Click 'Add record'.

![a record page](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/16bc22af-5d97-4427-998f-4c034d4248cb)

8. Repeat this for all the other subdomains speficied in the task and fill in the appropriate server IP addresses.
9. Now write a bash script to display domain information in the terminal with all the requirements specified in the task.
NB: These guidelines are written according to the time they were executed. Page design and instructions are subject to changes from get.tech, or if ALX decides to use another domain name provider.


## HAproxy SSL termination
[Back to the top](#Table-of-Contents)

These are the steps that I followed in solving the task. Please note that it is subject to correction.
Step 1: ssh into lb-01.

Step 2: Stop HAProxy process
```
sudo service haproxy stop
```
Step 3: Install Certbot
[Click here to open](https://certbot.eff.org/instructions?ws=haproxy&os=ubuntufocal) Certbot's official page for instructions on how to install it to work with HAProxy. Follow it step by step. When you get to step 7, switch over to [this article](https://www.linuxtechi.com/how-to-setup-haproxy-ssl-termination-ubuntu/).
In this article they installed it with apache. But we are installing with HAProxy, so scroll down to the part after the apache service is stopped.
```
sudo certbot certonly --standalone --preferred-challenges http --http-01-port 80 -d root_domain -d sub_domain
```
Replace root_domain with your own root domain.

Replace sub_domain with your own subdomain.

In the article, the answers to the prompts that show on the terminal are addressed in the screenshots. Follow them.

Step 4: Configure HAProxy to use your SSL certificate.
Continue with the article in Step 3. Edit the commands and fill in the appropriate details. For example:
```
DOMAIN='linuxtechgeek.info'
```
Replace 'linuxtechgeek.info' with your own root domain before executing the command.

The rest of the article is fairly straight forward. Just follow step by step. If you open your domain in a browser tab and it shows the padlock icon next to it, then it means your configuration was done properly.

Step 5:
Finally, type
```
sudo vi /etc/haproxy/haproxy.cfg
```
Highlight and copy its content. Close your ssh connection to go back to your normal terminal. Create a file 1-haproxy_ssl_termination and paste what you copied here.
Save and commit it to Github. Note that this configuration also covers redirecting HTTP traffic to HTTPS in the next task. Just include a line for HAProxy to return a 301. Copy out the configuration as you did above and commit to GitHub.

## MySQL Replica
[Back to the top](#Table-of-Contents)

This task involves creating a mirror version of your MySQL database in web-02 so that if anything happens to web-01, web-02 can serve to keep everything running while web-01 is troubleshooted and fixed. The replica updates all the changes made in the web-01 db. Here are tips on how to approach the tasks.

### How to install MySQL 5.7.x

This task is long and somewhat daunting. Be very meticulous when doing it.

The task requirement is to install MySQL 5.7.x (x is just a placeholder for any number. 5.7 is the focus). Here is an excellent guideline that takes you through the process of installing MySQL 5.7, especially if you have 8.0 already installed -> [Link](https://www.devart.com/dbforge/mysql/how-to-install-mysql-on-ubuntu/). Remember to install 5.7 in both web-01 and web-02.

* How to create a new user and grant them permission: [Link to article](https://www.digitalocean.com/community/tutorials/how-to-create-a-new-user-and-grant-permissions-in-mysql)
* How to set up replica infrastructure: [Link to article](https://www.digitalocean.com/community/tutorials/how-to-set-up-replication-in-mysql). PLease note that newer versions of MySQL use Source-Replica relationship description, while older versions use Master-Slave description. This Digital Ocean article above uses Source-Replica in the configuration. For example:
```
CHANGE REPLICATION SOURCE TO
SOURCE_HOST='source_server_ip',
SOURCE_USER='replica_user',
SOURCE_PASSWORD='password',
SOURCE_LOG_FILE='mysql-bin.000001',
SOURCE_LOG_POS=899;
```
But the task requirement is to use MySQL 5.7.x.

So when you get to the above part, revert back to MySQL's official documentation for 5.7: -> [Here](https://dev.mysql.com/doc/refman/5.7/en/replication-setup-replicas.html).
