# Developing a Simple Webserver
Name:Abdullah.R
Ref no:23013613


# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using python code


## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver

# PROGRAM:
#Type your code here:
```
from http.server import HTTPServer, 
BaseHTTPRequestHandler
content = """
<!doctype html>
<html>
<head>
<title>Top Five </title>
</head>
<body>
<h1>Top Five Application Development Frameworks</h1>
<h3>1.Django</h3>
<h3>2.MEAN Stock</h3>
<h3>3.React</h3>
</body>
</html>

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
![Alt text](webserver.png)


# RESULT:

The program is executed succesfully
