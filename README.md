
# MyTCP Library

The MyTCP Library is a reliable and in-order message delivery software library that operates over standard TCP sockets. It ensures the accurate and sequential transmission and reception of messages up to 5000 bytes.

## Features

- **Reliable and In-Order Delivery**: Messages sent using the MyTCP protocol are guaranteed to be delivered reliably and in the same order they were sent, ensuring data integrity.

- **Utilization of POSIX Threads**: The library leverages POSIX threads to enable concurrent execution of multiple threads, facilitating efficient handling of message transmission and reception.

- **Mutex Locks and Conditional Signals**: Synchronized access to global message buffers is ensured through the use of mutex locks and conditional signals. This prevents data races and facilitates proper coordination among threads that access shared resources.

- **Graceful Closure**: When closing the socket connection, all global data structures utilized by the MyTCP Library are cleared to maintain a clean state and prevent resource leaks.

## Usage

To incorporate the MyTCP Library into your project, follow the steps below:

1. Include the MyTCP Library in your project's source code or link it as a shared library.

2. Initialize the MyTCP Library and establish a connection between the sender and receiver using standard TCP sockets.

3. Utilize the provided API functions to send and receive messages using the MyTCP protocol. These functions handle reliable and in-order delivery of messages, ensuring data integrity.

4. Close the socket connection appropriately, ensuring that all global data structures are cleared.


## Requirements
For running this application we will need:
```
LinuxOS
gcc
```

## How To Run
```
make
./server
./client
(run ./server and ./client in different terminals)
```

## This project was made by Kriti Bhardwaj (20CS30028) and Vinod Meena (20CS10074)
