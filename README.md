# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js where long-running operations in request handlers can block the event loop, causing the server to appear unresponsive.  The `server.js` file contains the buggy code, and `serverSolution.js` provides a solution using asynchronous operations.

## Problem

The original `server.js` simulates a long-running task (5-second delay) within the request handler. This blocks the event loop, preventing the server from accepting new requests or responding to existing ones promptly.  This results in a server hang.