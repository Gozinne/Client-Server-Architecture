# IMPLEMENTATION OF A CLIENT SERVER ARCHITECTURE USING MYSQL DATABASE MANAGEMENT SYSTEM (DBMS). 
</a>

![Contributors](https://img.shields.io/github/contributors/Gozinne/Client-Server-Architecture?style=plastic)
![Forks](https://img.shields.io/github/forks/Gozinne/Client-Server-Architecture)
![Stars](https://img.shields.io/github/stars/Gozinne/Client-Server-Architecture)
![Licence](https://img.shields.io/github/license/Gozinne/Client-Server-Architecture)
![Issues](https://img.shields.io/github/issues/Gozinne/Client-Server-Architecture)

## Client-Server Architeure using MySQL Overview

There is a documentation of all you need to know about [Client-Server Architecture](https://github.com/Gozinne/Client-Server-Architecture)somewhere in this repository. In this section, we will concentrate on creating one using the MySQL Database Management System (DBMS).

<img
  src="https://user-images.githubusercontent.com/80969889/208237050-1925c4a0-326a-4fd9-a755-b26d74fcd820.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***
In the preceding example, a system attempting to visit a Web site using a Web browser or simply the "curl" command is a client, and it makes HTTP requests to a Web server (Apache, Nginx, IIS, or any other) via the Internet.

If we expand this notion and include a database server in our design, we obtain the following picture:

<img
  src="https://user-images.githubusercontent.com/80969889/208237112-97e4f304-a2d2-43f1-b288-366ebe73327c.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 300px; border: solid 2px red;">
***
In this example, our Web Server acts as a "client," connecting to and reading and writing to and from a Database (DB) Server (MySQL, MongoDB, Oracle, SQL Server, or any other), with communication taking place via a Local Network (it can also be an Internet connection, but it is a common practise to place the Web Server and DB Server close to each other in a local network). The setup displayed in the image above is a typical generic Web Stack architecture that you have already used in previous projects (LAMP, [LEMP](https://github.com/Gozinne/WEB-STACK-IMPLEMENTATION-LEMP-.github.io), [MEAN](https://github.com/Gozinne/WEB-STACK-IMPLEMENTATION-MEAN-.github.io), [MERN](https://github.com/Gozinne/WEB-STACK-IMPLEMENTATION-MERN-.github.io)). From simple single-page applications (SPAs) to large and complex portals, this architecture may be used with a range of other technologies, including different Web and DB servers.

<img
  src="https://user-images.githubusercontent.com/80969889/208236207-acab406c-018b-4298-9e69-ee274eb974f5.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***
An actual LAMP website example: This Github account has a [LAMP](https://github.com/Gozinne/WEB-STACK-IMPLEMENTATION-LAMP-) stack website implementation. Consider the following professionally deployed LAMP website: www.google.com. This LAMP website server(s) can be hosted anywhere in the world, and you can connect to them over the global network, the Internet. Assume you go to your browser and enter www.google.com. It denotes that your browser is the ", ient." It is essentially sending queries to the remote server and expecting a response from the distant server. Let's take a brief look at client-server communication in action. Launch the curl command in your Ubuntu or Windows terminal.
```
curl -Iv www.google.com
```
**Note**: If your Ubuntu does not have "curl," run to install it.
```
sudo apt install curl
```
In this example, your terminal is the client, and www.google.com is the server. 
The result below shows the answer from the remote server. 

<img
  src="https://user-images.githubusercontent.com/80969889/208237672-c0a63140-a0bd-4cd8-a537-3595e51cf55f.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 400px; border: solid 2px red;">
***
You can also see that the URL requests are being delivered by a machine with an IP address of 216.58.223.228 and a port number of 80. 
When it comes to networking tasks, we'll go through IP addresses and ports in further detail. 
Another easy method is to use a simple diagnostic tool like "ping," which will also report round-trip time—the time it takes for packets to go to and from the server. The ICMP protocol is used by this utility.

## Implementing a basic Client-Server using MySQL Relational Database Management System (RDBMS)

### Requirements
The following items are required to begin and complete this project.

* An account logged into the AWS console.
* Launch 2 AWS EC2 instance, name one as the `MySQL-Server` and the other as `MySOL-Client`
* Run the EC2 instance on Ubuntu 20.4, set the network security to: SSH,Port:22; HTTP,Port:80; MySQL, Port 3306, and an ICMP protocol.
* Connect VScode or MobaXterm to the EC2 instance and launch a new terminal.

<img
  src="https://user-images.githubusercontent.com/80969889/208238504-4bb761c7-bf55-4b9f-9a36-273a08e28a92.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 400px; border: solid 2px red;">
***
<img
  src="https://user-images.githubusercontent.com/80969889/208238773-18d045e6-5b96-44f7-93bf-1e8ace1ef72c.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 400px; border: solid 2px red;">
***
### Demonstration of the Implementation

On mysql server Linux Server install MySQL Server software.

// ssh into the mysql server instance

<img
  src="https://user-images.githubusercontent.com/80969889/208239688-3d88c18a-36d3-4a3a-b2ae-0c284fc16188.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 400px; border: solid 2px red;">
***

<img
  src="https://user-images.githubusercontent.com/80969889/208239627-6c800734-bf18-4bcb-bf76-bda4fe350149.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 400px; border: solid 2px red;">
***

<img
  src="https://user-images.githubusercontent.com/80969889/208239891-0ea16260-dfc1-48e0-b342-e3c1f3595bcb.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***

// On mysql server Linux Server install MySQL Server software
```
sudo apt update
```
// Then install the mysql-server package
```
sudo apt install mysql-server
```
// Ensure that the server is running using the systemctl command:
```
sudo systemctl start mysql.service
```
```
sudo systemctl status mysql.service
```

<img
  src="https://user-images.githubusercontent.com/80969889/208239971-60cc353a-a655-4ca8-bc33-48f3b55fdf52.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***

// Let's get started
```
sudo mysql
```
// To define the user's password as PassWord.1, enter
```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';
```
Then exit the MySQL shell with: `exit`

// Start the interactive script by running
```
sudo mysql_secure_installation
```
A prompt will appear to configure the VALIDATE PASSWORD PLUGIN.
It is safe to leave validation disabled.
Therefore click on any key apart from `Y` to continue without enabling.

Regardless of whether the VALIDATE PASSWORD PLUGIN was activated, the server will prompt you to select and confirm a password for the MySQL root user. 
`PassWord.1` should be used. 

For the rest of the questions, press `Y` and hit the `ENTER` key at each prompt.

<img
  src="https://user-images.githubusercontent.com/80969889/208240425-5cf727c1-91c4-4f26-9dc7-7ad1683793a5.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***


// Test the MySQL console by typing:
```
sudo mysql -p
```
Exit the MySQL console by typing `exit`.

```
sudo mysql
```
// Create a new database by running the following command from MySQL console
```
mysql> CREATE DATABASE `example_database`;
```
// The user's password is thus defined as password, although it may be updated with a safe password of choosing
```
mysql> CREATE USER 'example_user'@'%' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';
```
// Give this user permission over the example_database database
```
mysql> GRANT ALL ON example_database.* TO 'example_user'@'%';
```

<img
  src="https://user-images.githubusercontent.com/80969889/208240594-f2b20c72-ca89-4749-a2a3-ab729e4267b7.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***

// Exit the MySQL shell by typing **exit**, and then test by
```
mysql -u example_user -p
```

<img
  src="https://user-images.githubusercontent.com/80969889/208240649-981bf6b1-2e96-456b-a5a5-ef4eb5cd1f5a.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 500px; border: solid 2px red;">
***




























