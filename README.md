# Reflection
##  Commit 1 Reflection notes
Sets up a TCP server using the TcpListener module, binding it to the localhost address 127.0.0.1 and port 7878. It initiates an infinite loop to continuously listen for incoming connections. Upon receiving a connection, it unwraps the result using stream.unwrap() to handle any potential errors. Then it passes the obtained stream to a function called handle_connection() for further processing.

## Commit 2 Reflection notes
![Commit 2 screen capture](/assets/images/commit2.png)

## Commit 2 Reflection notes
The refactor that I add is to use If else to load the page by the status response
![Commit 3 screen capture](/assets/images/commit3.png)

## Commit 2 Reflection notes
The `/sleep` is slower because the thread we set to sleep for 10 second using this code: `thread::sleep(Duration::from_secs(10));`
