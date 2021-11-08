# 第一個 node JS

## 引入 require

```javascript
const http = require("http");
```

## 建立 Server

這邊使用 `http.createServer()` 建立 server 監聽 8888 port ， 透過 request 和 response 來接收data。

```javascript
const http = require("http");

http.createServer(function(request,response){

  response.writeHead(200,{'content-type':'text/plain'})

  response.end('Hello World\n');
}).listen(8888);

console.log('server running at http://127.0.0.1:8888/')
```

開啟 http://127.0.0.1:8888/ 就可以看見 hello world 。
