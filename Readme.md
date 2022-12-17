# UNDERSTANDING CLIENT SERVER ARCHITECTURE
</a>

![Contributors](https://img.shields.io/github/contributors/Gozinne/Client-Server-Architecture?style=plastic)
![Forks](https://img.shields.io/github/forks/Gozinne/Client-Server-Architecture)
![Stars](https://img.shields.io/github/stars/Gozinne/Client-Server-Architecture)
![Licence](https://img.shields.io/github/license/Gozinne/Client-Server-Architecture)
![Issues](https://img.shields.io/github/issues/Gozinne/Client-Server-Architecture)

## Client-Server Overview

As we continue on our DevOps journey, we will come across and employ principles that are not just relevant to us but to others in their varied areas. 
One such example is the client-server architecture. 
More people than ever before use and rely on computers and the networks to which they are connected for a variety of functions, putting a significant demand on servers and networks. 
As if these difficulties weren't enough, DevOps Engineer must also cope with a steady trickle of new technologies that must be integrated into the network. 
In this fast-paced environment, evolving is crucial for keeping a business current and competitive.
To withstand the pressure of evolving in this fast-paced environment, client-server architecture is built. 
It refers to a network-connected architecture in which two or more computers transmit and receive requests from one another.
Let us break it down further.
* Client: In the DevOps world this is refered to as a computer or device also known as `Host`. Client computers provide an interface to allow a computer user to request services of the server and to display the results the server returns
* Server: A server, on the other hand, is a remote computer that waits for client requests before responding to them. A server should ideally provide a standardised transparent interface to clients so that they are unaware of the characteristics of the system (i.e., the hardware and software) that is providing the service.
![image](https://user-images.githubusercontent.com/80969889/208232594-ec2affe5-0041-4678-a488-151c08e8d902.png)
***
This computing strategy works well when clients and servers have distinct tasks to complete on a regular basis. 
In hospital data processing, for example, a client computer may run application software to enter patient information, while the server computer runs another program to administer the database where the information is stored indefinitely. 
Many clients can access the server's information at the same time, and a client computer can perform other tasks, such as sending e-mail. 
The client-server technique varies significantly from the conventional "mainframe" design, in which a centrally located mainframe computer conducted all tasks for its associated "dumb" terminals.

## Client-Server Architecture
<img
  src="https://user-images.githubusercontent.com/80969889/208233440-f60922ba-6a73-4343-bdc7-0b6a2311aa79.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 500px; height: 400px; border: solid 2px red;">
***
<img
  src="https://user-images.githubusercontent.com/80969889/208233537-2dd41c31-bc45-4403-905d-72ee9289e9e9.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 300px; border: solid 2px red;">
***
The client-server architecture denotes a system that hosts, delivers, and manages the majority of the resources and services requested by the client. 
All requests and services are supplied across a network under this approach, which is also known as the networking computer model or client server network. 

A client-server architecture, often known as a client-server model, is a network application that divides duties and responsibilities between clients and servers on the same system or connected via a computer network. 
Multiple users' workstations, PCs, or other devices are often connected to a central server through an Internet connection or other network. 
The client submits a data request, which the server acknowledges and accommodates by transmitting data packets.
Simply put
* The customer first transmits their request using a network-enabled device. 
* The network server then accepts and processes the user's request. 
* Finally, the server sends the response to the client.

The typical client/server design has two levels: the client and the server. 
Another popular client/server system design employs three tiers:
* The User Interface is handled by the Presentation layer (or Client Tier). 
* The application layer (or business tier) is in charge of the detailed processing. 
* The database layer (or Data Tier) is where the information is stored.

The Presentation layer is managed by the Client system, the Application layer by the Application server, and the Database layer is managed by the Server system.

<img
  src="https://user-images.githubusercontent.com/80969889/208234121-01f4baa0-1b31-420c-9f8e-67ef6cbf8bc0.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 500px; height: 650px; border: solid 2px red;">
***
### Characteristics of Client-Server Architecture
* Client and server computers require varying amounts of hardware and software. 
* Client and server computers may be from different manufacturers. 
* Horizontal scalability (expanding the number of client computers) and vertical scalability (migration to a more powerful server or to a multi-server solution).  
* To establish communication and deliver or receive data, a client or server application interacts directly with a transport layer protocol. 
* Lower layer protocols are then used by the transport protocol to deliver and receive individual messages. As a result, a computer needs a whole stack of protocols to operate either a client or a server. 
* A single server-class computer can provide numerous services at the same time; each service requires its own server application.

## Client-Server vs Peer To Peer

In a client-server architecture, a central server is responsible for providing services to client devices. 
The client devices send requests to the server, which processes the requests and sends back a response. 
This architecture is common in many types of networks, including the Internet.

In a peer-to-peer (P2P) architecture, there is no central server. 
Instead, each device on the network acts as both a client and a server, making requests and providing services to other devices on the network. 
P2P networks can be used for many purposes, such as file sharing and communication.

There are several key differences between client-server and P2P architectures:
* Centralization: In a client-server architecture, there is a central point of control and responsibility, while in a P2P network, responsibility is distributed among the devices on the network.
* Scalability: Client-server architectures are generally more scalable than P2P networks, as they can handle a larger number of clients without experiencing performance issues.
* Reliability: In a client-server architecture, the server is a single point of failure, meaning that if it goes down, the entire system may be affected. In a P2P network, there is no central point of failure, so the network may be more reliable.
* Security: Client-server architectures may be more secure than P2P networks, as the server can be better protected from attacks and unauthorized access. However, P2P networks can also be secured through the use of encryption and other security measures.
Overall, the choice between a client-server and P2P architecture depends on the specific needs and requirements of the application or network in question.

<img
  src="https://user-images.githubusercontent.com/80969889/208235034-662006b5-7c5c-4cb3-877b-fb5a83101f31.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 500px; height: 500px; border: solid 2px red;">
***
## Why use Client-Server Architecture
* It’s a centralized system that keeps all the data and its controls in one place.
* It brings a high level of scalability, organization, and efficiency.
* It allows the IT staff to change the client and server capacities separately.
* It’s cost-efficient, especially in terms of maintenance.
* It allows data recovery.
* It allows load-balancing, which optimizes performance.
* It allows different platforms to share resources.
* Users don’t need to log into a terminal or another processor to access corporate information or desktop tools like PowerPoint presenters or spreadsheet utilities.
* The setup reduces the incidence of data replication.

Because nothing in the universe has yet to be perfectly created, things that have advantages typically have drawbacks, which include:
* The network is made up of linked clients and servers, therefore, if the server has a worm, virus, or Trojan, the clients are likely to get it. 
* Denial-of-Service (DoS) attacks are possible on the server. 
* During transmission, data packets might be faked or manipulated. 
* It is costly to set up and deploy at first. If a vital server fails, the clients are out of luck. 
* The configuration is vulnerable to phishing and Man in the Middle (MITM) attacks.

## Examples of Client-Server Architecture
* Web browsers and web servers: When you type a URL into your web browser and hit enter, your browser sends a request to a web server for the corresponding website. The server then sends back the HTML, CSS, and JavaScript files that make up the website, which your browser then renders for you to view.
* Email clients and email servers: When you send an email from your email client (such as Outlook or Gmail), your client sends a request to an email server to send the email on your behalf. The server then delivers the email to the recipient's email server, which passes it along to their email client.
* FTP clients and FTP servers: FTP (File Transfer Protocol) is a protocol used to transfer files over the internet. FTP clients (such as FileZilla) allow you to connect to an FTP server and transfer files to and from the server.
* Remote desktop clients and remote desktop servers: Remote desktop software allows you to remotely control another computer over the internet. A remote desktop client (such as Remote Desktop Connection) sends requests to a remote desktop server, which processes the requests and sends back the display and control information for the remote computer.
* Cloud storage: Cloud storage services like Google Drive and Dropbox use a client-server architecture, with the client uploading and downloading files from the server and the server storing and managing access to the files.
* Online banking: Online banking systems use a client-server architecture, with the client (such as a web browser or mobile app) sending requests to the bank's server to access account information and perform transactions.
* Social media: Social media platforms use a client-server architecture, with the client (such as a web browser or mobile app) sending requests to the server to access and post content, and the server responding with the requested content and updating the user's feed.
* Video streaming: Video streaming services like Netflix and YouTube use a client-server architecture, with the client requesting and receiving video streams from the server.
* Virtual private network (VPN): A VPN service uses a client-server architecture, with the client connecting to a server and routing internet traffic through the server to encrypt the connection and protect the user's privacy.
* File sharing network: A file sharing network allows clients to upload and download files from a central server. The server stores the files and manages access to them, while the clients request access to the files and receive them from the server.
* Online gaming: Online gaming platforms typically use a client-server architecture, with the game client running on the user's device and the game server hosting the game world and managing interactions between players.






