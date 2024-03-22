# Reflection
##  Commit 1 Reflection notes
Sets up a TCP server using the TcpListener module, binding it to the localhost address 127.0.0.1 and port 7878. It initiates an infinite loop to continuously listen for incoming connections. Upon receiving a connection, it unwraps the result using stream.unwrap() to handle any potential errors. Then it passes the obtained stream to a function called handle_connection() for further processing.

## Commit 2 Reflection notes
Returning an HTML file as a response to the incoming request. The response is a simple HTML file with a status code of 200 OK.
![Commit 2 screen capture](/assets/images/commit2.png)

## Commit 3 Reflection notes
Add another HTML file then refactor the `main.rs` file using if else statement to handle the request. If the request is `/` it will return the `hello.html` file, if the request is none of it will return the `404.html` file.
![Commit 3 screen capture](/assets/images/commit3.png)

## Commit 4 Reflection notes
The `/sleep` is slower because the thread we set to sleep for 10 second using this code: `thread::sleep(Duration::from_secs(10));`

## Commit 5 Reflection notes
A set of launched threads that are prepared and waiting to take on a task is known as a thread pool. One of the threads in the pool is assigned to each new job that the program gets, and that thread is responsible for processing it. While the first thread is processing, the other threads in the pool can take on any additional work. Upon completion of its duty, the initial thread returns to the idle pool, prepared to take on a new assignment. By processing connections concurrently, a thread pool boosts the server's throughput.