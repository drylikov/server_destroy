# Server destroy.

Enable destroying a server, and all currently open connections.

## Usage

```javascript
var enableDestroy = require('server_destroy');

var server = http.createServer(function(req, res) {
  // do stuff, blah blah blah
});

server.listen(PORT);

// enhance with a 'destroy' function
enableDestroy(server);

// some time later...
server.destroy();
```
