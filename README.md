# Reverse-Shell-Prototype

## Introduction

- **Shell shoveling**, in network security, refers to the act of redirecting the input and output of a shell to a service so that it can be remotely accessed. In computing, the most basic method of interfacing with the operating system is the shell.

- A **reverse shell** is a shell session established on a connection that is initiated from a remote machine, not from the local host. Attackers who successfully exploit a remote command execution vulnerability can use a reverse shell to obtain an interactive shell session on the target machine and continue their attack.

## Requirements
- **Language :** *Python 3 or above.*

- **Libraries :**
  - ***OS***
    - **Usage :** *It provides functions for interacting with the operating system.*
  - ***Socket***
    - **Usage :** *It is a way of connecting two nodes on a network to communicate with each other.*
  - ***SubProcess*** 
    - **Usage :** *It is used to run new applications or programs through Python code by creating new processes.*
  - ***SYS***
    - **Usage :** *It provides various functions and variables that are used to manipulate different parts of the Python runtime environment.*

## Algorithm of this Project

- Run `server.py` in the background (in your workstation). 
- You can do this by typing `python server.py` in the terminal window.
- It will create a socket server and will be listening to the port 8888 (manually set).
- Now you need to run the file `client.py` in the device you want to control.
- You can do this by typing `python client.py` in the terminal window.
- On running it for the first time, a request will be sent to the server running on your machine. 
- The server will acknowledge that request and will respond with bash commands you enter in the shell.
- Same commands will be carried out in the client and the final response will be printed out on your shell.
- **NOTE :**  Though it might look like you are running those commands on your machine but you have actually connected to the target (client).