# Threads in web apps
## Browser multithreading based on Web Worker API

### Pool of web workers

This is an example of in browser javascript multi threading using the asyn/await approach.

Usage example:
    `const result = await pool.run(task);`

The task will be executed in a background thread, not blocking the main thread and resolves the promise when finished.
Shared web worker is a good place for a web socket connection or cpu intencive calculations. 
