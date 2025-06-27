# Load Balancer Using Socket

## 🔗 Project Description

This project is a **TCP-based Load Balancer** developed as part of the **19AD551 – Computer Networking Laboratory**. It is designed to distribute incoming network traffic efficiently across multiple backend servers using **sockets** and **multithreading**. This ensures high availability, reliability, and better resource utilization.

## 👩‍💻 Team Members

- **Bhuvanika S** - [GitHub](https://github.com/bhuvanika1102)
- **Rajakumari S**
- **Suji S**

## 🚀 Features

- ⚖️ Load balancing across multiple backend servers
- 🔄 Dynamic load handling using multithreading
- 🏗️ Simple TCP socket-based communication
- 🧠 Server selection based on current load
- 💡 Supports basic load balancing strategies
- 🛡️ Fault-tolerant with health check simulation

## 🛠️ Technologies Used

- C (Socket Programming)
- TCP/IP Protocol
- Multithreading with Pthreads
- Linux/Unix Networking APIs

## 📁 Project Structure

```plaintext
load-balancer-socket/
├── client.c           # Client program
├── server1.c          # Backend Server 1
├── server2.c          # Backend Server 2
├── load_balancer.c    # Load Balancer
├── README.md          # Project documentation
```

### 💻 How to Run the Project
## 🖥️ Prerequisites
GCC compiler

Linux/Unix-based OS (or WSL on Windows)

Basic knowledge of terminal commands

🔧 Compilation
Open terminal in your project directory and run:

# Compile servers
```bash
gcc server1.c -o server1 -lpthread
gcc server2.c -o server2 -lpthread
```

# Compile load balancer
```bash
gcc load_balancer.c -o load_balancer -lpthread
```

# Compile client
```bash
gcc client.c -o client
```
🚀 Running the Servers
In separate terminal windows, run:
```bash
# Run Server 1
./server1 6001

# Run Server 2
./server2 6002
```
🔗 Running the Load Balancer
```bash
./load_balancer 6000
```
👨‍💻 Running the Client
```bash
./client
```
📝 Client Input Example
```bash
input: hello
output: HELLO
```
🔄 How It Works
The client connects to the load balancer.

The load balancer queries both servers for their current load.

It compares the load and forwards the request to the least loaded server.

The selected server capitalizes the input string and sends it back to the client
---
## 📞 Contact Me
Feel free to reach out to me via email at bhuvani1102@gmail.com or connect with me on LinkedIn at https://www.linkedin.com/in/bhuvani1102.
