# Developing a Simple Webserver
<<<<<<< HEAD
Name:Abdullah.R
Ref no:23013613

=======
Name: Karthi Govindharaju
ID: ISAI005
>>>>>>> 6f3272c27c06bbb1138b69891385a44fd121bf34

# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

from http.server import HTTPServer, BaseHTTPRequestHandler
content = """

<html>
<head>
<title>details</title>
 </head>
<body>
<h1 style="border:20px solid red","background-color:blue";>Details of myself</h1>
<hr>
<h4>NAME:Abdullah.R<h4>
<h4>AGE:19</h4>
<h4>NAME OF UNIVERSITY:Saveetha</h4>
<h4>DEPARTMENT:AIDS</h4>
<h4>REG_NO:23013613</h4>
<hr>
<p style=color:red;>the details are correct and are entered by me</p>

</body>
</html>
"""

class HelloHandler (BaseHTTPRequestHandler):
     def do_GET (self):
        self.send_response(200)
        self.send_header('Content-type', 'text/html; charset=utf-8')
        self.end headers ()
        self.wfile.write(content.encode())
        server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()


## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
```python
from http.server import HTTPServer, BaseHTTPRequestHandler
content = """

<html>
<head>
<title>details</title>
</head>
<body>
<h1 style="border:20px solid red","background-color:blue";>Details of myself</h1>
<hr>
<h4>NAME:Abdullah.R<h4>
<h4>AGE:19</h4>
<h4>NAME OF UNIVERSITY:Saveetha</h4>
<h4>DEPARTMENT:AIDS</h4>
<h4>REG_NO:23013613</h4>
<hr>
<p style=color:red;>the details are correct and are entered by me</p>

</body>
</html>
"""

class HelloHandler (BaseHTTPRequestHandler):
     def do_GET (self):
        self.send_response(200)
        self.send_header('Content-type', 'text/html; charset=utf-8')
        self.end headers ()
        self.wfile.write(content.encode())
        
server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()
```

# OUTPUT:
![Output](images/webserver1.png)



# RESULT:

The program is executed succesfully
