# Week_3 Day_1 Notes

### HTTP review: 
* Hypertext transfer protocol
* the http library is packed into nodejs runtime -- no need to import
* http is language agnostic and works over tcp

* Request -- Response cycle based - only get response to a request [x]
* it is a very popular protocol that dominates the web
* http has a secure cousine called https

**Request** 

- Methods -- GET/POST/PUT/PATCH/DELETE
- url

**Response**
- Status COde (100 / 200 / 300 / 400 / 500)
- Body (html, string, json)

**HTTP Stateless**
- Server's got amnesia

### HTTP Server - Demo [40m]

```JavaScript

// Server.js

// Get server set up
const http = require('http');
const server = http.createServer();

// get it (server) listening for requests 
  // obj.on("event", functionToHandleEvent)
server.on("request", (request, response)=>{
  const { url, method } = request;
  if (url === '/' && method === 'GET'){
    response.end("Welcome Home");
  }else if (url === '/rand' && method === "GET"){
    response.end(Math.random())
  }else{
  response.end("Response not found")
  }
  response.end("Response from server")
});
server.listen(3000, ()=>{
  console.log("server is listening")
})
// get it to respond to requests



```

```NodeJS
  npx nodemon -L node 'filename'
```

**Express**

```JavaScript
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send("Home from express.js");
})
app.listen(port, () => {
  console.log(`Server listening on ${port}`)
})

```