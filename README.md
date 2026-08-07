# Echoserver
Echo server and client using python socket
# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

HTML content creation is done

### Step 2:

Design of webserver workflow

### Step 3:

Implementation using Python code

### Step 4:

Serving the HTML pages.

### Step 5:

Testing the webserver

## PROGRAM:
```
client.py

import socket


HOST = "127.0.0.1"  # The server's hostname or IP address
PORT = 65432  # The port used by the server


with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
    s.connect((HOST, PORT))
    s.sendall(b"Hello, world")
    data = s.recv(1024)


print(f"Received {data!r}")

```
```
server.py

import socket

HOST = "127.0.0.1"
PORT = 65432

with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
    s.connect((HOST, PORT))
    s.sendall(b"Kanimozhi,25004451")
    data = s.recv(1024)

print(f"Received {data!r}")

```



## OUTPUT:
### CLIENT OUTPUT:
<img width="1280" height="800" alt="kali ep image 2" src="https://github.com/user-attachments/assets/a53de544-dfba-4df1-989f-f9369bb24c90" />


### SERVER OUTPUT:
<img width="1280" height="800" alt="kali ep 1" src="https://github.com/user-attachments/assets/409a891b-6f58-4b89-9946-28896adff537" />

## RESULT:
The program is executed succesfully
