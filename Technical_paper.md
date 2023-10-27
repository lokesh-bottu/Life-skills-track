# Technical Paper

## Introduction of OSI Model

OSI Model means Open System Interconnection Model. This mainly states that how the data is tranferred from one to one via internet. This OSI model was introduced in 1984.

## Why do we need OSI Model?

Before the OSI model is introduced the data is transferred using LAN cable, but this doesn't works in every situation. For example, one person uses Windows OS and the other uses Linux, or any other OS. So, to overcome this issue OSI model is introduced by ISO (Internation Standard Organization).

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
- Before the connection is setup, the server performs two different operations.
1. Checks the owner with the help of username and password
2. Checks the request permission is granted for him or not, like downloading the data or sending the data, or modifying the data. Incase if the permissions are not met then this session layer gives an error message.
- Session Layer makes a new copy of all the data present in the server and whenever the user requests to download or modify then the files that are stored in the new copy are sent, and this process is known as Session Management.

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
- Initially the segments are being recieved from the Transport Layer.
- Now the Network Layer assigns the IP address of sender and receiver which are unique in IPv4 or IPv6 format this is known as Logical Address.Basically ipv4 uses for smaller network and ipv6 for larger networks.
- When user requests some data from the server then the network layer assigns the IP address for the user and server and then the data is sent in the form of packets, and this data will be only sent to the requested source, this process is known as Routing.
- The Network Layer also determines the path which means that there could be multiple ways of going from server to receiver, so this chooses the path which takes less time to deliver the packet.

### 6) Data Link Layer
- Data Link Layer receives the data from the network layer. Now the data packets will have the address of sender and receiver.
- In Data link layer the twelve digit of MAC Addresses are assigned and the frame is formed.
- Frame will be in the following format
-   ##### MAC1|MAC2|SEGMENT IP1 IP2

### 7) Physical Layer
- Before the data is transferred here the data is encrypted at the presentation layer, assigned the IP addresses at the network layer,
given the MAC addresses in data link layer and frame is formed.
- Now the Physical Layer coverts the bits into signals and transmits to the local media.
- It will be a light signal in case of Optical fibres and electric signals in case of copper wire or LAN cable, and Radio Signals in case of air as medium. This will be completely dependent on the device which we use to connect the devices.
- Now at the receiver's end the signals are converted to the bits again in the physical Layer and again transferred to the data link layer to undo the things done at sender by each layer.


### Conclusion

- Once the data is recieved to the Physical Layer at the receiver's end then it again converts the signals into bits.
- Each layer reverses the actions performed at the sender's end.
- After the data is passed to the Application Layer, at the reciver's end the data will be shown.

### References

- https://www.youtube.com/watch?v=vv4y_uOneC0"
- https://www.geeksforgeeks.org/open-systems-interconnection-model-osi/
- https://www.youtube.com/watch?v=1msEo8PIcbw








