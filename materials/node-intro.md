# Node.js

## What is Node.js?

**Node.js** is a powerful and versatile open-source runtime environment for
executing JavaScript code on the server side. It enables developers to build
scalable network applications with ease.

### Key Features of Node.js

- **Open Source**: Node.js is free to use and open-source, with a vibrant
  community of contributors.
- **Cross-Platform**: Node.js runs on various operating systems including
  Windows, Linux, Unix, and macOS.
- **JavaScript Runtime**: Node.js uses JavaScript, allowing developers to use
  the same language for both client-side and server-side development.
- **Asynchronous and Event-Driven**: Node.js uses a non-blocking, event-driven
  architecture to handle concurrent operations efficiently.
- **Built on V8 Engine**: Node.js is built on Chrome's V8 JavaScript engine,
  which compiles JavaScript directly to native machine code for high
  performance.

![Node.js Overview](../assets/nodejs-overview.png)

## Core Concepts

### 1. Asynchronous Programming

Node.js utilizes an asynchronous, non-blocking I/O model, which helps in
building highly scalable applications.

```javascript
const fs = require("fs");

// Non-blocking asynchronous read
fs.readFile("example.txt", "utf8", (err, data) => {
  if (err) throw err;
  console.log(data);
});

console.log("This will log before the file content.");
```

### 2. Event Loop

The event loop is a core feature of Node.js that manages and dispatches events
or messages. It allows Node.js to perform non-blocking operations.

```javascript
const EventEmitter = require("events");
const myEmitter = new EventEmitter();

myEmitter.on("event", () => {
  console.log("An event occurred!");
});

myEmitter.emit("event");
```

### 3. NPM (Node Package Manager)

NPM is the default package manager for Node.js, which hosts thousands of
libraries and tools for Node.js development.

- **Install a package**:

  ```sh
  npm install <package-name>
  ```

- **Install a package globally**:

  ```sh
  npm install -g <package-name>
  ```

- **Uninstall a package**:

  ```sh
  npm uninstall <package-name>
  ```

- **Update packages**:

  ```sh
  npm update
  ```

### 4. Modules

Node.js uses modules to organize code into reusable components. There are
built-in modules, third-party modules, and custom modules.

- **Built-in Module Example**:

  ```javascript
  const http = require("http");

  http
    .createServer((req, res) => {
      res.writeHead(200, { "Content-Type": "text/plain" });
      res.end("Hello World\n");
    })
    .listen(8080);
  ```

- **Custom Module Example**:

  **`math.js`**:

  ```javascript
  module.exports.add = (a, b) => a + b;
  ```

  **`app.js`**:

  ```javascript
  const math = require("./math");
  console.log(math.add(2, 3)); // 5
  ```

## Getting Started with Node.js

### 1. Install Node.js

Download and install Node.js from the [official website](https://nodejs.org/).
The installation includes NPM.

### 2. Verify Installation

Check the installed versions of Node.js and NPM:

```sh
node -v
npm -v
```

### 3. Create Your First Node.js Application

Create a file named `app.js` with the following content:

```javascript
console.log("Hello, Node.js!");
```

Run the application:

```sh
node app.js
```

### 4. Create a Simple Web Server

Create a file named `server.js` with the following content:

```javascript
const http = require("http");

const hostname = "127.0.0.1";
const port = 3000;

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader("Content-Type", "text/plain");
  res.end("Hello World\n");
});

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}/`);
});
```

Run the server:

```sh
node server.js
```

Visit `http://127.0.0.1:3000/` in your web browser to see "Hello World".

## Advanced Topics

### 1. Express.js

**Express.js** is a popular web framework for Node.js, designed for building web
applications and APIs.

- **Install Express**:

  ```sh
  npm install express
  ```

- **Basic Express App**:

  ```javascript
  const express = require("express");
  const app = express();

  app.get("/", (req, res) => {
    res.send("Hello World!");
  });

  app.listen(3000, () => {
    console.log("App is listening on port 3000!");
  });
  ```

### 2. Asynchronous Programming with Promises and Async/Await

**Promises** and **async/await** are modern JavaScript features for handling
asynchronous operations.

- **Promise Example**:

  ```javascript
  const fs = require("fs").promises;

  fs.readFile("example.txt", "utf8")
    .then((data) => console.log(data))
    .catch((err) => console.error(err));
  ```

- **Async/Await Example**:

  ```javascript
  const fs = require("fs").promises;

  async function readFile() {
    try {
      const data = await fs.readFile("example.txt", "utf8");
      console.log(data);
    } catch (err) {
      console.error(err);
    }
  }

  readFile();
  ```

## Resources

- [Official Node.js Documentation](https://nodejs.org/en/docs/)
- [NPM Documentation](https://docs.npmjs.com/)
