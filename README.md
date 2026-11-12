<div align="center">

# 🟢 Learning Node.js

**My hands-on notes and practice scripts for learning the fundamentals of Node.js, one numbered file at a time.**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)

</div>

---

## 📖 Overview

Each file in this repo covers one core Node.js concept with a small, runnable example. Work through them in order to go from "hello world" to a basic HTTP server.

## 📚 Topics Covered

| # | File | Concept |
|---|---|---|
| 01 | [`01-intro.js`](01-intro.js) | First Node script |
| 02 | [`02-globals.js`](02-globals.js) | Globals: `__dirname`, `__filename`, `require`, `module`, `process` |
| 03 | [`03-modules.js`](03-modules.js) | CommonJS modules: importing other files |
| 04 | [`04-names.js`](04-names.js) | Exporting several values with `module.exports = { ... }` |
| 05 | [`05-utils.js`](05-utils.js) | Exporting a single function |
| 06 | [`06-alternative-flavor.js`](06-alternative-flavor.js) | Another way to export: `module.exports.x = ...` |
| 07 | [`07-mind-grenade.js`](07-mind-grenade.js) | Code in a required module runs on import |
| 08 | [`08-os-module.js`](08-os-module.js) | Built-in `os` module: user info, uptime, memory |
| 09 | [`09-path-module.js`](09-path-module.js) | Built-in `path` module: `join`, `basename`, `resolve` |
| 10 | [`10-fs-sync.js`](10-fs-sync.js) | Reading and writing files synchronously |
| 11 | [`11-fs-async.js`](11-fs-async.js) | Reading and writing files with callbacks |
| 12 | [`12-http.js`](12-http.js) | Creating a basic HTTP server with routes |

### 🔁 Event loop examples

| File | Shows |
|---|---|
| [`1-read-file.js`](1-event-loop-examples/1-read-file.js) | Async file reads run after synchronous code |
| [`2-setTimeout.js`](1-event-loop-examples/2-setTimeout.js) | `setTimeout(..., 0)` still waits for the call stack to clear |
| [`3-setInterval.js`](1-event-loop-examples/3-setInterval.js) | Intervals keep the process alive |
| [`4-server.js`](1-event-loop-examples/4-server.js) | A server keeps listening for request events |

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 18 or newer

### Run

```bash
git clone https://github.com/Happytyagi1/node.git
cd node
npm install

# run any lesson
node 01-intro.js
node 08-os-module.js

# run app.js with auto-reload (nodemon)
npm start
```

> 💡 Scripts that read files (`10`, `11` and `1-read-file.js`) use paths relative to the repo root, so run them from there.

## 📁 Project Structure

```
.
├── 01-intro.js … 12-http.js     # Numbered lessons
├── 1-event-loop-examples/       # Event loop demos
├── content/                     # Sample text files used by the fs lessons
├── app.js                       # Scratch file run by `npm start`
└── package.json                 # lodash + nodemon
```

<div align="center">

Made with ❤️ by **Happy Tyagi**

</div>
