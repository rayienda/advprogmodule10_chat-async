## Original code, and how it runs
![](images/async-chat-1.png)

How to run chat: Set up 4 terminals
- 1 terminal will be used as the server, run 
```bash
cargo run --bin server
```
- 3 terminals will be used as the clients, run 
```bash
 cargo run --bin client
 ```

 From the screenshot above, we can observe that when a client sends a message, the server receives it and broadcasts it to all connected clients, including the sender. This works because the server keeps track of every connected client and listens for messages. Once a message is received from any client, the server forwards it to all active connections.

