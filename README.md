# Threads in web apps
## Browser multithreading based on worker

### Simply a pool of web workers

This is an example of in browser javascript multi threading built using the asyn/await approach.

It allows running a task this way:
    const result = await pool.run(task);
Meaning the task will be executed in a background thread thus non blocking the main thread and resolves the promise when finished.

However this approach is limiting what your task may look like and what can be executed in threads. 
For more advenced usage of multithreading you can consider creating instances of the Thread by passing your own worker factory when creating a pool. 


