# Google Docs Clone

Built to replicate the usability of Google docs.

## Requirements

1. Mongo DB
2. Node (12.13.0 +)

## Features

<ul>
<li>Unique IDs per session</li>
<li>Live updates if a URL is shared with another user</li>
<li>Saves every 2 seconds to instance based on URL ID</li>
<li>Rich text editor from QuillJS</li>
<li>Print friendly</li>
</ul>

## Project Architecture

The project is divided into 2 parts: `Client` and `Server`

### Client:
The client is React application that uses [Quill](https://www.npmjs.com/package/quill) as a WYSIWYG text editor that emits events based on the user changes

### Server:
The server is a NodeJS script that uses [Socket.IO](https://socket.io/) to handle the user events and store them in MongoDB


## Installation 

In order to install the application, you have to do an `npm install` in each repository as below
* Clone The repo

* Install the server
```bash
cd server && npm install 
```
* Install the client
```bash
cd client && npm install
```
* Run the server
```bash
cd server && npm run start
```
* Run the client
```bash
cd client && npm run start
```
* Make sure that you have MongoDB Schema `google-docs-clone` working on your local machine


## Contributing
Pull requests are welcome. 
