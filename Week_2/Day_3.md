# Day_3 notes Week_2
HTTP - Hyper Text Transfer Protocol

Protocol -- the official procedure or system of rules governing affairs of state or diplomatic occasion.

For internet protocols -- are the rules that determine how to send, format and recieve data between computers.

OSI -- 7 layers
  7. Application layer -- Human-computer interaction layer, where users can access the network services
  6. Presentation Layer -- Ensures that data is in a usable format and where data encryption occurs
  5. Session Layer -- Maintains connection and is responsible for controlling port and seesions (on-going communication of 2 devices)
  4. Transport Layer -- Trasmits data using transmission protocoal including TCP, UDP, and ITP
  3. Network Layer -- Decides wheich physical path the data will take
  2. Datalink Layer -- Defines the format of data on the network
  1. Physical Layer -- transmits raw bit stream over the physical medium

TCP -- Transmistion Control Protocol - used to establish networked communication between applications. Exists at the transport layer of the OSI model. it is built on top of the IP (Internet Protocol) and is responsible for dividing a floe into segments to be sent through IP and combining those segments back into a file when they are recieved. 
  * connection oriented
    * connection has to be established between two parties before info is sent
  * congestion controll
  * error detection
  * lost data handling
  * adds port

Accuracy > Speed


HTTP -- Request <-> response