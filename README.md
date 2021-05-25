# nodejs

INSTALL
------

https://nodejs.org/en/download/


Download and Unzip the binary archive to any directory you wanna install Node, I use /usr/local/lib/nodejs
```
 VERSION=v14.17.0
 DISTRO=linux-x64
 wget https://nodejs.org/dist/$VERSION/node-$VERSION-$DISTRO.tar.xz
 sudo mkdir -p /usr/local/lib/nodejs
 sudo tar -xJvf node-$VERSION-$DISTRO.tar.xz -C /usr/local/lib/nodejs 
```
Set the environment variable ~/.profile
```
export PATH=/usr/local/lib/nodejs/node-$VERSION-$DISTRO/bin:$PATH

```
Refresh profile
```
. ~/.profile
```
If Refresh profile is not working ->
Edit the profile file
```
nano ~/.profile
nano ~/.bashrc
```

And add at the end the code below
```
 # Nodejs
 VERSION=v14.16.0
 DISTRO=linux-x64
 export PATH=/usr/local/lib/nodejs/node-$VERSION-$DISTRO/bin:$PATH
```

Reload bash term 
Test installation using
```
$ node -v

$ npm version

$ npx -v
```

the normal output is:
```
➜  node -v
v10.15.1
➜  npm version
{ npm: '6.4.1',
 ares: '1.15.0',
 cldr: '33.1',
 http_parser: '2.8.0',
 icu: '62.1',
 modules: '64',
 napi: '3',
 nghttp2: '1.34.0',
 node: '10.15.1',
 openssl: '1.1.0j',
 tz: '2018e',
 unicode: '11.0',
 uv: '1.23.2',
 v8: '6.8.275.32-node.12',
 zlib: '1.2.11' }


```


curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -



### CODE --JavaScript
```
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
```

### TEST
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
