# docker-node
docker node template

# npm install
docker run -w /usr/src/app -v <Your directory that contains package.json>:/usr/src/app node npm --loglevel=warn install

# install websocket cli command
https://github.com/vi/websocat#installation

# browser script example

```javascript
// Create WebSocket connection.
const socket = new WebSocket('ws://localhost:8080');

// Connection opened
socket.addEventListener('open', function (event) {
    socket.send('Hello Server!');
});

// Listen for messages
socket.addEventListener('message', function (event) {
    console.log('Message from server ', event.data);
    });
```
