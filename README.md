# ft_irc

`ft_irc` is a 42 School group project focused on network programming in C++.

The goal of the project is to build an IRC server compatible with IRC clients, using TCP sockets and a non-blocking server architecture.

This project helped me strengthen my understanding of client/server communication, file descriptor management, command parsing and real-time network interactions.

## My Contribution

This was a group project.  
My main contribution was focused on the networking part of the server, especially:

- TCP socket setup and server initialization
- File descriptor management
- Handling multiple client connections
- Client accept / disconnect logic
- Non-blocking network communication
- Reading and parsing incoming client messages
- Sending server responses to connected clients
- Improving the network architecture and reliability

I mainly worked on the `feature/rewrite-network` branch.

## Features

- IRC server written in C++
- Multiple clients handled simultaneously
- TCP socket communication
- File descriptor based client management
- Command parsing
- Channel management
- Private messages
- User authentication with server password
- Nickname and username handling
- Basic IRC protocol behavior

## Technologies

- C++
- TCP sockets
- File descriptors
- Linux / UNIX system calls
- Makefile
- IRC protocol

## Installation

Clone the repository:

```bash
git clone https://github.com/KillianSupinski/ft_irc.git
cd ft_irc
```

Compile the project:
```bash
make
```
Or:
```bash
make debug
```
## Usage

Run the server with a port and a password:
./ircserv <port> <password>
```bash
./ircserv 6667 mypassword
```
Then connect with an IRC client:
```bash
nc -c localhost 6667
```

## Example Commands
```bash
PASS mypassword
NICK killian
USER killian 0 * :Killian Supinski
JOIN #general
PRIVMSG #general :Hello everyone!
```
