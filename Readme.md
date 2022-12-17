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
* A client that communicates with the user. 
* An application server that houses the program's business logic. 
* A data storage resource manager.
<img
  src="https://user-images.githubusercontent.com/80969889/208234121-01f4baa0-1b31-420c-9f8e-67ef6cbf8bc0.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 400px; height: 300px; border: solid 2px red;">
***
### Characteristics of Client-Server Architecture
* Centralized resource management: The server manages the resources that are shared among the clients, such as data storage and processing power.
* Improved scalability: Because the server can handle multiple requests from different clients at the same time, the client-server architecture is more scalable than a peer-to-peer architecture, where each device acts as both a client and a server.
* Improved security: The server can enforce security policies and controls, such as authentication and access controls, to protect the shared resources.
* Dependency on the server: Because the clients depend on the server to provide resources and services, the server must be available and reliable. If the server goes down, the clients will not be able to access the resources or services.
* Asymmetric communication: In a client-server architecture, the client initiates communication with the server and the server responds. This is in contrast to a symmetric communication model, where both parties can initiate communication.

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



























