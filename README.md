# All A-Board

A framework for writing your own multiplayer board games. The framework consists of a client and a server componenet. The client is created using React Native, and can be run on the web or on mobile devices. The server is written in Node, and a default deployment exists on Heroku.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment section in the respective readme for client and server, for notes on how to deploy the project.

### Prerequisites

- [Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- Expo CLI (`npm install expo-cli --global`)

### Setting up the development environment

This repo has two git submodules for server and client. You'll have to clone recursively to get them.

```
git clone --recurse-submodules https://github.com/ammubhave/all-aboard.git
```

If you have already cloned the repository without initializing the submodules, run the following.

```
git submodule update --init
```

You'll find instructions both [server](https://github.com/ammubhave/all-aboard-server/blob/master/README.md) and [client](https://github.com/ammubhave/all-aboard-client/blob/master/README.md) in their respective README.md files.

The client requires the server to be already running, otherwise it won't be able to connect to it. The web client uses the production instance of the server by default. If you are developing locally, you will have to edit the SERVER_URI variable to point to your local instance.

The expo app for mobile devices uses expo releases to select which URL to use for the server. By default, it will use the actual production server URL.
