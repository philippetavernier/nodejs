# nodejs

INSTALL
------
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -



CODE --JavaScript

// Load the http module to create an http server.
var http = require('http');
 
// Configure our HTTP server to respond with Hello World to all requests.
var server = http.createServer(function (request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.end("Hello World\n");
});
 
// Listen on port 8000, IP defaults to 127.0.0.1
server.listen(8000);
 
// Put a friendly message on the terminal
console.log("Server running at http://127.0.0.1:8000/");
Nous enregistrons et fermons ensuite l’éditeur (CTRL + O, CTRL + X). Vous pouvez maintenant démarrer le serveur en entrant simplement ce qui suit dans le terminal :


TEST
node hello-world.js



Link 
----
https://github.com/nodejs/help/wiki/Installation
https://nodejs.org/en/download/

https://nodejs.org/en/docs/guides/

https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04-fr

INSPECT NODEJS
https://www.youtube.com/watch?v=Xb_0awoShR8
https://docs.google.com/presentation/d/1i5JREE3hhtG4FDip97zFJpMG_qb8k6fb5BRF09eyYTM/view

VIDEO COMMENT
-------------
1-Download nodejs LTS version
VERSION=v14.15.4
DISTRO=linux-x64
export PATH=/usr/local/lib/nodejs/node-$VERSION-$DISTRO/bin:$PATH

2-Test node webapp
https://nodejs.org/en/docs/guides/
