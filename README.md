# dev-server

Serving static files and directory indexes for you  
This package is a fork of original [dev-server](https://github.com/langpavel/node-dev-server) package by [Pavel Lang](https://github.com/langpavel).  
Main change is using cors middleware for CORS error case, when you want to connect static dev-server file into external dev-server which on another address or port.

## Quick usage
```
$ npx freecors-dev-server
```

## Install

```
$ npm install freecors-dev-server -g
```

## Run

```
$ DEV_SERVER_PORT=4000 DEV_SERVER_ROOT=. dev-server
```

### Environment Variables

- `DEV_SERVER_PORT` — port to listen, default 4000
- `DEV_SERVER_ROOT` — root directory

### Special files

File `dev-server-hooks.js` or `.dev-server-hooks.js` is loaded
on start and called with express app instance
