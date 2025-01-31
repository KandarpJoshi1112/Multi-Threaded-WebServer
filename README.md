# MultiThreaded WebServer

## Overview
The **MultiThreaded WebServer** is a lightweight, concurrent server implementation in Java that can handle multiple client connections simultaneously. This project includes a server that responds to client requests and a client that can initiate multiple concurrent requests. Additionally, a JMeter test plan is provided for load testing and performance evaluation.

## Features
- Multi-threaded architecture to handle multiple client requests concurrently.
- Lightweight implementation using Java sockets.
- Simple request-response mechanism.
- Load testing capability using JMeter.


## How It Works
- The **server** listens on a specified port (default: 8080) and accepts client connections.
- Each incoming client request is handled in a separate thread.
- The **client** initiates multiple connections to test concurrency.
- The **JMeter test plan** allows benchmarking and capacity testing.

## Setup and Usage
### Prerequisites
- Java (JDK 8 or later)
- Apache JMeter (for load testing)

## Running the Project
1. **Compile the files:**
   ```sh
   javac Server.java Client.java
   ```
2. **Start the server:**
   ```sh
   java Server
   ```
3. **Run the client in a separate terminal:**
   ```sh
   java Client
   ```
### Should Look Like Following

![Screenshot (8)](https://github.com/user-attachments/assets/3de3aa1d-1a81-46d3-ab6f-7357d40d1a0e)


## Now Load Testing with JMeter
1. Open `Jmeter.jmx` in Apache JMeter.
2. Configure the number of threads (users) and test duration.
3. Run the test to analyze performance metrics such as response time and throughput.

## Performance Testing
- The JMeter test plan simulates **30,000 concurrent users** over **30 seconds**.
- Performance metrics such as response time, success rate, and error handling are collected.
- The test plan includes graphical and tabular result analysis.

### Following are Test Results simulating **30,000 concurrent users** over **30 seconds**.
![Screenshot (9)](https://github.com/user-attachments/assets/1fee883c-89a3-43dc-80aa-656b7f634f4e)
![Screenshot (10)](https://github.com/user-attachments/assets/29df9a3d-0ce2-49ea-878c-38c7f9ba9ae6)
![Screenshot (11)](https://github.com/user-attachments/assets/e1c431c3-6d0c-46f1-9a6a-7e933fba1ebf)

👤 **Kandarp Joshi**

* Github: [@Kandarp Joshi](https://github.com/KandarpJoshi1112)
* LinkedIn: [@Kandarp Joshi](https://www.linkedin.com/in/kandarp-joshi-3451231bb/)

Enjoy coding! 🚀
