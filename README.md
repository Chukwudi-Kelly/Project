# Project
lampstack and lempstack
# Project

# Lemp-Stack


# Lemp-Implementation Project

The LEMP stack is a software stack used for web development. It is similar to the more commonly known LAMP stack but replaces Apache with Nginx. LEMP stands for Linux, Nginx (pronounced Engine-X), MySQL, and PHP.

![nginx](./img/1.1%20nginx.PNG)

Launch and EC2 instance
![Lempserver](./img/1.2%20%20launch%20an%20EC2%20instance.png)

 Edit inbound rules to control incoming traffic to the instances 
![inbound rules edit](./img/2.%20edit%20inbound%20rules.png)

Connect to a terminal (Termius) and install nginx
![nginx Installation](./img/4.%20nginx%20installation.png)

Confirm nginx is succesfully installed and running
![Nginx active](./img/5.%20nginx%20active.png)

On the browser url, try the IP address at port 80. If it shows welcome to nginx, it means web server is correctly installed and accessible through the fire walls
![ip on url](./img/7%20nginx%20server%20responding.png)

## Install mysql-server
![sql](./img/8%20sql%20installation.png)

sudo mysql shows the sql version
![version](./img/9%20sql%20version.png)

Run the MySQL secure installation script and validate password
![secure installation](./img/9%20sql%20version.png)

## PHP installation and configuration. 
Install php-fpm and php-mysql. PHP fastCGI process manager tells nginx to pass php requests to this software for processing. php-mysql allows php to communicate with mysql databases
![php](./img/10%20php-fm%20php-mysql%20installation.png)

## Root web directory creation and domain assignment
Creat the root web directory for your domain and assign ownership of the environment with the $USER environment variable. Also paste a try file on projectLEMP file. Activate configuration by linking to the config file from nginx sites-enabled directory.
![Alt](./img/11%20projectLEMP.png)

Check for configuration and syntax error
![Alt](./img/12%20configuration%20and%20syntax%20error%20test.png)

Try to open your url using IP address
![Alt](./img/13%20testing%20projectLEMP.png)

Test PHP  with nginx. create a test file in your document root and open a php file, info.php. Test the page on your web browser
![phpinfo](./img/14%20phpinfo.png)

## Retrieving data from mysql

First connect to the mysql console using the root account and creat a database
![connect to sql](./img/15%20connect%20to%20sql%20console%20and%20creat%20a%20database.png)

creat a new user and grant the user full priviledges on the data that was created
![](./img/15.1%20adding%20data%20to%20sql%20data.png)
![](./img/18.0%20todolist%20cat.png)

Run SHOW DATABASES command to display the database that was created
![database](./img/16%20show%20databse.png)

insert few more roles in the test table
![](./img/17%20database%20created.png)
![](./img/17.1%20updated%20rows.png)
