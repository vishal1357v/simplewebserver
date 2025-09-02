# EX01 Developing a Simple Webserver
## Date: 25/08/2025
## Name : Vishal P
## Reg no: 212224230306

## AIM:
To develop a simple webserver to serve html pages and display the list of protocols in TCP/IP Protocol Suite.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Import the necessary modules.

### Step 5:
Define a custom request handler.

### Step 6:
Start an HTTP server on a specific port.

### Step 7:
Run the Python script to serve web pages.

### Step 8:
Serve the HTML pages.

### Step 9:
Start the server script and check for errors.

### Step 10:
Open a browser and navigate to http://127.0.0.1:8000 (or the assigned port).

## PROGRAM:

```
from http.server import HTTPServer, BaseHTTPRequestHandler 
class MyServer(BaseHTTPRequestHandler):
    def do_GET(self):
        print("Get request received...")
        self.send_response(200) 
        self.send_header("content-type", "experiment1/html")       
        self.end_headers()
        self.wfile.write(content.encode())

print("Experiment1") 
server_address =('',8000)
httpd = HTTPServer(server_address,MyServer)

<html>
    <head><title> my first page</title></head>
    <body>
        <table align="left" border="5" cellpadding="10">
            <caption> LIST OF PROTOCOLS IN TCP/IP PROTOCOL SUITE</caption>
            <tr><th>>S.no</th><th>Name of the layer</th><th>Name of the protocol</th></tr>
            <tr><td>1</td><td>application layer</td><td>HTTP, FTP, DNS,telnet & SSH</td></tr>
            <tr><td>2</td><td>transport layer</td><td>TCP/UDP</td></tr>
            <tr><td>3</td><td>network layer</td><td>IPV4/IPV6</td></tr>
            <tr><td>4</td><td>link layer<t</td><td>Ethernet</td></tr>
           
            

        </table>
    </body>
    


</html>
```



## OUTPUT:

<img width="1152" height="142" alt="Screenshot 2025-09-02 121652" src="https://github.com/user-attachments/assets/812f51f5-1eb3-440b-8c92-f9f79253b7cf" />
<img width="710" height="482" alt="Screenshot 2025-09-02 121819" src="https://github.com/user-attachments/assets/40934012-4e12-4ba1-9e6d-481837768840" />




## RESULT:
The program for implementing simple webserver is executed successfully.
