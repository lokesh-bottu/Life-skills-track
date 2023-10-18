# Technical Paper

## What does the OSI Model means?

OSI Model means Open System Interconnection Model. This mainly states that how the data is tranferred from one to one via internet. This OSI model was introduced in 1984.

## Why do we need OSI Model?

Before the OSI model is introduced the data is transferred using LAN cable, but this doesn't works in every situation. For example, one person uses Windows OS and the other uses Linux, or any other OS. So, to overcome this issue OSI model is introduced by  by ISO (Internation Standard Organization).

## How does the OSI Model works?

- Basically this model is divided into 7 layers which includes Application Layer, Presentation Layer, Session Layer, Transport Layer, Network Layer, Datalink Layer, and Physical Layer.
- Initially the  data is transferred from Application to Physical Layer one by one and then it is sent to the user through internet.

### 1) Application Layer

- Application Layer provides services for application which works by internet, with the help of application protocols like HTTPS Protocols, NFS, IRC etc.. to do web surfing. 
- These protocols collectives make an Application Layer, and are used to File transfer, email etc.

### 2) Presentation Layer

- For the Presentaion Layer the data is received from Application layer. The data is stored in form of numbers and characters. But as the computer doesn't understands the human language so it is converted to binary language.
- Presentation Layer reduces the number of bits used by the data which makes the data transmission faster. Also the data is encrypted from the senders end and decrypted at the receiver's end and for this Secure Sockets Layer is used. In simple words the bigger the data the more time it takes.

### 3) Session Layer

- Session Layer helps in making the connection between the sender and receiver.
- Before the connection is setup, the serves performs two different operations.
1. Checks the owner with the help of username and password
2. Checks the request permission is granted for him or not, like downloading the data or sending the data, or modifying the data. Incase if the permissions are not met then this session layer gives an error message.
- Session Layer makes a new copy of all the data present in the server and whenever the user request to download or modify then the files that are stored in the new copy are sent, and this process is known as Session Management.

### 4) Transport Layer

- Transport Layer segments the data into smaller parts and each segmented part contains the sequence number and port number. Port number is used to know the application to which it is sent.
Sequence number tells the sequence number of the message.
For Eg. if the message is How are you then each word will be having a seq number inorder to send it in the same order, and this process is known as Segmentation
- Transport Layer also performs Flow control. For example if the receiving speed of the receiver is less than the sending speed of sender then this comes into picture and control the speed from the both the sides and vice versa.
- This also performs Error control in case of missing data. 
This consists of 2 protocols 
#### 1. TCP (Transmission Control Protocol) used for connection oriented communication
- In this case the missing data can be retrieved because this tells whether the data is completely received or not using the checksum process, so as a result this works slower.
#### 2. UDP (User Datagram Protol) used for connection less communication.
- In this case the feedback is not provided and hence no missing data can be retrieved and hence this also works faster


### 5) Network Layer







