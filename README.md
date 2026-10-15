<div align="center">

# 🚀 Top 100 Node.js Interview Questions and Answers (2026)

### Beginner to Advanced • Easy Indian English • Code Examples • Interview Tips

![Node.js](https://img.shields.io/badge/Node.js-Interview_Preparation-339933?style=for-the-badge&logo=nodedotjs&logoColor=white) ![Questions](https://img.shields.io/badge/Questions-100-blue?style=for-the-badge) ![Level](https://img.shields.io/badge/Level-Beginner_to_Advanced-orange?style=for-the-badge) ![Year](https://img.shields.io/badge/Updated-2026-purple?style=for-the-badge)

**Made with ❤️ by [Code with Jamshed](https://github.com/Jamshed7664)**

</div>

---

> ⭐ **If you find this repository helpful, please give it a star and share it with developers preparing for Node.js interviews.**

## 📖 About This Repository

A complete **Node.js interview preparation guide** with **100 frequently asked questions**, clear answers in **easy Indian English**, short practical examples and an **interview tip** for each question. Designed for freshers and experienced backend developers.

**Examples:** Most runnable Node.js snippets use CommonJS (`require`) unless an ES module is explicitly shown. Some snippets demonstrate Express or other packages and mention required installations. Terminal commands and pseudocode are labelled.

**Recommended runtime:** Use a supported Node.js LTS release for real applications. As of **15 October 2026**, Node.js **24.x** is Active LTS and **26.x** is Current; check [the official release schedule](https://github.com/nodejs/Release) for updates.

## ⚙️ Quick Start

```bash
node --version
npm --version
mkdir nodejs-interview-practice && cd nodejs-interview-practice
npm init -y
node app.js
```

Create `app.js` before running the last command. For Express examples, first install the stated packages.

## 🧭 Table of Contents

| Section | Questions | Jump |
|---|---:|---|
| Node.js Fundamentals | 1–15 | [Open section](#nodejs-fundamentals) |
| Modules & Core APIs | 16–30 | [Open section](#modules-core-apis) |
| Async Programming & Event Loop | 31–48 | [Open section](#async-programming-event-loop) |
| HTTP, APIs & Networking | 49–63 | [Open section](#http-apis-networking) |
| Streams, Files & Performance | 64–77 | [Open section](#streams-files-performance) |
| Security, Testing & Production | 78–100 | [Open section](#security-testing-production) |

<details>
<summary><strong>📚 Expand all 100 questions (click to navigate)</strong></summary>

1. [Q1. What is Node.js?](#q1-what-is-nodejs)
2. [Q2. How is Node.js different from JavaScript?](#q2-how-is-nodejs-different-from-javascript)
3. [Q3. Why is Node.js popular for backend development?](#q3-why-is-nodejs-popular-for-backend-development)
4. [Q4. What is the V8 engine?](#q4-what-is-the-v8-engine)
5. [Q5. Is Node.js single-threaded?](#q5-is-nodejs-single-threaded)
6. [Q6. What is non-blocking I/O?](#q6-what-is-non-blocking-io)
7. [Q7. What is the difference between synchronous and asynchronous code?](#q7-what-is-the-difference-between-synchronous-and-asynchronous-code)
8. [Q8. What are globals in Node.js?](#q8-what-are-globals-in-nodejs)
9. [Q9. What is process in Node.js?](#q9-what-is-process-in-nodejs)
10. [Q10. What is REPL?](#q10-what-is-repl)
11. [Q11. What is npm?](#q11-what-is-npm)
12. [Q12. What is package.json?](#q12-what-is-packagejson)
13. [Q13. What is package-lock.json?](#q13-what-is-package-lockjson)
14. [Q14. What are dependencies and devDependencies?](#q14-what-are-dependencies-and-devdependencies)
15. [Q15. What is npx?](#q15-what-is-npx)
16. [Q16. What is CommonJS?](#q16-what-is-commonjs)
17. [Q17. What are ES modules in Node.js?](#q17-what-are-es-modules-in-nodejs)
18. [Q18. CommonJS vs ES modules: what is the difference?](#q18-commonjs-vs-es-modules-what-is-the-difference)
19. [Q19. What is module caching?](#q19-what-is-module-caching)
20. [Q20. What is the node: prefix?](#q20-what-is-the-node-prefix)
21. [Q21. What is the fs module?](#q21-what-is-the-fs-module)
22. [Q22. What is the path module?](#q22-what-is-the-path-module)
23. [Q23. What is the os module?](#q23-what-is-the-os-module)
24. [Q24. What is the url module?](#q24-what-is-the-url-module)
25. [Q25. What is Buffer?](#q25-what-is-buffer)
26. [Q26. What is the crypto module?](#q26-what-is-the-crypto-module)
27. [Q27. What is EventEmitter?](#q27-what-is-eventemitter)
28. [Q28. What is an EventEmitter once listener?](#q28-what-is-an-eventemitter-once-listener)
29. [Q29. What is the util module?](#q29-what-is-the-util-module)
30. [Q30. What is __dirname and its ESM alternative?](#q30-what-is-dirname-and-its-esm-alternative)
31. [Q31. What is the Node.js event loop?](#q31-what-is-the-nodejs-event-loop)
32. [Q32. What are the major event loop phases?](#q32-what-are-the-major-event-loop-phases)
33. [Q33. What is the difference between setTimeout and setImmediate?](#q33-what-is-the-difference-between-settimeout-and-setimmediate)
34. [Q34. What is process.nextTick()?](#q34-what-is-processnexttick)
35. [Q35. What are microtasks?](#q35-what-are-microtasks)
36. [Q36. What is callback hell?](#q36-what-is-callback-hell)
37. [Q37. What is a Promise?](#q37-what-is-a-promise)
38. [Q38. What is async/await?](#q38-what-is-asyncawait)
39. [Q39. Promise.all vs Promise.allSettled?](#q39-promiseall-vs-promiseallsettled)
40. [Q40. Promise.race vs Promise.any?](#q40-promiserace-vs-promiseany)
41. [Q41. How do you handle async errors?](#q41-how-do-you-handle-async-errors)
42. [Q42. What is an unhandled promise rejection?](#q42-what-is-an-unhandled-promise-rejection)
43. [Q43. What is the libuv thread pool?](#q43-what-is-the-libuv-thread-pool)
44. [Q44. What does concurrency mean in Node.js?](#q44-what-does-concurrency-mean-in-nodejs)
45. [Q45. How do you avoid blocking the event loop?](#q45-how-do-you-avoid-blocking-the-event-loop)
46. [Q46. What is AbortController used for?](#q46-what-is-abortcontroller-used-for)
47. [Q47. How do you run two independent async tasks together?](#q47-how-do-you-run-two-independent-async-tasks-together)
48. [Q48. What is the difference between I/O-bound and CPU-bound work?](#q48-what-is-the-difference-between-io-bound-and-cpu-bound-work)
49. [Q49. How do you create an HTTP server without Express?](#q49-how-do-you-create-an-http-server-without-express)
50. [Q50. What are req and res?](#q50-what-are-req-and-res)
51. [Q51. What are HTTP methods?](#q51-what-are-http-methods)
52. [Q52. What are common HTTP status codes?](#q52-what-are-common-http-status-codes)
53. [Q53. How do you send a JSON response?](#q53-how-do-you-send-a-json-response)
54. [Q54. How do you read JSON request bodies?](#q54-how-do-you-read-json-request-bodies)
55. [Q55. What is REST API?](#q55-what-is-rest-api)
56. [Q56. What is routing?](#q56-what-is-routing)
57. [Q57. What is middleware?](#q57-what-is-middleware)
58. [Q58. What is CORS?](#q58-what-is-cors)
59. [Q59. What is the difference between authentication and authorisation?](#q59-what-is-the-difference-between-authentication-and-authorisation)
60. [Q60. What is JWT?](#q60-what-is-jwt)
61. [Q61. What is rate limiting?](#q61-what-is-rate-limiting)
62. [Q62. What is pagination?](#q62-what-is-pagination)
63. [Q63. What is WebSocket?](#q63-what-is-websocket)
64. [Q64. What is a stream in Node.js?](#q64-what-is-a-stream-in-nodejs)
65. [Q65. What are the four stream types?](#q65-what-are-the-four-stream-types)
66. [Q66. What is backpressure?](#q66-what-is-backpressure)
67. [Q67. What is pipe()?](#q67-what-is-pipe)
68. [Q68. What is stream.pipeline()?](#q68-what-is-streampipeline)
69. [Q69. How do you handle large file uploads?](#q69-how-do-you-handle-large-file-uploads)
70. [Q70. What is gzip compression?](#q70-what-is-gzip-compression)
71. [Q71. What is memory usage monitoring?](#q71-what-is-memory-usage-monitoring)
72. [Q72. What causes memory leaks in Node.js?](#q72-what-causes-memory-leaks-in-nodejs)
73. [Q73. How do you measure execution time?](#q73-how-do-you-measure-execution-time)
74. [Q74. What is clustering?](#q74-what-is-clustering)
75. [Q75. What are worker threads?](#q75-what-are-worker-threads)
76. [Q76. Worker threads vs child processes?](#q76-worker-threads-vs-child-processes)
77. [Q77. What is horizontal scaling?](#q77-what-is-horizontal-scaling)
78. [Q78. How should you use environment variables?](#q78-how-should-you-use-environment-variables)
79. [Q79. What is SQL injection and how do you prevent it?](#q79-what-is-sql-injection-and-how-do-you-prevent-it)
80. [Q80. What is input validation?](#q80-what-is-input-validation)
81. [Q81. How do you store passwords securely?](#q81-how-do-you-store-passwords-securely)
82. [Q82. What is HTTPS?](#q82-what-is-https)
83. [Q83. What is Helmet in Express?](#q83-what-is-helmet-in-express)
84. [Q84. How do you prevent path traversal?](#q84-how-do-you-prevent-path-traversal)
85. [Q85. What is the built-in Node.js test runner?](#q85-what-is-the-built-in-nodejs-test-runner)
86. [Q86. What is mocking in tests?](#q86-what-is-mocking-in-tests)
87. [Q87. What is integration testing?](#q87-what-is-integration-testing)
88. [Q88. What is logging best practice?](#q88-what-is-logging-best-practice)
89. [Q89. What is graceful shutdown?](#q89-what-is-graceful-shutdown)
90. [Q90. How do you handle uncaught exceptions?](#q90-how-do-you-handle-uncaught-exceptions)
91. [Q91. What is health check vs readiness check?](#q91-what-is-health-check-vs-readiness-check)
92. [Q92. What is a production process manager?](#q92-what-is-a-production-process-manager)
93. [Q93. How do you debug Node.js applications?](#q93-how-do-you-debug-nodejs-applications)
94. [Q94. How do you use Node.js built-in fetch?](#q94-how-do-you-use-nodejs-built-in-fetch)
95. [Q95. What is AsyncLocalStorage?](#q95-what-is-asynclocalstorage)
96. [Q96. What is a zero-downtime deployment strategy?](#q96-what-is-a-zero-downtime-deployment-strategy)
97. [Q97. What is the best way to prepare a Node.js app for production?](#q97-what-is-the-best-way-to-prepare-a-nodejs-app-for-production)
98. [Q98. What is API versioning?](#q98-what-is-api-versioning)
99. [Q99. What are idempotent HTTP requests?](#q99-what-are-idempotent-http-requests)
100. [Q100. How can you avoid duplicate jobs?](#q100-how-can-you-avoid-duplicate-jobs)

</details>

---

## Node.js Fundamentals

[⬆ Back to Table of Contents](#-table-of-contents)

### Q1. What is Node.js?

<a id="q1-what-is-nodejs"></a>

**✅ Easy Answer:** Node.js is a JavaScript runtime built on the V8 engine. We can run JavaScript outside the browser, mainly for servers, scripts and tools.

**💻 Example:**

```javascript
console.log('Hello from Node.js');
```

**🎯 Interview Tip:** Node.js is a runtime, not a programming language or framework.

---

### Q2. How is Node.js different from JavaScript?

<a id="q2-how-is-nodejs-different-from-javascript"></a>

**✅ Easy Answer:** JavaScript is the language. Node.js is one environment that runs it and provides server-side APIs such as file system and networking.

**💻 Example:**

```javascript
const os = require('node:os');
console.log(os.platform());
```

**🎯 Interview Tip:** Browser APIs like document are not available in a normal Node.js process.

---

### Q3. Why is Node.js popular for backend development?

<a id="q3-why-is-nodejs-popular-for-backend-development"></a>

**✅ Easy Answer:** It handles many I/O requests efficiently using non-blocking APIs, and teams can use JavaScript on both frontend and backend.

**💻 Example:**

```javascript
const http = require('node:http');
http.createServer((req, res) => res.end('Hi')).listen(3000);
```

**🎯 Interview Tip:** CPU-heavy synchronous code can still block request handling.

---

### Q4. What is the V8 engine?

<a id="q4-what-is-the-v8-engine"></a>

**✅ Easy Answer:** V8 executes JavaScript and uses just-in-time compilation. Node.js uses V8 along with its own runtime APIs.

**💻 Example:**

```javascript
console.log(process.versions.v8);
```

**🎯 Interview Tip:** V8 is not the event loop.

---

### Q5. Is Node.js single-threaded?

<a id="q5-is-nodejs-single-threaded"></a>

**✅ Easy Answer:** JavaScript callbacks normally execute on one main thread per Node.js isolate, but Node.js also uses OS facilities and worker threads for background work.

**💻 Example:**

```javascript
console.log('PID:', process.pid);
```

**🎯 Interview Tip:** Never say the entire runtime uses only one thread.

---

### Q6. What is non-blocking I/O?

<a id="q6-what-is-non-blocking-io"></a>

**✅ Easy Answer:** Node.js starts an I/O operation and can continue doing other work instead of waiting for it to finish.

**💻 Example:**

```javascript
const fs = require('node:fs');
fs.readFile('package.json', 'utf8', (err, data) => {
  if (err) return console.error(err);
  console.log(data.length);
});
console.log('This can print first');
```

**🎯 Interview Tip:** Use asynchronous APIs for operations that may take time.

---

### Q7. What is the difference between synchronous and asynchronous code?

<a id="q7-what-is-the-difference-between-synchronous-and-asynchronous-code"></a>

**✅ Easy Answer:** Synchronous code runs in sequence and can block. Asynchronous operations allow completion to be handled later.

**💻 Example:**

```javascript
const fs = require('node:fs');
const text = fs.readFileSync('package.json', 'utf8');
console.log(text.length);
```

**🎯 Interview Tip:** Sync APIs are fine for small startup scripts, but avoid them on busy request paths.

---

### Q8. What are globals in Node.js?

<a id="q8-what-are-globals-in-nodejs"></a>

**✅ Easy Answer:** Common globals include `process`, `Buffer`, `console`, timers and `globalThis`. Some CommonJS names are module-scoped, not truly global.

**💻 Example:**

```javascript
console.log(typeof process);
console.log(globalThis === global);
```

**🎯 Interview Tip:** `__dirname` is available in CommonJS, not directly in ES modules.

---

### Q9. What is process in Node.js?

<a id="q9-what-is-process-in-nodejs"></a>

**✅ Easy Answer:** `process` provides information and control for the running Node.js process, including environment variables and exit events.

**💻 Example:**

```javascript
console.log(process.pid);
console.log(process.env.NODE_ENV ?? 'development');
```

**🎯 Interview Tip:** Avoid printing secrets from `process.env`.

---

### Q10. What is REPL?

<a id="q10-what-is-repl"></a>

**✅ Easy Answer:** REPL means Read-Eval-Print Loop. It lets us test small JavaScript expressions interactively.

**💻 Example:**

```javascript
// In terminal, run: node
// Then type: 2 + 3
// Output: 5
```

**🎯 Interview Tip:** Use `.exit` or Ctrl+D to leave the REPL.

---

### Q11. What is npm?

<a id="q11-what-is-npm"></a>

**✅ Easy Answer:** npm is the package manager commonly used with Node.js to install dependencies and run project scripts.

**💻 Example:**

```javascript
// Terminal:
// npm init -y
// npm install express
```

**🎯 Interview Tip:** Prefer project-local dependencies.

---

### Q12. What is package.json?

<a id="q12-what-is-packagejson"></a>

**✅ Easy Answer:** It stores project metadata, scripts, dependency ranges and configuration.

**💻 Example:**

```javascript
{
  "scripts": { "start": "node server.js" },
  "dependencies": {}
}
```

**🎯 Interview Tip:** The sample is JSON, not code to paste into a `.js` file.

---

### Q13. What is package-lock.json?

<a id="q13-what-is-package-lockjson"></a>

**✅ Easy Answer:** It records an exact resolved dependency tree to help make installs repeatable.

**💻 Example:**

```javascript
// Terminal:
// npm ci
```

**🎯 Interview Tip:** Commit the lockfile for applications and CI pipelines.

---

### Q14. What are dependencies and devDependencies?

<a id="q14-what-are-dependencies-and-devdependencies"></a>

**✅ Easy Answer:** `dependencies` are needed by the application in production. `devDependencies` are mainly used for development, testing or building.

**💻 Example:**

```javascript
// Terminal:
// npm install express
// npm install -D eslint
```

**🎯 Interview Tip:** Build tooling can be a devDependency even if CI uses it.

---

### Q15. What is npx?

<a id="q15-what-is-npx"></a>

**✅ Easy Answer:** `npx` runs package-provided commands, often without creating a global installation.

**💻 Example:**

```javascript
// Terminal:
// npx eslint --version
```

**🎯 Interview Tip:** Check which package you are executing before running unfamiliar commands.

---

## Modules & Core APIs

[⬆ Back to Table of Contents](#-table-of-contents)

### Q16. What is CommonJS?

<a id="q16-what-is-commonjs"></a>

**✅ Easy Answer:** CommonJS is the traditional Node.js module format that uses `require` and `module.exports`.

**💻 Example:**

```javascript
// math.cjs
module.exports.add = (a, b) => a + b;
// app.cjs
const { add } = require('./math.cjs');
console.log(add(2, 3));
```

**🎯 Interview Tip:** A `require` example may use `.cjs` explicitly.

---

### Q17. What are ES modules in Node.js?

<a id="q17-what-are-es-modules-in-nodejs"></a>

**✅ Easy Answer:** ES modules use standard `import` and `export`. Use `.mjs` or set `"type": "module"` in package.json.

**💻 Example:**

```javascript
// math.mjs
export const add = (a, b) => a + b;
// app.mjs
import { add } from './math.mjs';
console.log(add(2, 3));
```

**🎯 Interview Tip:** Include extensions for relative ESM imports.

---

### Q18. CommonJS vs ES modules: what is the difference?

<a id="q18-commonjs-vs-es-modules-what-is-the-difference"></a>

**✅ Easy Answer:** CommonJS commonly uses `require` and exports; ESM uses `import` and `export` with statically analysable module syntax.

**💻 Example:**

```javascript
// CommonJS: const fs = require('node:fs');
// ESM: import fs from 'node:fs';
```

**🎯 Interview Tip:** Module interop has rules; do not assume every import works identically.

---

### Q19. What is module caching?

<a id="q19-what-is-module-caching"></a>

**✅ Easy Answer:** After loading a CommonJS module, Node.js normally reuses its cached export for the same resolved filename.

**💻 Example:**

```javascript
const a = require('node:os');
const b = require('node:os');
console.log(a === b); // true
```

**🎯 Interview Tip:** Caching behaviour for ESM is managed separately.

---

### Q20. What is the node: prefix?

<a id="q20-what-is-the-node-prefix"></a>

**✅ Easy Answer:** It explicitly identifies a Node.js built-in module and helps avoid confusion with user packages.

**💻 Example:**

```javascript
const fs = require('node:fs');
const path = require('node:path');
console.log(path.basename('/tmp/a.txt'));
```

**🎯 Interview Tip:** Prefer `node:` for built-in imports.

---

### Q21. What is the fs module?

<a id="q21-what-is-the-fs-module"></a>

**✅ Easy Answer:** `node:fs` provides file and directory operations such as reading, writing and listing files.

**💻 Example:**

```javascript
const fs = require('node:fs/promises');
async function run() {
  await fs.writeFile('demo.txt', 'Hello');
  console.log(await fs.readFile('demo.txt', 'utf8'));
}
run().catch(console.error);
```

**🎯 Interview Tip:** Use `node:fs/promises` with async/await.

---

### Q22. What is the path module?

<a id="q22-what-is-the-path-module"></a>

**✅ Easy Answer:** `node:path` safely builds, normalises and inspects filesystem paths.

**💻 Example:**

```javascript
const path = require('node:path');
console.log(path.join('uploads', 'photo.png'));
```

**🎯 Interview Tip:** Do not use `path.join` alone to authorise user-controlled paths.

---

### Q23. What is the os module?

<a id="q23-what-is-the-os-module"></a>

**✅ Easy Answer:** `node:os` provides system information such as platform, CPU details and temporary directory.

**💻 Example:**

```javascript
const os = require('node:os');
console.log(os.platform(), os.tmpdir());
```

**🎯 Interview Tip:** System information is not a substitute for runtime health metrics.

---

### Q24. What is the url module?

<a id="q24-what-is-the-url-module"></a>

**✅ Easy Answer:** The standard `URL` API parses and builds URLs safely.

**💻 Example:**

```javascript
const url = new URL('https://example.com/?page=2');
console.log(url.searchParams.get('page'));
```

**🎯 Interview Tip:** Prefer `URL` over manual string splitting.

---

### Q25. What is Buffer?

<a id="q25-what-is-buffer"></a>

**✅ Easy Answer:** Buffer represents a sequence of bytes and is useful for binary files, networking and encodings.

**💻 Example:**

```javascript
const data = Buffer.from('Hi', 'utf8');
console.log(data.toString('hex')); // 4869
```

**🎯 Interview Tip:** Bytes and JavaScript characters are not always one-to-one.

---

### Q26. What is the crypto module?

<a id="q26-what-is-the-crypto-module"></a>

**✅ Easy Answer:** `node:crypto` provides primitives for hashing, signing, encryption and secure random data.

**💻 Example:**

```javascript
const { randomUUID } = require('node:crypto');
console.log(randomUUID());
```

**🎯 Interview Tip:** Never invent your own cryptography; password hashing requires a dedicated password-hashing algorithm.

---

### Q27. What is EventEmitter?

<a id="q27-what-is-eventemitter"></a>

**✅ Easy Answer:** `EventEmitter` provides an event-based API where listeners respond when events are emitted.

**💻 Example:**

```javascript
const { EventEmitter } = require('node:events');
const bus = new EventEmitter();
bus.on('ready', name => console.log('Hello', name));
bus.emit('ready', 'Jamshed');
```

**🎯 Interview Tip:** Remove listeners when they are no longer required.

---

### Q28. What is an EventEmitter once listener?

<a id="q28-what-is-an-eventemitter-once-listener"></a>

**✅ Easy Answer:** `once` registers a handler that automatically removes itself after the first matching event.

**💻 Example:**

```javascript
const { EventEmitter } = require('node:events');
const bus = new EventEmitter();
bus.once('done', () => console.log('Only once'));
bus.emit('done');
bus.emit('done');
```

**🎯 Interview Tip:** An unhandled `error` event on EventEmitter can throw.

---

### Q29. What is the util module?

<a id="q29-what-is-the-util-module"></a>

**✅ Easy Answer:** `node:util` exposes useful helpers such as promisify and inspect.

**💻 Example:**

```javascript
const { promisify } = require('node:util');
const fs = require('node:fs');
const readFile = promisify(fs.readFile);
readFile('package.json', 'utf8').then(console.log);
```

**🎯 Interview Tip:** Where possible, prefer built-in promise APIs directly.

---

### Q30. What is __dirname and its ESM alternative?

<a id="q30-what-is-dirname-and-its-esm-alternative"></a>

**✅ Easy Answer:** `__dirname` is the current module directory in CommonJS. ES modules can derive a path from `import.meta.url`.

**💻 Example:**

```javascript
// In an ES module (.mjs):
import { fileURLToPath } from 'node:url';
import { dirname } from 'node:path';
const here = dirname(fileURLToPath(import.meta.url));
console.log(here);
```

**🎯 Interview Tip:** `process.cwd()` means working directory and can differ from module directory.

---

## Async Programming & Event Loop

[⬆ Back to Table of Contents](#-table-of-contents)

### Q31. What is the Node.js event loop?

<a id="q31-what-is-the-nodejs-event-loop"></a>

**✅ Easy Answer:** The event loop coordinates when ready callbacks are run after the current JavaScript work completes.

**💻 Example:**

```javascript
console.log('A');
setTimeout(() => console.log('C'), 0);
console.log('B'); // A, B, C
```

**🎯 Interview Tip:** Timers are not guaranteed to execute at an exact millisecond.

---

### Q32. What are the major event loop phases?

<a id="q32-what-are-the-major-event-loop-phases"></a>

**✅ Easy Answer:** Important phases include timers, pending callbacks, poll, check and close callbacks. Node processes microtasks around callback execution.

**💻 Example:**

```javascript
setImmediate(() => console.log('check'));
setTimeout(() => console.log('timer'), 0);
```

**🎯 Interview Tip:** At top level, timer versus immediate order is not guaranteed.

---

### Q33. What is the difference between setTimeout and setImmediate?

<a id="q33-what-is-the-difference-between-settimeout-and-setimmediate"></a>

**✅ Easy Answer:** `setTimeout` schedules after a minimum delay; `setImmediate` schedules in the check phase. Their order depends on context.

**💻 Example:**

```javascript
const fs = require('node:fs');
fs.readFile(__filename, () => {
  setImmediate(() => console.log('immediate'));
  setTimeout(() => console.log('timeout'), 0);
});
```

**🎯 Interview Tip:** Inside an I/O callback, `setImmediate` typically runs first.

---

### Q34. What is process.nextTick()?

<a id="q34-what-is-processnexttick"></a>

**✅ Easy Answer:** It puts a callback in the next-tick queue, which Node drains before progressing to more event-loop work.

**💻 Example:**

```javascript
console.log('start');
process.nextTick(() => console.log('tick'));
console.log('end');
```

**🎯 Interview Tip:** Recursive nextTick scheduling can starve the event loop.

---

### Q35. What are microtasks?

<a id="q35-what-are-microtasks"></a>

**✅ Easy Answer:** Promise handlers and `queueMicrotask` callbacks run as microtasks after the current synchronous work.

**💻 Example:**

```javascript
console.log(1);
queueMicrotask(() => console.log(3));
console.log(2);
```

**🎯 Interview Tip:** Node also has its own next-tick queue.

---

### Q36. What is callback hell?

<a id="q36-what-is-callback-hell"></a>

**✅ Easy Answer:** Callback hell means deeply nested callbacks that are difficult to read, test and handle errors in.

**💻 Example:**

```javascript
const fs = require('node:fs/promises');
async function show() {
  const text = await fs.readFile('package.json', 'utf8');
  console.log(JSON.parse(text).name);
}
show().catch(console.error);
```

**🎯 Interview Tip:** Refactor nested callbacks into named functions or promises.

---

### Q37. What is a Promise?

<a id="q37-what-is-a-promise"></a>

**✅ Easy Answer:** A Promise represents a future completion or failure of an asynchronous operation.

**💻 Example:**

```javascript
const p = Promise.resolve(10);
p.then(value => console.log(value));
```

**🎯 Interview Tip:** A promise does not automatically create a separate thread.

---

### Q38. What is async/await?

<a id="q38-what-is-asyncawait"></a>

**✅ Easy Answer:** `async` functions return promises. `await` pauses that function until a promise settles, without blocking the whole event loop.

**💻 Example:**

```javascript
async function getNumber() {
  return await Promise.resolve(42);
}
getNumber().then(console.log);
```

**🎯 Interview Tip:** Use try/catch around awaited work that might reject.

---

### Q39. Promise.all vs Promise.allSettled?

<a id="q39-promiseall-vs-promiseallsettled"></a>

**✅ Easy Answer:** `Promise.all` rejects when one input rejects. `allSettled` waits for every input and reports each outcome.

**💻 Example:**

```javascript
const tasks = [Promise.resolve(1), Promise.reject('fail')];
Promise.allSettled(tasks).then(console.log);
```

**🎯 Interview Tip:** Use allSettled for independent batch operations where failures should be reported.

---

### Q40. Promise.race vs Promise.any?

<a id="q40-promiserace-vs-promiseany"></a>

**✅ Easy Answer:** `race` settles on the first settled input. `any` fulfills on the first fulfilled input and rejects only if all reject.

**💻 Example:**

```javascript
Promise.any([Promise.reject('x'), Promise.resolve('ok')])
  .then(console.log);
```

**🎯 Interview Tip:** `Promise.any` rejects with AggregateError when all promises reject.

---

### Q41. How do you handle async errors?

<a id="q41-how-do-you-handle-async-errors"></a>

**✅ Easy Answer:** Use try/catch around awaited operations or `.catch()` on promises. Handle errors at your API boundary.

**💻 Example:**

```javascript
const fs = require('node:fs/promises');
async function main() {
  try { await fs.readFile('missing.txt'); }
  catch (err) { console.error(err.code); }
}
main();
```

**🎯 Interview Tip:** Do not silently swallow errors.

---

### Q42. What is an unhandled promise rejection?

<a id="q42-what-is-an-unhandled-promise-rejection"></a>

**✅ Easy Answer:** A rejection is unhandled when no rejection handler is attached in time. It can result in process failure depending on configuration.

**💻 Example:**

```javascript
Promise.reject(new Error('Oops')).catch(console.error);
```

**🎯 Interview Tip:** Attach error handling rather than relying on global handlers.

---

### Q43. What is the libuv thread pool?

<a id="q43-what-is-the-libuv-thread-pool"></a>

**✅ Easy Answer:** libuv provides a pool used by certain operations such as some filesystem, DNS and crypto tasks.

**💻 Example:**

```javascript
const { pbkdf2 } = require('node:crypto');
pbkdf2('password', 'salt', 1000, 32, 'sha256', (err, key) => {
  if (err) return console.error(err);
  console.log(key.length);
});
```

**🎯 Interview Tip:** Not every network request runs inside the thread pool.

---

### Q44. What does concurrency mean in Node.js?

<a id="q44-what-does-concurrency-mean-in-nodejs"></a>

**✅ Easy Answer:** Concurrency means making progress on multiple tasks during overlapping time, often by waiting asynchronously for I/O.

**💻 Example:**

```javascript
async function main() {
  await Promise.all([
    new Promise(r => setTimeout(r, 100)),
    new Promise(r => setTimeout(r, 100))
  ]);
  console.log('Both finished');
}
main();
```

**🎯 Interview Tip:** Concurrency does not always imply parallel CPU execution.

---

### Q45. How do you avoid blocking the event loop?

<a id="q45-how-do-you-avoid-blocking-the-event-loop"></a>

**✅ Easy Answer:** Avoid long synchronous loops and sync I/O in request handlers. Use async I/O, chunk work, or worker threads.

**💻 Example:**

```javascript
setTimeout(() => console.log('Still responsive'), 0);
// Avoid a huge synchronous while loop here.
```

**🎯 Interview Tip:** Move CPU-intensive work into workers or separate services.

---

### Q46. What is AbortController used for?

<a id="q46-what-is-abortcontroller-used-for"></a>

**✅ Easy Answer:** It allows cancellation requests for supported asynchronous operations, including fetch.

**💻 Example:**

```javascript
const controller = new AbortController();
setTimeout(() => controller.abort(), 100);
fetch('https://example.com', { signal: controller.signal })
  .catch(err => console.log(err.name));
```

**🎯 Interview Tip:** Cancellation is cooperative; check API support.

---

### Q47. How do you run two independent async tasks together?

<a id="q47-how-do-you-run-two-independent-async-tasks-together"></a>

**✅ Easy Answer:** Start both promises first and await their combined result with Promise.all.

**💻 Example:**

```javascript
async function main() {
  const [a, b] = await Promise.all([
    Promise.resolve('users'),
    Promise.resolve('orders')
  ]);
  console.log(a, b);
}
main();
```

**🎯 Interview Tip:** Do not parallelise tasks that depend on each other.

---

### Q48. What is the difference between I/O-bound and CPU-bound work?

<a id="q48-what-is-the-difference-between-io-bound-and-cpu-bound-work"></a>

**✅ Easy Answer:** I/O-bound tasks wait on disks or networks; CPU-bound tasks spend time calculating. Each needs a different performance approach.

**💻 Example:**

```javascript
const start = performance.now();
let total = 0;
for (let i = 0; i < 100_000; i++) total += i;
console.log(total, performance.now() - start);
```

**🎯 Interview Tip:** Workers help CPU-heavy tasks, whereas async I/O helps waiting workloads.

---

## HTTP, APIs & Networking

[⬆ Back to Table of Contents](#-table-of-contents)

### Q49. How do you create an HTTP server without Express?

<a id="q49-how-do-you-create-an-http-server-without-express"></a>

**✅ Easy Answer:** Use the built-in `node:http` module and respond to incoming requests.

**💻 Example:**

```javascript
const http = require('node:http');
http.createServer((req, res) => {
  res.writeHead(200, { 'Content-Type': 'text/plain' });
  res.end('Hello Node.js');
}).listen(3000);
```

**🎯 Interview Tip:** Open http://localhost:3000 after starting the script.

---

### Q50. What are req and res?

<a id="q50-what-are-req-and-res"></a>

**✅ Easy Answer:** `req` describes the incoming HTTP request. `res` is used to write headers, status and response body.

**💻 Example:**

```javascript
const http = require('node:http');
http.createServer((req, res) => {
  res.statusCode = 200;
  res.end(req.method + ' ' + req.url);
}).listen(3000);
```

**🎯 Interview Tip:** A response should end exactly once.

---

### Q51. What are HTTP methods?

<a id="q51-what-are-http-methods"></a>

**✅ Easy Answer:** Methods express the intended action: GET reads, POST submits, PUT replaces, PATCH partially updates and DELETE removes.

**💻 Example:**

```javascript
const method = 'PATCH';
console.log(['GET','POST','PUT','PATCH','DELETE'].includes(method));
```

**🎯 Interview Tip:** Methods have semantics; do not use GET for actions that mutate data.

---

### Q52. What are common HTTP status codes?

<a id="q52-what-are-common-http-status-codes"></a>

**✅ Easy Answer:** 200 means OK, 201 created, 400 bad request, 401 unauthenticated, 403 forbidden, 404 missing and 500 server error.

**💻 Example:**

```javascript
const codes = { ok: 200, created: 201, badRequest: 400, notFound: 404 };
console.log(codes.notFound);
```

**🎯 Interview Tip:** Use status codes that match what actually happened.

---

### Q53. How do you send a JSON response?

<a id="q53-how-do-you-send-a-json-response"></a>

**✅ Easy Answer:** Set `Content-Type: application/json` and serialise an object.

**💻 Example:**

```javascript
const http = require('node:http');
http.createServer((req, res) => {
  res.writeHead(200, { 'Content-Type': 'application/json' });
  res.end(JSON.stringify({ message: 'Success' }));
}).listen(3000);
```

**🎯 Interview Tip:** Do not leak database fields or secrets automatically.

---

### Q54. How do you read JSON request bodies?

<a id="q54-how-do-you-read-json-request-bodies"></a>

**✅ Easy Answer:** Collect incoming data with a size limit, then parse JSON safely. In production, use robust body parsing middleware.

**💻 Example:**

```javascript
const http = require('node:http');
http.createServer(async (req, res) => {
  try {
    let body = '';
    for await (const chunk of req) {
      body += chunk;
      if (body.length > 10_000) throw new Error('Too large');
    }
    const data = JSON.parse(body || '{}');
    res.end(JSON.stringify(data));
  } catch { res.writeHead(400); res.end('Invalid body'); }
}).listen(3000);
```

**🎯 Interview Tip:** Production byte limits should count bytes, not JavaScript string length.

---

### Q55. What is REST API?

<a id="q55-what-is-rest-api"></a>

**✅ Easy Answer:** REST is an architectural style for resource-based APIs. HTTP URLs, methods and representations help clients interact with resources.

**💻 Example:**

```javascript
// Example routes:
// GET /users
// GET /users/42
// POST /users
// DELETE /users/42
```

**🎯 Interview Tip:** REST is more than just naming endpoints.

---

### Q56. What is routing?

<a id="q56-what-is-routing"></a>

**✅ Easy Answer:** Routing selects the handler for a request based on path and HTTP method.

**💻 Example:**

```javascript
const http = require('node:http');
http.createServer((req, res) => {
  if (req.method === 'GET' && req.url === '/health')
    return res.end('OK');
  res.writeHead(404); res.end('Not found');
}).listen(3000);
```

**🎯 Interview Tip:** Parse URLs properly when query strings are involved.

---

### Q57. What is middleware?

<a id="q57-what-is-middleware"></a>

**✅ Easy Answer:** Middleware is a function in frameworks such as Express that can inspect or modify requests and pass control to the next handler.

**💻 Example:**

```javascript
// Requires: npm install express
const express = require('express');
const app = express();
app.use((req, res, next) => {
  console.log(req.method);
  next();
});
```

**🎯 Interview Tip:** Middleware belongs to a framework pattern, not the HTTP core module itself.

---

### Q58. What is CORS?

<a id="q58-what-is-cors"></a>

**✅ Easy Answer:** Cross-Origin Resource Sharing is a browser-enforced mechanism where servers allow selected origins through HTTP headers.

**💻 Example:**

```javascript
// Example Express middleware (npm install cors):
const cors = require('cors');
app.use(cors({ origin: 'https://myapp.example' }));
```

**🎯 Interview Tip:** `app` refers to an Express instance declared earlier; CORS is not authentication.

---

### Q59. What is the difference between authentication and authorisation?

<a id="q59-what-is-the-difference-between-authentication-and-authorisation"></a>

**✅ Easy Answer:** Authentication checks who the user is. Authorisation checks whether that user may perform an action.

**💻 Example:**

```javascript
function canEdit(user, ownerId) {
  return user?.id === ownerId;
}
console.log(canEdit({ id: 4 }, 4));
```

**🎯 Interview Tip:** Always check authorisation on the server.

---

### Q60. What is JWT?

<a id="q60-what-is-jwt"></a>

**✅ Easy Answer:** A JSON Web Token is a compact token format containing claims that can be signed or encrypted. APIs commonly validate signed JWTs for authentication.

**💻 Example:**

```javascript
// Example payload only, not a signed token:
const claims = { sub: 'user-42', role: 'reader' };
console.log(claims.sub);
```

**🎯 Interview Tip:** Do not trust decoded claims before validating signature, algorithm and expiry.

---

### Q61. What is rate limiting?

<a id="q61-what-is-rate-limiting"></a>

**✅ Easy Answer:** Rate limiting restricts how frequently a client can call an endpoint to reduce abuse and resource exhaustion.

**💻 Example:**

```javascript
// Express example after installing express-rate-limit:
const { rateLimit } = require('express-rate-limit');
const limiter = rateLimit({ windowMs: 60_000, limit: 60 });
app.use('/api', limiter);
```

**🎯 Interview Tip:** For multi-instance production setups, use a shared store when needed.

---

### Q62. What is pagination?

<a id="q62-what-is-pagination"></a>

**✅ Easy Answer:** Pagination returns a manageable subset of a large dataset using page/limit or cursor-based approaches.

**💻 Example:**

```javascript
const users = ['A', 'B', 'C', 'D'];
const page = 2, limit = 2;
console.log(users.slice((page - 1) * limit, page * limit));
```

**🎯 Interview Tip:** Validate limits to prevent very expensive requests.

---

### Q63. What is WebSocket?

<a id="q63-what-is-websocket"></a>

**✅ Easy Answer:** WebSocket creates a persistent full-duplex connection for real-time communication between client and server.

**💻 Example:**

```javascript
// With npm install ws:
const { WebSocketServer } = require('ws');
const wss = new WebSocketServer({ port: 8080 });
wss.on('connection', socket => socket.send('Connected'));
```

**🎯 Interview Tip:** For large-scale deployment, consider heartbeat, auth and backpressure.

---

## Streams, Files & Performance

[⬆ Back to Table of Contents](#-table-of-contents)

### Q64. What is a stream in Node.js?

<a id="q64-what-is-a-stream-in-nodejs"></a>

**✅ Easy Answer:** A stream processes data in chunks instead of waiting for the entire content at once.

**💻 Example:**

```javascript
const fs = require('node:fs');
const stream = fs.createReadStream('package.json');
stream.on('data', chunk => console.log(chunk.length));
stream.on('error', console.error);
```

**🎯 Interview Tip:** Streams are useful for large files and network responses.

---

### Q65. What are the four stream types?

<a id="q65-what-are-the-four-stream-types"></a>

**✅ Easy Answer:** Readable produces data, Writable consumes data, Duplex does both, and Transform changes data while streaming.

**💻 Example:**

```javascript
const { Readable } = require('node:stream');
Readable.from(['Hello', ' Node']).on('data', c => console.log(c.toString()));
```

**🎯 Interview Tip:** Transform is a special kind of Duplex stream.

---

### Q66. What is backpressure?

<a id="q66-what-is-backpressure"></a>

**✅ Easy Answer:** Backpressure means producers slow down when consumers cannot process data quickly enough.

**💻 Example:**

```javascript
const { Writable } = require('node:stream');
const out = new Writable({
  write(chunk, enc, cb) { setTimeout(cb, 10); }
});
console.log(out.write('data'));
out.end();
```

**🎯 Interview Tip:** Respect the boolean returned by writable.write and wait for drain if false.

---

### Q67. What is pipe()?

<a id="q67-what-is-pipe"></a>

**✅ Easy Answer:** `pipe` connects a readable stream to a writable stream and manages basic flow control.

**💻 Example:**

```javascript
const fs = require('node:fs');
const source = fs.createReadStream('package.json');
const target = fs.createWriteStream('copy.json');
source.pipe(target);
source.on('error', console.error);
target.on('error', console.error);
```

**🎯 Interview Tip:** For robust error propagation prefer `pipeline`.

---

### Q68. What is stream.pipeline()?

<a id="q68-what-is-streampipeline"></a>

**✅ Easy Answer:** `pipeline` connects streams and handles many cleanup and error cases automatically.

**💻 Example:**

```javascript
const { pipeline } = require('node:stream/promises');
const fs = require('node:fs');
async function main() {
  await pipeline(fs.createReadStream('package.json'),
                 fs.createWriteStream('backup.json'));
}
main().catch(console.error);
```

**🎯 Interview Tip:** Promise-based pipeline is convenient with async/await.

---

### Q69. How do you handle large file uploads?

<a id="q69-how-do-you-handle-large-file-uploads"></a>

**✅ Easy Answer:** Stream uploads to controlled storage and enforce size, type and access limits.

**💻 Example:**

```javascript
// Minimal stream example (not a production upload endpoint):
const fs = require('node:fs');
const source = fs.createReadStream('large-file.bin');
source.pipe(fs.createWriteStream('copy.bin'));
```

**🎯 Interview Tip:** Never trust client-supplied filenames or MIME types.

---

### Q70. What is gzip compression?

<a id="q70-what-is-gzip-compression"></a>

**✅ Easy Answer:** Gzip reduces the bytes of compressible response or file data at the cost of CPU.

**💻 Example:**

```javascript
const { gzipSync } = require('node:zlib');
const zipped = gzipSync(Buffer.from('hello hello hello'));
console.log(zipped.length);
```

**🎯 Interview Tip:** Avoid compressing already-compressed formats without measurement.

---

### Q71. What is memory usage monitoring?

<a id="q71-what-is-memory-usage-monitoring"></a>

**✅ Easy Answer:** `process.memoryUsage()` reports memory metrics such as rss and heapUsed.

**💻 Example:**

```javascript
const mem = process.memoryUsage();
console.log(Math.round(mem.heapUsed / 1024 / 1024), 'MB');
```

**🎯 Interview Tip:** Monitor trends and workload, not a single number.

---

### Q72. What causes memory leaks in Node.js?

<a id="q72-what-causes-memory-leaks-in-nodejs"></a>

**✅ Easy Answer:** Typical causes include unbounded caches, forgotten timers or listeners, and objects retained in closures.

**💻 Example:**

```javascript
const cache = new Map();
cache.set('user:1', { name: 'A' });
cache.delete('user:1'); // release when no longer needed
```

**🎯 Interview Tip:** Use bounded caching and heap profiling.

---

### Q73. How do you measure execution time?

<a id="q73-how-do-you-measure-execution-time"></a>

**✅ Easy Answer:** Use `performance.now()` for elapsed timing or `console.time()` for quick investigation.

**💻 Example:**

```javascript
console.time('work');
let sum = 0;
for (let i = 0; i < 1000; i++) sum += i;
console.timeEnd('work');
```

**🎯 Interview Tip:** Benchmark realistic workloads and repeat tests.

---

### Q74. What is clustering?

<a id="q74-what-is-clustering"></a>

**✅ Easy Answer:** The cluster module can create multiple Node.js worker processes to use multiple CPU cores for server workloads.

**💻 Example:**

```javascript
const cluster = require('node:cluster');
console.log(cluster.isPrimary ? 'Primary process' : 'Worker process');
```

**🎯 Interview Tip:** This demonstrates role detection; a complete cluster needs fork and lifecycle management.

---

### Q75. What are worker threads?

<a id="q75-what-are-worker-threads"></a>

**✅ Easy Answer:** Worker threads run JavaScript in separate threads and are helpful for CPU-intensive calculations.

**💻 Example:**

```javascript
const { Worker, isMainThread, parentPort } = require('node:worker_threads');
if (isMainThread) {
  new Worker(__filename).on('message', console.log);
} else {
  parentPort.postMessage(2 + 2);
}
```

**🎯 Interview Tip:** Save as a CommonJS file and run with Node.js; workers are not needed for ordinary async I/O.

---

### Q76. Worker threads vs child processes?

<a id="q76-worker-threads-vs-child-processes"></a>

**✅ Easy Answer:** Workers share a process but have separate JS execution contexts; child processes run independently with process isolation.

**💻 Example:**

```javascript
const { spawn } = require('node:child_process');
const child = spawn(process.execPath, ['--version']);
child.stdout.on('data', data => console.log(data.toString()));
```

**🎯 Interview Tip:** Prefer spawn with explicit arguments rather than building shell commands from input.

---

### Q77. What is horizontal scaling?

<a id="q77-what-is-horizontal-scaling"></a>

**✅ Easy Answer:** Horizontal scaling runs more application instances behind a load balancer to handle more traffic.

**💻 Example:**

```javascript
// Example health endpoint used by a load balancer:
const http = require('node:http');
http.createServer((req, res) => res.end('healthy')).listen(3000);
```

**🎯 Interview Tip:** Keep shared state outside individual instances when necessary.

---

## Security, Testing & Production

[⬆ Back to Table of Contents](#-table-of-contents)

### Q78. How should you use environment variables?

<a id="q78-how-should-you-use-environment-variables"></a>

**✅ Easy Answer:** Store environment-specific configuration in environment variables, validate required values and keep secrets out of source control.

**💻 Example:**

```javascript
const port = Number(process.env.PORT ?? 3000);
if (!Number.isInteger(port) || port < 1 || port > 65535)
  throw new Error('Invalid PORT');
console.log(port);
```

**🎯 Interview Tip:** Never commit real `.env` secrets.

---

### Q79. What is SQL injection and how do you prevent it?

<a id="q79-what-is-sql-injection-and-how-do-you-prevent-it"></a>

**✅ Easy Answer:** SQL injection happens when untrusted input changes query syntax. Use parameterised queries instead of string concatenation.

**💻 Example:**

```javascript
// Example with a PostgreSQL client named db:
// await db.query('SELECT * FROM users WHERE id = $1', [userId]);
```

**🎯 Interview Tip:** This is a conceptual query example; `db` must be initialised separately.

---

### Q80. What is input validation?

<a id="q80-what-is-input-validation"></a>

**✅ Easy Answer:** Input validation checks that data has the expected type, size and format before business logic uses it.

**💻 Example:**

```javascript
function validateAge(age) {
  if (!Number.isInteger(age) || age < 0 || age > 120)
    throw new Error('Invalid age');
  return age;
}
console.log(validateAge(25));
```

**🎯 Interview Tip:** Validation and output encoding solve different problems.

---

### Q81. How do you store passwords securely?

<a id="q81-how-do-you-store-passwords-securely"></a>

**✅ Easy Answer:** Store a salted password hash using a password-specific algorithm like Argon2id or scrypt, never plaintext passwords.

**💻 Example:**

```javascript
const { scryptSync, randomBytes } = require('node:crypto');
const salt = randomBytes(16);
const hash = scryptSync('demo-password', salt, 64);
console.log({ salt: salt.toString('hex'), hash: hash.toString('hex') });
```

**🎯 Interview Tip:** Production code should use a vetted password library or carefully designed async hashing and safe verification.

---

### Q82. What is HTTPS?

<a id="q82-what-is-https"></a>

**✅ Easy Answer:** HTTPS sends HTTP over TLS to protect data in transit and authenticate the server.

**💻 Example:**

```javascript
const https = require('node:https');
https.get('https://example.com', res => {
  console.log(res.statusCode);
  res.resume();
}).on('error', console.error);
```

**🎯 Interview Tip:** Use valid certificates and modern TLS settings.

---

### Q83. What is Helmet in Express?

<a id="q83-what-is-helmet-in-express"></a>

**✅ Easy Answer:** Helmet is Express middleware that sets several security-related HTTP response headers.

**💻 Example:**

```javascript
// npm install express helmet
const express = require('express');
const helmet = require('helmet');
const app = express();
app.use(helmet());
```

**🎯 Interview Tip:** Security headers are only one part of application security.

---

### Q84. How do you prevent path traversal?

<a id="q84-how-do-you-prevent-path-traversal"></a>

**✅ Easy Answer:** Do not allow user input to pick arbitrary filesystem paths. Use allowlists and verify that resolved paths stay within an authorised directory.

**💻 Example:**

```javascript
const path = require('node:path');
const root = path.resolve('public');
const requested = 'image.png';
const candidate = path.resolve(root, requested);
if (!candidate.startsWith(root + path.sep)) throw new Error('Blocked');
console.log(candidate);
```

**🎯 Interview Tip:** Also consider symlinks and platform-specific filesystem behaviour.

---

### Q85. What is the built-in Node.js test runner?

<a id="q85-what-is-the-built-in-nodejs-test-runner"></a>

**✅ Easy Answer:** Node.js includes a test runner via `node:test`, so basic tests need no third-party framework.

**💻 Example:**

```javascript
const test = require('node:test');
const assert = require('node:assert/strict');
test('addition works', () => {
  assert.equal(2 + 3, 5);
});
```

**🎯 Interview Tip:** Run with `node --test` on a supported Node.js version.

---

### Q86. What is mocking in tests?

<a id="q86-what-is-mocking-in-tests"></a>

**✅ Easy Answer:** Mocking replaces dependencies with controlled behaviour, making tests faster and more predictable.

**💻 Example:**

```javascript
function greet(fetchName) { return 'Hi ' + fetchName(); }
const fakeFetchName = () => 'Jamshed';
console.log(greet(fakeFetchName));
```

**🎯 Interview Tip:** Mock external boundaries, but test real business logic.

---

### Q87. What is integration testing?

<a id="q87-what-is-integration-testing"></a>

**✅ Easy Answer:** Integration tests check whether components work together, such as an HTTP endpoint and a database or service.

**💻 Example:**

```javascript
// Example test target:
// GET /health -> HTTP 200 and body 'OK'
// Run server in test setup, send a request, assert response.
```

**🎯 Interview Tip:** Use a dedicated test database and clean test data.

---

### Q88. What is logging best practice?

<a id="q88-what-is-logging-best-practice"></a>

**✅ Easy Answer:** Use structured logs with levels, timestamps and request IDs. Do not log passwords, tokens or personal secrets.

**💻 Example:**

```javascript
const log = { level: 'info', event: 'user_created', userId: 'u42' };
console.log(JSON.stringify(log));
```

**🎯 Interview Tip:** Logs should help debugging without exposing confidential data.

---

### Q89. What is graceful shutdown?

<a id="q89-what-is-graceful-shutdown"></a>

**✅ Easy Answer:** On termination, stop accepting requests, finish in-flight work as appropriate and close connections before exiting.

**💻 Example:**

```javascript
const http = require('node:http');
const server = http.createServer((req, res) => res.end('OK')).listen(3000);
process.on('SIGTERM', () => {
  server.close(err => { if (err) process.exitCode = 1; });
});
```

**🎯 Interview Tip:** Real apps must also close database pools and define shutdown timeouts.

---

### Q90. How do you handle uncaught exceptions?

<a id="q90-how-do-you-handle-uncaught-exceptions"></a>

**✅ Easy Answer:** An uncaught exception means a serious error escaped normal handling. Log the failure and terminate safely; let a supervisor restart.

**💻 Example:**

```javascript
process.on('uncaughtException', err => {
  console.error('Fatal error:', err.message);
  process.exit(1);
});
```

**🎯 Interview Tip:** Do not continue normal operations after a fatal uncaught exception.

---

### Q91. What is health check vs readiness check?

<a id="q91-what-is-health-check-vs-readiness-check"></a>

**✅ Easy Answer:** A liveness check asks whether the process is alive. A readiness check asks whether the service can receive traffic.

**💻 Example:**

```javascript
// Example endpoints:
// GET /live  -> 200 if process is responsive
// GET /ready -> 200 only when critical dependencies are ready
```

**🎯 Interview Tip:** Do not make liveness depend on every downstream service.

---

### Q92. What is a production process manager?

<a id="q92-what-is-a-production-process-manager"></a>

**✅ Easy Answer:** A process manager or container orchestrator starts, monitors and restarts services and can coordinate deployments.

**💻 Example:**

```javascript
// Example PM2 commands (after installing pm2):
// pm2 start server.js --name api
// pm2 logs api
```

**🎯 Interview Tip:** PM2 is one option; systemd and orchestration platforms are alternatives.

---

### Q93. How do you debug Node.js applications?

<a id="q93-how-do-you-debug-nodejs-applications"></a>

**✅ Easy Answer:** Use breakpoints through the inspector, useful logs, profiling and error stacks.

**💻 Example:**

```javascript
// Terminal:
// node --inspect-brk app.js
// Open your debugger and attach.
```

**🎯 Interview Tip:** Do not expose inspector ports publicly.

---

### Q94. How do you use Node.js built-in fetch?

<a id="q94-how-do-you-use-nodejs-built-in-fetch"></a>

**✅ Easy Answer:** Modern Node.js provides a global `fetch` API for making HTTP requests.

**💻 Example:**

```javascript
async function load() {
  const response = await fetch('https://example.com');
  if (!response.ok) throw new Error(`HTTP ${response.status}`);
  console.log((await response.text()).slice(0, 30));
}
load().catch(console.error);
```

**🎯 Interview Tip:** Set timeouts and validate response formats in real services.

---

### Q95. What is AsyncLocalStorage?

<a id="q95-what-is-asynclocalstorage"></a>

**✅ Easy Answer:** `AsyncLocalStorage` keeps request-scoped context available across supported asynchronous operations, useful for correlation IDs.

**💻 Example:**

```javascript
const { AsyncLocalStorage } = require('node:async_hooks');
const store = new AsyncLocalStorage();
store.run({ requestId: 'req-1' }, () => {
  setTimeout(() => console.log(store.getStore().requestId), 0);
});
```

**🎯 Interview Tip:** Do not use it as global mutable business state.

---

### Q96. What is a zero-downtime deployment strategy?

<a id="q96-what-is-a-zero-downtime-deployment-strategy"></a>

**✅ Easy Answer:** Start healthy new instances, move traffic gradually, then drain and stop old instances without dropping active requests.

**💻 Example:**

```javascript
// Deployment outline:
// 1. Start new instance
// 2. Wait for readiness
// 3. Route traffic to new instance
// 4. Drain old instance
```

**🎯 Interview Tip:** Database migrations must remain compatible during a rolling deployment.

---

### Q97. What is the best way to prepare a Node.js app for production?

<a id="q97-what-is-the-best-way-to-prepare-a-nodejs-app-for-production"></a>

**✅ Easy Answer:** Use a supported LTS release, validate configuration, lock dependencies, test APIs, secure secrets, add monitoring and handle shutdown.

**💻 Example:**

```javascript
// Terminal examples:
// npm ci
// npm test
// NODE_ENV=production node server.js
```

**🎯 Interview Tip:** Production readiness is a checklist, not a single configuration flag.

---

### Q98. What is API versioning?

<a id="q98-what-is-api-versioning"></a>

**✅ Easy Answer:** API versioning lets clients move between changing API contracts without sudden breakage.

**💻 Example:**

```javascript
// Example route versions:
// GET /api/v1/users
// GET /api/v2/users
```

**🎯 Interview Tip:** Avoid changing existing API responses without a migration plan.

---

### Q99. What are idempotent HTTP requests?

<a id="q99-what-are-idempotent-http-requests"></a>

**✅ Easy Answer:** An idempotent operation produces the same intended server state when repeated. GET, PUT and DELETE are idempotent by definition of their semantics.

**💻 Example:**

```javascript
// PUT /users/42 with the same body twice
// should leave the resource in the same intended state.
```

**🎯 Interview Tip:** A repeated request may still produce different logs or response metadata.

---

### Q100. How can you avoid duplicate jobs?

<a id="q100-how-can-you-avoid-duplicate-jobs"></a>

**✅ Easy Answer:** Use unique job IDs or database constraints and make handlers safe to retry when possible.

**💻 Example:**

```javascript
const processed = new Set();
function handle(id) {
  if (processed.has(id)) return 'already done';
  processed.add(id); return 'processed';
}
console.log(handle('job-1'), handle('job-1'));
```

**🎯 Interview Tip:** An in-memory Set is only a demo; production multi-instance systems need durable coordination.

---

## 🎓 Interview Preparation Roadmap

1. **Start with fundamentals:** runtime, npm, modules and core APIs.
2. **Practise async logic:** promises, callbacks, event loop and error handling.
3. **Build APIs:** HTTP, authentication, validation, pagination and logging.
4. **Go deeper:** streams, performance, workers and scaling.
5. **Prepare for production:** security, testing, observability and deployment.

## 🔗 Official References

- [Node.js Documentation](https://nodejs.org/api/)
- [Node.js Learning](https://nodejs.org/en/learn)
- [Node.js Release Schedule](https://github.com/nodejs/Release)
- [npm Documentation](https://docs.npmjs.com/)

## 🤝 Contributing

Found an error or want to improve an explanation? Open an issue or submit a pull request. Keep examples small, accurate, and beginner-friendly.

## ⭐ Support

If these notes helped your interview preparation, **star this repository** and share it with your friends.

<div align="center">

**Created by [Code with Jamshed](https://github.com/Jamshed7664) • Happy Coding! 💚**

</div>
