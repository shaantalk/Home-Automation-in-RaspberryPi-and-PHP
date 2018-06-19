# Home Automation in RaspberryPi and PHP

One of the advantages of the Raspberry Pi is the ease at which it can be connected to network and by extension the internet. Here’s how we have accessed the GPIO pins of Raspberry Pi using simple PHP scripts and Web Browser of choice. 

Step 1: At first we needed to setup a web server. We setup a typical LAMP (Linux, Apache, MySQL, and PHP/Perl) server in our system.Using first the sudo (Super User Do) modifier we use apt-get install/remove to install and uninstall various packages. First we install apache2 which will be our web server that responds to requests from web browsers connecting over port 80. apt-get will ask if we wish to download the resources necessary to install the requested package, we typed Y on the keyboard indicating Yes. 

Code:  pi@raspberrypi ~ $ sudo apt-get install apache2 

Step 2: Next we should install a database server, do so by running the command below. You will be asked to enter a MySQL root password, this can be the same as your current password or something different if you want to be more secure about it. 

Code: pi@raspberrypi ~ $ sudo apt-get install mysql-server 

Step 3: Now, We write the PHP code within a file named index.php that must be placed within the folder as such: 
/var/www/html 
And then we need to edit the index.php by running this code in terminal 
Code: sudoleafpadindex.php
This code opens a graphical editor named leafpad for writing the php code within it. We could have used nanoeditor but it is not a graphical editor so it is difficult to edit a webpage here. 

Step 4: The code for the PHP page is given here in the repository
