# Curl
cURL is a command-line tool that lets you make HTTP requests and see the raw responses. It’s great when you need something precise or don’t have access to a browser-based tool.
Applications, like our browsers, communicate with servers using HTTP (Hypertext Transfer Protocol). Think of HTTP as the language for asking a server for resources (pages, images, JSON data) and getting answers back.

curl http://10.64.170.175/  -- what it does -What happens after running the command is that curl sends an HTTP GET request for the site's home page. An HTTP response is received containing the body, which is then printed in the terminal. Because this is a terminal, instead of rendering the webpage, what you'll see is the text representation of the page in HTML.


sending POST request-Suppose you've found a login form whose POST target is /post.php. When you log in through a browser, it sends a POST request to the server containing the credentials you entered. We can simulate this directly from the terminal

curl -X POST -d "username=user&password=user" http://10.64.170.175/post.php
